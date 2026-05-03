# Versioning Protocols (versioning-protocols)
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
