# Commonplace Content Model

**Status:** Approved v0.1  
**Scope:** Content requirements and editorial metadata for the Commonplace MVP

## 1. Purpose

This document defines the kinds of content Commonplace publishes, the information recorded about each item, and the relationships between items. It is a content and editorial specification, not a decision about storage technology, database design, URL implementation, or a particular schema language.

The model supports three connected activities:

- **Discover:** find and evaluate useful developer resources.
- **Learn:** read original and community-authored technical knowledge.
- **Contribute:** submit resources, knowledge, corrections, and practical experience.

Published public content remains GitHub-source-controlled, as specified in the approved product strategy.

## 2. Content origins and provenance

Every published item must make its origin clear. Use one primary provenance value:

| Value | Meaning |
|---|---|
| `commonplace_editorial` | Original content written and maintained by the Commonplace editorial team |
| `community_contributed` | Content submitted or authored by a community contributor |
| `external_resource` | A third-party resource described or linked by Commonplace |
| `maintainer_curated` | A collection or learning track assembled and maintained by Commonplace maintainers |

Provenance describes origin or editorial responsibility; it is not a quality rating, endorsement, or verification result. A maintainer-curated collection may contain items from several origins. The origin of each included item must remain visible.

## 3. Discover resource types

The MVP includes exactly these five Discover categories:

1. **Prompts** — reusable instructions for coding, debugging, research, UI/UX, productivity, and related developer tasks.
2. **Skills** — task or domain capabilities and instructions intended for compatible AI tools or development environments.
3. **MCP Servers** — Model Context Protocol servers and integrations, including their setup, capabilities, permissions, and security considerations.
4. **Developer Tools** — software, IDEs, extensions, APIs, services, utilities, and relevant open-source projects.
5. **Rules & Configurations** — project instructions and configuration conventions such as AGENTS.md, CLAUDE.md, GEMINI.md, editor rules, and coding standards.

Each resource record should explain what the resource does, who it is for, how to evaluate or use it, and what limitations or risks are known. A record describing an external resource is not an endorsement of that resource.

## 4. Learn content forms

Learn supports the approved subject areas: Start Here, Developer Fundamentals, AI Engineering and AI-assisted Development, Secure Development, Software Architecture, SEO & Website Growth, GEO & AI Search Visibility, UI/UX & Accessibility, Testing & QA, Deployment & Infrastructure, Legal Awareness, and practical guides and learning tracks.

Content may take these forms:

- **Guide:** structured explanation that helps a reader understand or complete a task.
- **Tutorial:** a sequenced, hands-on walkthrough with prerequisites and expected outcomes.
- **Article / Explainer:** an original or contributed discussion of a concept, technique, decision, or engineering experience.
- **Reference:** organised factual material intended for lookup.
- **Checklist:** a concise set of actionable review or completion steps.
- **Learning Track:** a maintained sequence of related learning items with an intended progression.

Commonplace-authored technical articles and tutorials are first-class Learn content alongside community contributions. Their authorship and maintenance responsibility must be explicit. Editorial authorship does not by itself mean independent verification.

## 5. Shared metadata

Published items should carry the following fields where they are meaningful and known. Unknown values should be omitted or stated as unknown; they must not be invented.

| Field | Purpose |
|---|---|
| `id` | Stable internal identifier |
| `title` | Human-readable title |
| `slug` | Human-readable identifier for routing |
| `summary` | Concise statement of purpose and value |
| `content_type` | Resource type or Learn content form |
| `category` | Approved Discover or Learn category |
| `provenance` | Origin value from Section 2 |
| `authors` | Named authors or credited contributors |
| `maintainers` | Person or team responsible for upkeep |
| `tags` | Useful descriptive terms |
| `audience` | Intended reader or experience level |
| `prerequisites` | Knowledge, tools, or setup needed |
| `canonical_source` | Primary source, project, or canonical URL where applicable |
| `references` | Supporting sources and further reading |
| `license` | Applicable content or resource licence, when known |
| `version` | Version of the item or referenced resource, when applicable |
| `compatibility` | Supported tools, platforms, versions, or environments |
| `published_at` | Initial publication date |
| `updated_at` | Most recent substantive update |
| `last_reviewed_at` | Date of the latest recorded review |
| `review_status` | Editorial review state and relevant review dimensions |
| `lifecycle_status` | Current publication lifecycle state |

Metadata requirements may vary by content type. The implementation must not require fabricated values merely to fill optional fields.

## 6. Type-specific metadata

### 6.1 Discover resources

As applicable, record:

- Official name, publisher, author, and maintainer.
- Official website and source repository.
- Resource purpose, capabilities, and intended use.
- Installation, setup, or usage instructions.
- Supported versions, platforms, dependencies, and compatibility.
- Licence or reuse terms, with a clear unknown state when unavailable.
- Maintenance signals such as latest release or last observed update.
- Required permissions, data access, network access, and potentially destructive capabilities.
- Known limitations, risks, and relevant security advisories.
- Date and scope of the latest verification.

For MCP servers, skills, prompts, and rules/configurations, describe how a user can inspect and use the item safely. Commonplace must not execute contributed content as part of publication or review.

### 6.2 Guides, tutorials, articles, references, and checklists

As applicable, record:

- Intended outcome and audience.
- Prerequisites and required environment.
- Estimated effort only when there is a reasonable basis.
- Steps, examples, expected results, and troubleshooting notes.
- Limitations, caveats, and version-sensitive details.
- Sources supporting factual and technical claims.
- Author, editorial owner, and review date.

Code examples must identify relevant language, runtime, framework, or version assumptions. Untested examples must be labelled honestly.

### 6.3 Learning tracks

Record the track's purpose, intended audience, prerequisites, learning outcomes, ordered items, optional items, and maintainer. Each included item remains independently attributed and retains its own provenance. Tracks are editorial learning sequences, not personal progress trackers.

### 6.4 Editorial collections

Record the collection's purpose, curator or maintainer, inclusion criteria, and ordered or grouped entries. Collections are public, maintainer-curated groupings. They are not private user notebooks, personal bookmarks, or a templates library.

## 7. Review dimensions

A single review label must not imply that every aspect of an item has been verified. Track review dimensions separately where applicable:

- Content and editorial quality reviewed.
- Primary source checked.
- Attribution and authorship checked.
- Licence and reuse terms checked.
- Required metadata reviewed.
- Compatibility checked.
- Security considerations reviewed.

A security review is a distinct activity and must only be marked as performed when it actually occurred. Editorial review is not a penetration test, formal security audit, legal opinion, or guarantee that third-party software is safe.

## 8. Lifecycle states

Use these lifecycle states to describe publication and maintenance:

| State | Meaning |
|---|---|
| `draft` | Being prepared; not public |
| `in_review` | Awaiting or undergoing review |
| `approved` | Accepted for publication but not necessarily published yet |
| `published` | Publicly available |
| `needs_update` | Published item requires correction or re-verification |
| `archived` | Retained for historical context but no longer actively maintained |
| `withdrawn` | Removed from active publication, with an appropriate explanation where possible |

Contribution workflow statuses (Submitted, Reviewing, Changes requested, Approved, Published, Rejected) describe the submission process and are not substitutes for an item's lifecycle state.

## 9. Relationships between content

Content may reference and link to other content:

- A resource may be explained by one or more guides.
- A guide may recommend or compare relevant resources.
- A learning track may order guides, articles, and resources.
- A collection may group items across categories and provenance.
- An article may link to primary sources, standards, and further reading.

Relationships should be intentional, descriptive, and maintained. A link or inclusion does not imply endorsement.

## 10. Versioning and maintenance

Version-sensitive resources and instructions should identify the version or date to which they apply. When a change materially affects compatibility, setup, security, or correctness, update the item and its review information. Older material may be archived or marked as needing an update rather than silently presented as current.

Published content is maintained through the repository's Git history and review process. Immutable versioned URLs, content hashes, automated update detection, and detailed compatibility matrices are implementation decisions for later architecture work; this document does not require them for the MVP.

## 11. Attribution, licensing, and permissions

Every item must distinguish original Commonplace writing, community-authored work, and third-party material. Credit authors and sources clearly. Do not copy or republish third-party material without permission or a licence that allows the intended use.

The platform source-code licence, Commonplace editorial-content licence, contributor terms, and treatment of third-party resources are not finalised by this document. They remain explicit project decisions. Until those decisions are approved and published, contributors must not be told that submission automatically grants a particular licence or that public availability means permission to reuse.

## 12. Safety and trust

- Do not execute submitted prompts, skills, scripts, MCP servers, or other contributed code on Commonplace infrastructure.
- Treat external content and installation instructions as untrusted until reviewed.
- Describe permissions, data access, network access, and destructive actions when known.
- Do not label an item secure, verified, official, or endorsed without evidence and a clearly defined basis.
- Preserve provenance, source links, review dates, and known limitations.
- Escalate suspected malicious content or vulnerabilities through the repository's security reporting process.

## 13. Decisions reserved for implementation

The following remain open for later technical architecture and implementation planning: file formats and schema language; directory layout; identifiers and URL rules; search indexing; tag and category vocabularies beyond the approved categories; automated freshness checks; review tooling; and any future migration or API strategy. This document defines the content requirements without prematurely selecting those mechanisms.
