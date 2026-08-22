# Versioning Protocols (versioning-protocols)

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

Standards and methodologies for managing changes and updates to APIs, software interfaces, and data formats while maintaining backward compatibility and clear communication of breaking changes. Covers Semantic Versioning (SemVer), Calendar Versioning (CalVer), URI path versioning, header-based versioning, and deprecation management strategies.

**URL:** [https://semver.org/](https://semver.org/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - API Design, Backward Compatibility, Software Development, Version Control, Semantic Versioning, API Lifecycle, Deprecation

## Timestamps

- **Created:** 2025
- **Modified:** 2026-05-03

## APIs

### Semantic Versioning (SemVer)
Semantic Versioning uses a MAJOR.MINOR.PATCH format where MAJOR increments denote breaking changes, MINOR increments indicate new backward-compatible features, and PATCH increments represent backward-compatible bug fixes. SemVer 2.0.0 is the canonical specification.

**Human URL:** [https://semver.org/](https://semver.org/)

#### Tags:

 - Semantic Versioning, SemVer, Breaking Changes, API Versioning

#### Properties

- [Documentation](https://semver.org/)
- [Specification](https://semver.org/spec/v2.0.0.html)
- [JSONSchema](json-schema/versioning-protocols-semver-schema.json)
- [JSONStructure](json-structure/versioning-protocols-semver-structure.json)

### Calendar Versioning (CalVer)
Calendar Versioning uses the release date as the version identifier, typically in YYYY.MM.DD or YYYY-MM-DD format. Used by APIs like Stripe to communicate when an API version was released.

**Human URL:** [https://calver.org/](https://calver.org/)

#### Tags:

 - Calendar Versioning, CalVer, Date-Based Versioning, API Versioning

#### Properties

- [Documentation](https://calver.org/)
- [JSONSchema](json-schema/versioning-protocols-calver-schema.json)

### URI Path Versioning
URI path versioning embeds the API version in the URL path (e.g., /v1/users, /v2/users). The most widely adopted strategy for public REST APIs due to its explicitness and cache-friendliness.

**Human URL:** [https://www.askantech.com/api-versioning-strategies-rest-header-url-deprecation-guide/](https://www.askantech.com/api-versioning-strategies-rest-header-url-deprecation-guide/)

#### Tags:

 - URI Versioning, Path Versioning, REST, API Design

#### Properties

- [Documentation](https://www.askantech.com/api-versioning-strategies-rest-header-url-deprecation-guide/)
- [JSONSchema](json-schema/versioning-protocols-uri-path-versioning-schema.json)

### Header-Based Versioning
Header-based versioning passes the API version in a custom HTTP request header (e.g., API-Version: 2026-04-01), keeping URLs clean and enabling more granular version control.

**Human URL:** [https://redocly.com/blog/api-versioning-best-practices](https://redocly.com/blog/api-versioning-best-practices)

#### Tags:

 - Header Versioning, Content Negotiation, REST, API Design

### OpenAPI Versioning
OpenAPI handles versioning through the info.version field, the deprecated flag, and multiple server entries. Tools like oasdiff enable automated breaking change detection.

**Human URL:** [https://openapispec.com/docs/how/how-does-openapi-handle-api-versioning/](https://openapispec.com/docs/how/how-does-openapi-handle-api-versioning/)

#### Tags:

 - OpenAPI, API Specification, Breaking Changes, Deprecation

## Common Properties

- [Website](https://semver.org/)
- [Documentation](https://semver.org/spec/v2.0.0.html)

## Features

| Name | Description |
|------|-------------|
| Semantic Versioning | MAJOR.MINOR.PATCH versioning that communicates the impact of changes on API consumers. |
| Calendar Versioning | Date-based versioning (YYYY.MM.DD) that communicates the freshness of an API release. |
| URI Path Versioning | Embedding the API major version in the URL path for explicit, cache-friendly versioning. |
| Header-Based Versioning | Passing the API version in HTTP headers for clean URL structures and content negotiation. |
| Deprecation Management | Structured policies for communicating and retiring old API versions with adequate notice. |
| Breaking Change Detection | Tooling and processes to identify breaking changes between API versions using spec diffing. |
| N-2 Support Policy | Support policy maintaining the current major version plus the two previous versions. |

## Use Cases

| Name | Description |
|------|-------------|
| API Lifecycle Governance | Establish organizational versioning policies that balance innovation with backward compatibility. |
| Breaking Change Communication | Communicate breaking changes clearly to API consumers with version bumps and deprecation notices. |
| Multi-Version Support | Maintain multiple active API versions simultaneously to support consumers at different adoption stages. |
| Automated Change Detection | Integrate spec diffing tools into CI/CD pipelines to detect breaking changes before release. |
| Deprecation Planning | Plan and execute API version deprecations with 12-18 months notice and migration guides. |

## Integrations

| Name | Description |
|------|-------------|
| Kong API Gateway | Deploy version routing plugins and deprecation headers in Kong. |
| Apigee | Support versioned API proxies and detailed version analytics. |
| AWS API Gateway | Run different stages for version control in AWS API Gateway. |
| Azure API Management | First-class support for multiple API versions and revisions in Azure APIM. |
| oasdiff | Open-source tool for detecting breaking changes between OpenAPI specification versions. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [versioning-protocols-semver-schema.json](json-schema/versioning-protocols-semver-schema.json)
- [versioning-protocols-calver-schema.json](json-schema/versioning-protocols-calver-schema.json)
- [versioning-protocols-uri-path-versioning-schema.json](json-schema/versioning-protocols-uri-path-versioning-schema.json)

### JSON Structure

- [versioning-protocols-semver-structure.json](json-structure/versioning-protocols-semver-structure.json)
- [versioning-protocols-calver-structure.json](json-structure/versioning-protocols-calver-structure.json)
- [versioning-protocols-uri-path-versioning-structure.json](json-structure/versioning-protocols-uri-path-versioning-structure.json)

### JSON-LD

- [versioning-protocols-context.jsonld](json-ld/versioning-protocols-context.jsonld)

## Vocabulary

- [Versioning Protocols Vocabulary](vocabulary/versioning-protocols-vocabulary.yaml) — Unified taxonomy mapping 4 resources, 6 actions, 1 workflow, and 3 personas across versioning standards and practices

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
