---
name: Read CIP events, venues and organizers
description: Fetch the Civil Infrastructure Platform community event calendar — upcoming events, their venues and their organizers — from the public, unauthenticated CIP REST API.
api: openapi/civil-infrastructure-platform-tec-v1-openapi-original.json
operations: [getEvents, getEvent, getVenues, getVenue, getOrganizers, getOrganizer, getSeries]
generated: '2026-09-05'
method: generated
source: openapi/civil-infrastructure-platform-tec-v1-openapi-original.json
---

# Read CIP events, venues and organizers

The Civil Infrastructure Platform publishes its mini-summit and community event calendar
through a REST API on its own site. Reads of published records need no credentials.

**Base URL:** `https://cip-project.org/wp-json/tec/v1`
(the older, wider surface is `https://cip-project.org/wp-json/tribe/events/v1` — see "Two namespaces" below)

## Auth

None for published reads. Confirmed live: `GET /wp-json/tribe/events/v1/events` returns 200 anonymously.
Writes require HTTP Basic with a WordPress Application Password — see
`authentication/civil-infrastructure-platform-authentication.yml`. Do not attempt writes; CIP has not
issued credentials for this surface.

## Steps

1. **List events** — `getEvents` (`GET /events`).
   Useful parameters, all declared in the spec: `page`, `per_page`, `search`,
   `start_date`, `end_date`, `status`, `order`, `orderby`.
   Read `total` and `total_pages` from the body, or the `X-WP-Total` / `X-WP-TotalPages`
   response headers, to decide whether to page.
2. **Page** by incrementing `page`. The body also carries `next_rest_url` / `previous_rest_url`;
   follow those rather than constructing URLs.
3. **Fetch one event** — `getEvent` (`GET /events/{id}`) when you need the full record.
   The event representation embeds its venue and organizer objects in full; there is no
   expand or sparse-fieldset parameter, so do not ask for one.
4. **Resolve places and people separately** when you want the catalogue rather than one
   event: `getVenues` (`GET /venues`) and `getOrganizers` (`GET /organizers`), each with the
   same `page` / `per_page` / `search` shape, then `getVenue` / `getOrganizer` by id.
5. **Series** — `getSeries` (`GET /series`) exposes recurring-event series where the site
   defines them.

## Error handling

Errors are the WordPress envelope, **not** RFC 9457 problem+json:

```json
{"code":"rest_no_route","message":"No route was found matching the URL and request method.","data":{"status":404}}
```

Read `data.status`, not just the HTTP code. The catalogue of declared responses is in
`errors/civil-infrastructure-platform-problem-types.yml`. On a read path expect:

- `400` — a query variable is in the wrong format. Fix the parameter; do not retry unchanged.
- `404` — the record does not exist, or you paged past the end (`The requested page was not found`).
- `401` / `403` — you asked for something that is not published. Do not retry with guesses.

## Rate limits and caching

None are published, and none appear on a live response — no `RateLimit-*`, no `Retry-After`,
no 429 in the contract. Responses are `cache-control: public, max-age=604800`, so cache
aggressively and poll no more than daily; a week-old cached calendar is what the origin is
serving you anyway.

## Two namespaces

CIP serves the same data through two versioned namespaces with no stated retirement plan:

- `tec/v1` — 17 operations, named `operationId`s, a declared `BasicAuth` scheme. Prefer this one.
- `tribe/events/v1` — 30 operations including event categories and tags, but **no**
  `operationId`s at all. Use it only for `/categories` and `/tags`, which `tec/v1` does not carry.

Both are described by OpenAPI documents the site serves at `/wp-json/tec/v1/docs` and
`/wp-json/tribe/events/v1/doc`.

## What this API is not

This is the CIP **website's** event calendar. It is not an interface to the SLTS kernel, CIP Core,
the CVE tracker or the testing lab — those are source trees and mailing lists, not APIs. See
`lifecycle/civil-infrastructure-platform-lifecycle.yml` for the machine-readable kernel support
schedule, which is a YAML dataset in GitLab rather than an endpoint.
