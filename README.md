# Civil Infrastructure Platform

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The Civil Infrastructure Platform (CIP) is a Linux Foundation collaborative project that builds an industrial-grade open source base layer for civil infrastructure systems such as transportation, power generation and distribution, building and city management, industrial control, and healthcare equipment. CIP curates a Super Long-Term Support (SLTS) kernel and core user-space packages that can be maintained for more than ten years, plus working groups for security (IEC 62443 alignment), software update, real-time, and testing. CIP's primary programmable interface is source code — the kernel, CIP Core images and tooling published through GitLab and Debian-derived package archives — and it publishes machine-readable product lifecycle data for those. CIP also serves one live REST API: its own event calendar at cip-project.org/wp-json, declared in an RFC 9727 /.well-known/api-catalog and described by OpenAPI documents the site serves itself.

**Areas:** Embedded · Industrial · Infrastructure · Linux · Linux Foundation · Long-Term Support · Open Source

## Civil Infrastructure Platform on APIs.io

Everything profiled for Civil Infrastructure Platform is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/civil-infrastructure-platform/](https://apis.io/providers/civil-infrastructure-platform/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [CIP SLTS Kernel](https://apis.io/apis/civil-infrastructure-platform/cip-kernel/) — The CIP Kernel is a Super Long-Term Support (SLTS) Linux kernel branch maintained for ten or more years, providing a stable base for industrial systems that…
- [CIP Core Packages](https://apis.io/apis/civil-infrastructure-platform/cip-core/) — CIP Core provides a curated set of Debian-derived user-space packages aligned with the SLTS kernel to deliver a complete reference platform for civil…
- [CIP Software Update](https://apis.io/apis/civil-infrastructure-platform/cip-software-update/) — The CIP Software Update working group maintains tooling such as SWUpdate and hawkBit-based servers used to deliver secure over-the-air updates across…
- [CIP Security](https://apis.io/apis/civil-infrastructure-platform/cip-security/) — The CIP Security working group aligns the CIP base layer with IEC 62443-4-1 and 62443-4-2 industrial cybersecurity requirements and tracks CVE handling…
- [CIP Testing](https://apis.io/apis/civil-infrastructure-platform/cip-testing/) — The CIP Testing working group runs continuous-integration and hardware-in-the-loop testing on member-supplied boards to validate kernel and core packages…
- [Civil Infrastructure Platform Website (WordPress REST)](https://apis.io/apis/civil-infrastructure-platform/cip-project-org-website-wordpress-rest/) — The public WordPress REST API (wp-json) of the Civil Infrastructure Platform website at cip-project.org: the route index of the site's content management…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [civil-infrastructure-platform](https://apis.io/servers/civil-infrastructure-platform/civil-infrastructure-platform/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Civil Infrastructure Platform Context](https://apis.io/jsonld/civil-infrastructure-platform/civil-infrastructure-platform-context/)

#### Overlays (3)

OpenAPI overlays, including conversational phrasing for each operation.

- [Civil Infrastructure Platform Events Overlay](https://apis.io/overlays/civil-infrastructure-platform/civil-infrastructure-platform-events-overlay/)
- [Civil Infrastructure Platform Tec V1 Overlay](https://apis.io/overlays/civil-infrastructure-platform/civil-infrastructure-platform-tec-v1-overlay/)
- [Civil Infrastructure Platform Zapier Overlay](https://apis.io/overlays/civil-infrastructure-platform/civil-infrastructure-platform-zapier-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Civil Infrastructure Platform API Rules](https://apis.io/rules/civil-infrastructure-platform/civil-infrastructure-platform-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Civil Infrastructure Platform Authentication](https://apis.io/security/civil-infrastructure-platform/civil-infrastructure-platform-authentication/)
- [Civil Infrastructure Platform Domain Security](https://apis.io/security/civil-infrastructure-platform/civil-infrastructure-platform-domain-security/)
- [Civil Infrastructure Platform Vulnerability Disclosure](https://apis.io/security/civil-infrastructure-platform/civil-infrastructure-platform-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Civil Infrastructure Platform Plans Pricing](https://apis.io/plans/civil-infrastructure-platform/civil-infrastructure-platform-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Civil Infrastructure Platform Rate Limits](https://apis.io/rate-limits/civil-infrastructure-platform/civil-infrastructure-platform-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Civil Infrastructure Platform Finops](https://apis.io/finops/civil-infrastructure-platform/civil-infrastructure-platform-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.cip-project.org/)
- [Documentation](https://cip-documents.readthedocs.io/)
- [API reference](https://cip-project.org/wp-json/tec/v1/docs)
- [Pricing](https://cip-project.org/about/join)
- [Sign up](https://enrollment.lfx.linuxfoundation.org/?project=cip)
- [Support](https://lists.cip-project.org/g/cip-dev)
- [Blog](https://cip-project.org/blog/)
- [Security](https://wiki.linuxfoundation.org/civilinfrastructureplatform/cipkernelmaintenance#security_fixes)
- [Compliance](https://www.bestpractices.dev/projects/10564)
- [Terms of service](https://www.linuxfoundation.org/terms)
- [Privacy policy](https://www.linuxfoundation.org/privacy)
- [GitHub](https://github.com/cip-project)

## API Evangelist rating

**Kin Score 34.8** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 10.7 |
| Contract governance | 29.5 |
| Operational transparency | 28.9 |
| Developer ergonomics | 37.5 |
| Access clarity | 39.5 |

**Agent readiness 9.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/civil-infrastructure-platform/](https://apis.io/providers/civil-infrastructure-platform/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Civil Infrastructure Platform: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/civil-infrastructure-platform/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
