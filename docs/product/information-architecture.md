# Information Architecture

**Version:** 0.1  
**Status:** Approved  
**Stage:** 2 — Information Architecture  
**Scope:** Commonplace MVP

## 1. Purpose

This document defines the MVP's information architecture: its primary navigation, sitemap, content areas, shared page types, search boundaries, and cross-linking model.

Commonplace is an open knowledge platform for people who build with technology. It brings together three equally important activities:

- **Discover** useful developer resources.
- **Learn** concepts and practices that help people build better software.
- **Contribute** resources and knowledge to the shared collection.

The primary navigation also includes **About**, which explains the project's purpose, principles, and governance. About is an informational destination, not a fourth product pillar.

## 2. Primary navigation

The MVP has four primary navigation destinations:

1. **Discover** — browse and evaluate practical developer resources.
2. **Learn** — read guides and follow structured learning tracks.
3. **Contribute** — understand contribution options, submit material, and follow the review process.
4. **About** — understand Commonplace, its principles, governance, and open-source approach.

A global search entry point is available throughout the site. Search is a shared utility rather than a fifth primary navigation destination.

Navigation must remain understandable on small phones, foldable cover and inner screens, tablets, laptops, and desktop displays. The presentation may adapt by viewport; the information hierarchy should remain consistent.

## 3. Sitemap

### 3.1 Home

The homepage introduces the purpose of Commonplace and provides clear routes into the three product pillars.

Proposed sections:

- Search-led introduction.
- Three primary destinations: Discover, Learn, and Contribute.
- Recently added or updated entries, based on real published content.
- Editorial collections curated by maintainers.
- Trust and editorial-principles explanation.
- Short About introduction.
- Footer links to project, policy, and contribution information.

Do not display invented activity counts, popularity metrics, testimonials, or verification claims.

### 3.2 Discover

Discover is the public directory for the five approved MVP resource categories.

#### Prompts

Organize prompt entries by practical purpose, including:

- Coding and development.
- Debugging and code explanation.
- System prompts and agent instructions.
- UI/UX and design work.
- Research and productivity.

A prompt detail page should explain its intended task, expected inputs, usage guidance, limitations, attribution, and source where applicable.

#### Skills

Include skills for AI coding agents and developer workflows, including tool-specific skills and broader engineering skills.

A skill entry should explain:

- What the skill does and what it does not do.
- When it is useful.
- Supported tools and compatibility, where known.
- Installation and usage instructions.
- Requirements and dependencies.
- Permissions, file access, network access, and other security-relevant behavior, where known.
- Source repository, publisher, licence, version, and verification information, where available.

#### MCP Servers

Include Model Context Protocol servers and related integrations that connect AI clients to tools or data.

Organize entries by practical function, such as:

- Developer integrations.
- Browser and automation.
- Databases and data sources.
- Utilities and productivity.

An MCP entry should make setup requirements and permission implications understandable. Do not imply that listing or reviewing a server constitutes a security audit.

#### Developer Tools

Include developer-facing tools and services relevant to building software, such as:

- AI coding tools.
- IDEs and extensions.
- Developer utilities.
- APIs and developer services.
- Open-source developer tools.

Entries should help readers understand purpose, platform support, pricing or availability where verified, source, and relevant alternatives.

#### Rules & Configurations

Include instruction files, coding rules, and configuration resources used by developer tools and AI coding environments, including:

- AGENTS.md.
- CLAUDE.md.
- GEMINI.md.
- Cursor rules.
- GitHub Copilot instructions.
- Coding standards and related configuration.

Explain the target tool or environment, placement, precedence or scope when known, and any operational risks.

#### Discover page types

- **Category directory:** browse entries within one category, with relevant filters.
- **Resource detail:** inspect one resource, its provenance, compatibility, instructions, and related knowledge.
- **Editorial collection:** browse a maintainer-curated group of related public entries.

Editorial collections are public editorial groupings. They are not personal notebooks, user-created private collections, or a templates library.

### 3.3 Learn

Learn contains educational material, practical guides, and structured learning tracks. The MVP includes all of the following areas:

- **Start Here:** orientation for people who are new to software development or AI-assisted building.
- **Developer Fundamentals:** programming basics, HTML/CSS/JavaScript, Git and GitHub, command-line use, files and folders, package managers, environment variables, and understanding errors and AI-generated code.
- **AI Engineering:** models, APIs, prompting and context, tool calling, agents, retrieval-augmented generation, embeddings, evaluation, reliability, and related engineering concepts.
- **Secure Development:** secure coding, authentication and authorization, secrets, API and database security, dependency risks, validation, testing, and AI-generated code risks.
- **Software Architecture:** application structure, frontend and backend boundaries, APIs, databases, system design, architecture trade-offs, and technical debt.
- **SEO & Website Growth:** technical and on-page SEO, indexing, sitemaps, robots directives, structured data, performance, Search Console, and content strategy.
- **GEO & AI Search Visibility:** crawlability, clear source attribution, structured and useful content, retrieval and citation concepts, and measurement. Do not promise that a search engine or AI system will recommend or cite a site.
- **UI/UX & Accessibility:** interaction design, responsive layouts, semantic HTML, keyboard access, contrast, forms, assistive technology, and accessibility testing.
- **Testing & QA:** unit, integration, end-to-end, browser and API testing, regression testing, debugging, and validation of AI-generated code.
- **Deployment & Infrastructure:** hosting, domains and DNS, CI/CD, environment configuration, backups, deployment platforms, and operational basics.
- **Legal Awareness:** copyright, software and content licences, attribution, privacy, terms, cookies and consent, and responsible use of third-party material. Content is educational and is not legal advice.

#### Learning page types

- **Guide:** a focused educational article with prerequisites, steps or explanations, examples, sources, and related entries.
- **Learning track:** a curated sequence of guides and resources that helps readers progress through a subject. MVP tracks do not require accounts or persist individual progress.

### 3.4 Contribute

Contribute explains how the community can improve Commonplace and provides both approved contribution routes.

Proposed pages and sections:

- How to contribute.
- Submit through the website.
- Contribute through GitHub (fork, branch, and pull request).
- Contribution guidelines.
- Editorial and review process.
- Code of Conduct.
- Contribution status and feedback guidance.

Both website-based submissions and GitHub pull requests are MVP requirements. They must feed into a shared review and publication process. Published public content remains version-controlled in the GitHub repository.

The website submission implementation must protect credentials and repository permissions. A GitHub write token must never be placed in browser-side code. The secure intake and publishing mechanism remains a technical-architecture decision.

### 3.5 About

About is the fourth primary navigation destination.

Proposed sections:

- **Mission:** what Commonplace is and whom it serves.
- **Principles:** open knowledge, useful curation, transparency, tool and model neutrality, accessibility, and community contribution.
- **How it works:** how resources are collected, checked, reviewed, and published.
- **Governance:** maintainership, editorial responsibilities, and how project decisions are made.
- **Open source:** repository, licence information when decided, and ways to participate.
- **Contact:** appropriate project contact and issue-reporting routes.

Only publish governance, licence, and contact details that have actually been established. Do not imply a formal organization, certification, or review authority that does not exist.

### 3.6 Shared and supporting destinations

The following are shared utilities or supporting pages, not primary navigation destinations:

- Global search and search results.
- Privacy information.
- Terms of use.
- Licence and attribution information.
- Security contact or vulnerability-reporting guidance.
- Not-found page.

The existence, content, and final URLs of legal and policy pages must be confirmed during the relevant governance and launch-planning work. This sitemap does not itself approve legal wording.

## 4. Global search

The MVP provides one global search experience across published **Discover** and **Learn** content.

Search should:

- Accept queries from any primary site area.
- Return clearly labelled result types, such as prompt, skill, MCP server, developer tool, rule/configuration, guide, and learning track.
- Link to the canonical detail page for each result.
- Support basic, relevant filtering by category or content type.
- Present useful empty and no-results states.
- Preserve a usable path to browse categories when a query returns no result.

Search does not require user accounts and does not include personalized recommendations, private saved searches, or AI-generated ranking in the MVP. Search implementation and ranking mechanics are technical decisions for a later stage.

## 5. Shared page and content patterns

The MVP needs a small set of reusable page patterns:

| Page pattern | Purpose |
| --- | --- |
| Homepage | Explain the platform and route visitors into its pillars |
| Directory | Browse and filter a resource category |
| Resource detail | Evaluate and use a Discover entry |
| Guide | Read a focused learning resource |
| Learning track | Follow a curated sequence of learning material |
| Editorial collection | Explore a public, maintainer-curated group of entries |
| Search results | Find published Discover and Learn content |
| Contribution | Submit or propose improvements and understand review |
| About | Understand mission, principles, and governance |
| Supporting policy page | Read applicable project policies and notices |

A shared visual shell may be used across page patterns, but each page must prioritize the information relevant to its task.

## 6. Cross-linking and relationships

Commonplace should connect related knowledge rather than leave entries as isolated records.

Examples:

- A skill can link to the tool or MCP server it uses.
- An MCP server can link to setup and security guides.
- A prompt can link to a relevant skill or learning guide.
- A developer tool can link to fundamentals or architecture material.
- A guide can link to related resources and other guides.
- A learning track can sequence guides and entries.
- An editorial collection can group entries from multiple Discover categories and relevant Learn pages.

Links should be explicit and editorially meaningful. Avoid automatic or misleading relationships based only on shared tags.

## 7. Trust, provenance, and editorial signals

Where relevant and available, entries should expose:

- Original source or canonical URL.
- Publisher or maintainer.
- Source repository.
- Licence and attribution requirements.
- Version or release information.
- Compatibility and supported environments.
- Last-verified date.
- Maintenance information.
- Setup requirements and permissions.
- Security-relevant observations or known limitations.

Use precise review labels. For example, metadata checked, source checked, licence information reviewed, and compatibility checked are distinct claims. A general editorial review must not be presented as a security audit or guarantee.

If a field is unknown, say so or omit it. Do not invent a licence, publisher, maintenance status, or verification date.

## 8. Responsive information architecture

The same content hierarchy must work across:

- Small and large phones, portrait and landscape.
- Foldable phones, including cover and unfolded screens.
- Tablets, portrait and landscape.
- Laptops and desktop displays.

Adapt navigation, density, filters, and columns to available space. Do not simply shrink a desktop layout. On narrow screens, prioritize the current task and make secondary filters or navigation accessible without obscuring content.

Foldable-specific browser capabilities, such as viewport segments or device posture information, may be used as progressive enhancements where supported. Core navigation and content must not depend on them.

## 9. Explicit MVP exclusions

The following are not part of this approved MVP information architecture:

- Personal notebooks or private collections.
- User profiles and account-dependent personalization.
- Personal bookmarks or saved reading lists.
- Persisted learning progress.
- Voting, reputation, or badge systems.
- Forums, social feeds, or a general discussion network.
- Personalized or AI-generated recommendations.
- Interactive execution of third-party code, prompts, skills, or MCP servers.
- A templates library or templates marketplace.

These exclusions do not prevent future proposals, but adding them requires a separate scope decision.

## 10. Decisions reserved for later stages

This document does not select or finalize:

- URL and slug conventions.
- Content schemas and required metadata fields.
- Search engine or indexing implementation.
- Exact filter behavior and taxonomy.
- Editorial collection creation and maintenance workflow.
- Visual design, components, breakpoints, and interaction details.
- Framework, backend, hosting configuration, or deployment architecture.
- Legal policy wording or final policy URLs.
- Website submission infrastructure and status-notification mechanism.

Those decisions belong in the content-system, design, governance, and technical-blueprint stages.

## 11. Approval boundary

This document records the approved MVP information architecture. It authorizes planning and specification work based on this structure. It does not by itself authorize application implementation or settle technical choices reserved for later stages.
