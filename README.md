# Konfig (konfig)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

> **Status: Sunset (December 2024).** Konfig was a developer-tools startup focused on automatic SDK, API documentation, demo, and tutorial generation from OpenAPI Specifications and Postman Collections. Founder Dylan Huang publicly closed the company on November 25, 2024, and the flagship `konfig-dev/konfig` repository's GitHub description now reads "SDK & API Docs Generator. Sunset as of December 2024." The category has consolidated around Stainless, Fern, Speakeasy, and the OpenAPI Generator open-source project.

Konfig's developer platform generated and published SDKs in Python, TypeScript, Java, C#, Go, Ruby, PHP, Swift, and Kotlin, paired with auto-synchronized API reference documentation, interactive markdown demos, and onboarding tutorials. Delivery was through the `konfig-cli` command-line tool and a GitHub Actions automation pipeline that republished SDKs when the upstream OpenAPI spec changed. Konfig itself never exposed a public REST API for its platform; commercial usage was sold contact-sales through the "Schedule a Demo" funnel.

This API Evangelist index is retained as a historical record of the platform, its public properties, and its place in the SDK-generation tooling landscape.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/konfig/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Status:** Sunset
- **Sunset Date:** 2024-12-25
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- API Documentation
- CLI
- Developer Tools
- OpenAPI
- Postman
- SDK Generation
- Sunset

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-22

## APIs

### Konfig SDK Generation Platform (Sunset)

Konfig's developer platform for generating, validating, and publishing SDKs, API reference documentation, and interactive tutorials from OpenAPI specifications and Postman Collections. Delivered primarily through the `konfig-cli` command-line interface and a GitHub Actions integration that republished SDKs on spec change. Konfig never published a public REST API for the platform itself, so the surface profiled here is the CLI + GitHub Actions + hosted-docs offering rather than a callable HTTP API. The platform was sunset in December 2024 along with the `konfigthis.com` hosted offering.

**Human URL:** [https://konfigthis.com/](https://konfigthis.com/)

#### Properties

- [Documentation](https://konfigthis.com/docs/)
- [Getting Started](https://konfigthis.com/docs/getting-started/openapi-specification/)
- [Interactive Tutorial](https://konfigthis.com/interactive-tutorial/)
- [GitHub Generator (konfig-dev/konfig)](https://github.com/konfig-dev/konfig)
- [Getting Started Example](https://github.com/konfig-dev/getting-started-example)
- [Closure Announcement](https://dylanhuang.com/blog/closing-my-startup/)

## Provider

- **Legal Name:** Konfig
- **Founder:** Dylan Huang
- **Status:** Sunset (2024-12-25)
- **Closure Announcement:** [Closing My Startup (Dylan Huang)](https://dylanhuang.com/blog/closing-my-startup/)
- **GitHub Org:** [github.com/konfig-dev](https://github.com/konfig-dev) (58 repos)
- **Flagship Repo:** [konfig-dev/konfig](https://github.com/konfig-dev/konfig) (1,531 stars at sunset)
- **Competitive Context:** Stainless, Fern, Speakeasy, OpenAPI Generator

## Common Properties

- [Website](https://konfigthis.com/)
- [Documentation](https://konfigthis.com/docs/)
- [Getting Started](https://konfigthis.com/docs/getting-started/openapi-specification/)
- [Blog](https://konfigthis.com/blog/) (last post April 30, 2024)
- [GitHub Org](https://github.com/konfig-dev)
- [GitHub Generator](https://github.com/konfig-dev/konfig)
- [GitHub Automation](https://github.com/konfig-dev/automation)
- [GitHub Backstage Plugin](https://github.com/konfig-dev/backstage-plugin-konfig)
- [LinkedIn](https://www.linkedin.com/company/konfig)
- [Schedule Demo](https://konfigthis.com/schedule-demo/)
- [Closure Announcement](https://dylanhuang.com/blog/closing-my-startup/)
- [Plans (Historical Scaffold)](plans/konfig-plans-pricing.yml)
- [Rate Limits (Historical Scaffold)](rate-limits/konfig-rate-limits.yml)
- [FinOps (Historical Scaffold)](finops/konfig-finops.yml)

## Archived Blog Content

A historical mirror of 22 Konfig blog posts (October 2023 - April 2024) is preserved under [`blogs/`](blogs/), including changelogs #7-#11, the "Introducing Konfig SDKs" launch post, the "Why We Pivoted Away From B2B Gaming" retrospective, and the company's "10 Best APIs" listicle series.

## Notable Absences

- No public OpenAPI specification — Konfig generated SDKs from other providers' OpenAPI specs but never published one for its own platform.
- No public pricing page — `konfigthis.com/pricing/` returns HTTP 404.
- No published rate limits — the platform was contact-sales, not a metered API.
- No RSS feed for the blog; the blog has not been updated since April 30, 2024.
- No active GitHub releases since December 2024.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
