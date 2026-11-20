# Commonplace — Product Strategy

**Document:** `product-strategy.md`  
**Version:** 0.2  
**Status:** Product direction and MVP scope approved; detailed design and implementation decisions remain open  
**Project:** Commonplace  
**Organisation:** VRuntime Labs

---

## 1. Product overview

**Commonplace is an open knowledge platform for people who build with technology.**

It brings together useful developer resources, practical learning, and community contributions in one carefully organised place.

Inspired by the historical commonplace book, the platform aims to make scattered knowledge easier to discover, understand, evaluate, maintain, and share.

**Tagline:** Knowledge worth keeping.

**Product description:** An open knowledge platform for people who build with technology.

## 2. Vision

Create a shared, continuously improving knowledge space where anyone can discover useful resources, develop technical understanding, and contribute knowledge that helps others build better software.

## 3. Mission

- Make valuable technical knowledge easier to find.
- Help beginners understand concepts without excluding experienced developers.
- Make AI-assisted development more understandable, reliable, and secure.
- Connect resources with the knowledge needed to use them effectively.
- Encourage open contribution and responsible knowledge sharing.
- Preserve useful knowledge through attribution, verification, and maintenance.

## 4. The problem

People building software face an increasingly fragmented knowledge landscape.

- Resources are scattered across repositories, websites, documentation, communities, and directories.
- Finding a resource does not necessarily explain whether it is trustworthy, maintained, compatible, or safe.
- Beginners often encounter advanced material without enough context.
- Experienced developers spend time searching across disconnected sources.
- AI-generated code and workflows can introduce security, quality, licensing, and maintenance problems.
- Useful community knowledge can become outdated, difficult to discover, or lost.

Commonplace aims to address these problems through organised discovery, practical education, and community contribution.

## 5. Target audiences

### Beginners and aspiring developers

People learning programming, Git, development tools, and software fundamentals.

**Needs:** Clear explanations, guided learning, practical examples, and trustworthy starting points.

### AI-assisted developers

People using AI coding assistants, agents, prompts, skills, and MCP servers to build software.

**Needs:** Tool compatibility, installation guidance, practical workflows, security awareness, and ways to evaluate AI-generated work.

### Experienced developers

People who need technical references, architecture guidance, engineering practices, and specialised tools.

**Needs:** Accurate technical depth, useful filters, maintained resources, and efficient discovery.

### Open-source contributors and maintainers

People publishing tools, documentation, guides, and community knowledge.

**Needs:** A clear contribution process, attribution, version history, and transparent editorial review.

### Educators and technical writers

People helping others understand and apply technical knowledge.

**Needs:** A place to share structured educational material and connect learning with practical resources.

## 6. Product pillars

All three pillars are central to Commonplace.

### A. Discover

Help people find useful resources for building software and working with technology.

Potential resource categories:

- Prompts and system instructions.
- Skills and agent capabilities.
- MCP servers and integrations.
- AI models and AI coding tools.
- IDE extensions and developer tools.
- Rules and configurations.
- Workflows and agents.
- APIs and developer services.
- UI components and component libraries.
- Open-source projects and technical resources.

Each resource should provide useful context rather than just a name and link.

Where relevant, resource entries should explain purpose, source, licence, compatibility, installation, usage, maintenance, and limitations.

### B. Learn

Help people understand the knowledge behind good software development.

Potential learning areas:

- Programming and web development fundamentals.
- Git, GitHub, and developer tooling.
- AI engineering and AI-assisted development.
- Software architecture and system design.
- Databases, APIs, and backend development.
- Security and secure coding.
- Testing, debugging, and quality assurance.
- UI/UX and accessibility.
- SEO and website growth.
- AI search visibility and GEO.
- Deployment and infrastructure.
- Performance and monitoring.
- Software licensing, privacy, and legal awareness.

Learning content should support both introductory and advanced understanding.

### C. Contribute

Make it possible for people to improve the shared knowledge base.

Two contribution paths are intended:

1. **GitHub-first:** Fork, edit, and submit a pull request.
2. **Website-based:** Submit or suggest knowledge through a guided contribution experience.

Both paths should enter a shared review and validation process.

GitHub is the proposed source of truth for published public content.

## 7. Core product capabilities

| Capability | MVP commitment |
|---|---|
| Resource discovery | Browse the initial Discover categories listed in Section 10 |
| Search | Static, cross-category search with useful basic filters |
| Resource detail pages | Explain purpose, source, licence, compatibility, installation or usage, maintenance, and known limitations where relevant |
| Learning guides | Publish practical, beginner-accessible guides with technical depth where needed |
| Learning paths | Provide a small number of curated sequences that connect related guides and resources |
| Editorial collections | Group related public knowledge into curated collections; these are not downloadable templates or user-personalised notebooks |
| Trust information | Show source, attribution, licence, review state, and maintenance information without overstating verification |
| Contributions | Support both GitHub pull requests and a guided website submission path |
| Editorial review | Validate submissions and use human review before publication |
| Responsive interface | Support phones, foldables, tablets, laptops, and desktops |

The MVP boundary and exclusions are defined in Section 10. These commitments describe product outcomes, not a decision to use a particular framework, database, hosting runtime, or submission implementation.

## 8. Trust and editorial principles

Commonplace should be curated, not merely aggregated.

Content quality should consider:

- **Source:** Where did the information originate?
- **Attribution:** Who created or maintains it?
- **Licence:** Under what terms can it be used or shared?
- **Relevance:** Is it useful to the intended audience?
- **Accuracy:** Is the information supported and technically sound?
- **Maintenance:** Is it current, abandoned, or known to have changed?
- **Compatibility:** Which tools, versions, or environments does it support?
- **Security:** Are there relevant permissions, risks, or warnings?

Editorial checks must be described accurately. A source or metadata check must never be presented as a security audit.

Guides about legal, security, and compliance topics should explain their scope and limitations. Educational material is not a substitute for professional legal or security advice.

## 9. Product principles

1. **Open knowledge:** Useful knowledge should be accessible and shareable.
2. **Curated, not merely aggregated:** Quality and context matter more than quantity.
3. **Tool agnostic:** No single vendor, model, IDE, or framework defines the platform.
4. **Beginners welcome, experts equipped:** Accessibility should not come at the cost of technical depth.
5. **Honest by design:** Be transparent about sources, limitations, verification, and uncertainty.
6. **Community driven:** Knowledge improves through responsible contribution.
7. **Accessible and responsive:** The platform should work across devices and accommodate different needs.
8. **Maintainable:** Content and software should be structured for long-term improvement.

## 10. Approved MVP scope

**Status: Approved by the project owner on 20 November 2026.**

The first release must deliver a useful, dependable knowledge experience across all three pillars: Discover, Learn, and Contribute. None of the three pillars is treated as an optional add-on.

### 10.1 Discover — MVP

Launch with focused, curated directories for:

- Prompt Library.
- Skills Library.
- MCP Server Directory.
- Developer Tools and AI Coding Tools.
- Rules and Configurations.

Each resource entry should include the relevant details needed to evaluate and use it: purpose, original source, attribution, licence or licence status, supported tools and versions where known, installation or usage guidance, maintenance information, and known limitations or safety considerations. Do not invent missing metadata; show when information is unknown or not yet checked.

Provide cross-category search and basic category/topic filters. Prioritise reliable discovery over advanced personalisation or complex search infrastructure.

### 10.2 Learn — MVP

Publish practical guides and curated learning tracks covering:

- Developer Fundamentals.
- AI Engineering and AI-assisted development.
- Secure Development and secure coding.
- Software Architecture and engineering practices.
- SEO and Website Growth.
- GEO and AI Search Visibility.
- UI/UX Standards and Accessibility.
- Testing, debugging, and quality assurance.
- Deployment and Infrastructure.
- Legal, licensing, privacy, and compliance awareness.

Content should offer beginner-friendly entry points without excluding advanced material. Guides should link to relevant resources and to other guides. Legal and security material must clearly state its scope and must not present itself as professional advice or a certification.

### 10.3 Contribute — MVP

Both contribution paths are part of the approved MVP:

1. **GitHub-first:** Contributors can fork the repository, make a change, and submit a pull request.
2. **Website-based:** Contributors can submit a resource or knowledge suggestion through a guided website experience.

Both paths must feed a shared validation, moderation, and human editorial review process. Approved public content is committed to GitHub, which remains the source of truth for published content. Contributors should receive clear submission guidance, feedback or status information appropriate to the chosen path, and attribution for accepted work.

The website submission path must not expose a GitHub write token or other privileged credential in browser code. Its implementation must use a safe server-side integration or a safe GitHub-backed intake mechanism. This is a product and security requirement, not a selection of a particular backend or hosting service.

### 10.4 MVP experience and quality requirements

- Public reading and basic discovery are free and do not require an account.
- The interface adapts to phones, foldable devices, tablets, laptops, and desktops; it is not merely a scaled desktop layout.
- Core reading and navigation remain usable with keyboard access and assistive technologies.
- Public content should remain readable when client-side JavaScript is unavailable; search enhancement must not make the knowledge itself inaccessible.
- Resource sources, attribution, licence status, review state, and maintenance information are presented honestly.
- Contributions are validated and reviewed; contributed code, skills, prompts, MCP servers, and shell instructions are treated as untrusted and are never automatically executed by the platform.
- The platform remains open-source, free-first, and tool- and model-agnostic.
- Launch with a focused set of useful, reviewed entries and guides rather than maximising the number of listings.

### 10.5 Explicitly out of scope for the MVP

The following are deferred until a later phase demonstrates a clear need:

- User accounts, public profiles, and sign-in-dependent features.
- Personal bookmarks, private notebooks, and personalised collections.
- Voting, reputation scores, badges, and gamified contribution systems.
- Forums, social feeds, direct messaging, and broad discussion features.
- Personalised or AI-generated recommendations and matching.
- Interactive code execution, hosted playgrounds, or execution of third-party skills/MCP servers.
- Complex real-time collaboration and advanced workflow automation.
- Advanced compatibility checkers and automated security certification.

Curated editorial collections of public content are allowed in the MVP; personal collections are not. This is not a templates library or a paid-product marketplace.

### 10.6 MVP success principle

The first release is successful when people can find a useful resource, understand how and whether to use it, learn the relevant concepts, and contribute improvements through either approved path. Quality, clarity, safety, and maintainability take priority over feature count.

## 11. Later phases

Potential capabilities to evaluate after the MVP, based on demonstrated user needs:

- User accounts and profiles.
- Personal bookmarks, private notebooks, and reading lists.
- Learning progress and personalisation.
- Community discussions and project showcases.
- Contributor recognition, voting, or reputation features.
- Advanced search and personalised discovery.
- Resource compatibility tools and richer verification workflows.
- Version comparison, change notifications, and additional collaboration features.
- Interactive learning experiences, only with an appropriate safety model.

These are future possibilities, not commitments. The MVP exclusions in Section 10 remain deferred unless explicitly reconsidered and approved.

## 12. Differentiation

Commonplace should distinguish itself through the combination of:

- Discovery connected to practical learning.
- Technical resources with context and evaluation information.
- Beginner-friendly explanations alongside expert-level material.
- Tool- and model-agnostic coverage.
- Responsible curation, attribution, and maintenance.
- Open contribution through both GitHub and a guided website pathway.
- Knowledge organised for long-term usefulness rather than short-lived engagement.

The goal is not to become another link directory. It is to make discovered knowledge genuinely useful.

## 13. Success measures

Success should be measured through meaningful outcomes rather than vanity metrics.

Potential measures:

**Discovery**
- Search success and resource engagement.
- Visitors reaching relevant resource detail pages.
- Search queries that return useful results.

**Learning**
- Guide completion and return visits.
- Navigation between guides and related resources.
- Feedback on clarity and usefulness.

**Contribution**
- Valid submissions and merged pull requests.
- Contributor retention.
- Time from submission to review.
- Quality and maintenance of published contributions.

**Trust**
- Percentage of entries with source and licence information.
- Percentage of time-sensitive entries reviewed within their defined review interval.
- Reports of outdated or incorrect content and resolution time.

**Quality**
- Accessibility conformance.
- Mobile and responsive usability.
- Core Web Vitals.
- Reliability and build health.

Baseline targets should be established after the initial release, using real usage data.

## 14. Non-goals

Commonplace is not intended to be:

- A downloadable templates library.
- A generic link aggregator.
- A marketplace for paid developer products.
- A social-media feed or engagement-first network.
- A certification or accreditation authority.
- A platform tied to one AI provider or coding tool.
- An execution environment for arbitrary third-party code, skills, or MCP servers.
- A replacement for official documentation or professional advice.
- A platform that claims to guarantee search rankings or AI-generated recommendations.

## 15. Constraints and operating principles

The project should follow a free-first and open-source approach.

- Prefer free hosting and infrastructure while practical.
- Avoid unnecessary recurring costs.
- Keep the public knowledge experience fast and accessible.
- Do not introduce accounts or backend services before their value is established.
- Never expose privileged credentials in browser code.
- Treat third-party resources and executable instructions as untrusted until reviewed.
- Preserve content attribution and licensing requirements.
- Make architectural choices based on actual product needs.

## 16. Decisions reserved for later planning stages

The following are not settled by approval of the product direction and MVP scope. They must be researched, documented, and approved in their relevant planning stages before implementation:

- Final sitemap, navigation, page hierarchy, and user journeys.
- Initial launch content volume, editorial priorities, and exact guide sequence.
- Detailed content schemas, metadata requirements, and review intervals.
- Website submission mechanics and secure server-side or GitHub-backed intake design.
- Final editorial verification levels and moderation procedures.
- Framework, build tooling, search implementation, hosting configuration, and any backend/database choices.
- Detailed responsive breakpoints, design tokens, typography, and visual identity implementation.
- Accessibility acceptance criteria and testing approach.
- Initial language support and localisation scope.
- Licensing model for platform code and original editorial content.
- Deployment, privacy, analytics, and operational procedures.

Approval of this document does not authorise coding or silently select any of these technical decisions. They remain subject to the project's planning and approval workflow.

## 17. Guiding statement

**Commonplace exists to help people discover useful knowledge, understand it, build with it, and keep it available for others.**

*Knowledge worth keeping. Kept in common.*
