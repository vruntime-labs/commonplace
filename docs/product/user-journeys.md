# User Journeys

**Version:** 0.1  
**Status:** Approved  
**Stage:** 2 — Information Architecture  
**Scope:** Commonplace MVP

## 1. Purpose

This document describes the primary tasks people should be able to complete in the Commonplace MVP. It connects the approved product scope and information architecture to observable user needs and success criteria.

Commonplace serves people with different levels of experience. Public discovery and learning must be useful without requiring an account.

## 2. User groups

These are practical audience descriptions, not account types or rigid personas.

- **Beginners:** people learning programming, developer tools, or how to build with AI assistance.
- **AI-assisted developers:** people using coding agents, prompts, skills, MCP servers, and related tools in real projects.
- **Experienced developers:** people evaluating integrations, configurations, engineering practices, and technical trade-offs.
- **Learners and educators:** people looking for structured explanations, references, and learning sequences.
- **Contributors:** people sharing new resources, correcting existing entries, or improving guides.
- **Maintainers and reviewers:** people checking submissions, maintaining quality, and publishing accepted contributions.

The MVP does not require separate profiles or permission tiers for these groups. Any permissions needed for contribution review are an implementation and governance matter.

## 3. Discovery journeys

### Journey 1 — A beginner discovers a developer tool

**User need:** Understand what a tool is, whether it is relevant, and how to get started without being overwhelmed.

**Path:**
1. Arrive at the homepage.
2. Choose Discover or use global search.
3. Browse Developer Tools or search for a known tool or task.
4. Open a result.
5. Read the purpose, intended audience, requirements, platform support, source, and availability information.
6. Follow the official source or a relevant Commonplace guide to continue.

**Success criteria:**
- The user can understand the tool's purpose and intended use.
- Important requirements and unknowns are visible.
- The user can reach a trustworthy source or next learning step.
- No account is required to read the entry.

### Journey 2 — An experienced developer evaluates an MCP server

**User need:** Decide whether an MCP server is relevant and understand the implications of connecting it to an AI client.

**Path:**
1. Open Discover → MCP Servers or use global search.
2. Filter or browse by function.
3. Open the server detail page.
4. Inspect its publisher, canonical repository, licence, maintenance and version information where available.
5. Review supported clients, setup requirements, permissions, file or data access, network behavior, and destructive capabilities where documented.
6. Read relevant setup or security guidance.
7. Visit the canonical source to inspect the project and decide whether to install it independently.

**Success criteria:**
- Provenance and known compatibility are easy to locate.
- Permission and security-relevant information is not hidden behind promotional copy.
- Unknown or unverified details are clearly identified.
- The page does not imply that Commonplace has audited or certified the server.
- Commonplace does not execute or install the server on the user's behalf.

### Journey 3 — A developer finds and uses an AI coding skill

**User need:** Find a skill that fits a task and install or use it in the intended environment.

**Path:**
1. Open Discover → Skills or search by task, tool, or skill name.
2. Open a relevant skill entry.
3. Understand what the skill does, its limits, and when it is useful.
4. Check supported tools, versions, requirements, permissions, and source.
5. Follow the documented installation instructions.
6. Consult linked guides or alternatives if needed.

**Success criteria:**
- The intended task and supported environment are clear.
- Installation instructions identify the correct source and destination.
- Risks, permissions, and dependencies are disclosed where known.
- The user is not encouraged to run untrusted instructions without review.

### Journey 4 — A beginner learns to build a website more securely with AI

**User need:** Learn a practical process for using AI assistance without blindly trusting generated code.

**Path:**
1. Open Learn → Start Here or Secure Development.
2. Read an introductory guide that explains the build-and-review process.
3. Follow links to relevant fundamentals, such as HTML, JavaScript, APIs, authentication, and environment variables.
4. Work through security topics such as input validation, access control, secrets, dependency review, and testing.
5. Use a relevant checklist or reference where available.
6. Return to the guide's sources and further reading.

**Success criteria:**
- The guide is understandable to its stated audience.
- Prerequisites and unfamiliar terms are explained or linked.
- Practical safeguards and verification steps are included.
- The material distinguishes general education from project-specific security review.
- The guide does not promise that AI-generated code is safe.

### Journey 5 — A website owner learns about SEO and AI search visibility

**User need:** Improve discoverability while understanding what can and cannot be controlled.

**Path:**
1. Open Learn → SEO & Website Growth or GEO & AI Search Visibility.
2. Choose an introductory guide or relevant learning track.
3. Learn the fundamentals: crawlability, indexing, content quality, metadata, structured data, performance, and clear source attribution.
4. Follow practical steps and official references.
5. Review measurement guidance and understand the limits of attribution.
6. Apply changes independently and monitor results.

**Success criteria:**
- SEO and AI search visibility are explained without conflating them.
- Advice distinguishes controllable technical improvements from external ranking or citation decisions.
- No guide promises placement, ranking, recommendation, or citation by a search engine or AI system.
- Recommendations link to relevant primary documentation where practical.

### Journey 6 — A learner follows a learning track

**User need:** Move through a subject in a useful order without having to assemble every resource independently.

**Path:**
1. Open Learn or global search.
2. Choose a learning track relevant to a goal.
3. Review its intended audience, prerequisites, outcomes, and sequence.
4. Open each guide or linked resource.
5. Use related links to explore a topic further.
6. Return to the track as needed.

**Success criteria:**
- The sequence and learning outcomes are clear.
- Prerequisites are stated.
- Each step links to published material.
- The track remains usable without an account.
- The MVP does not claim to save personal progress or completion state.

## 4. Contribution journeys

Both contribution routes are required in the MVP and must lead to the same editorial review and publication process.

### Journey 7 — A contributor submits through GitHub

**User need:** Add or improve content using a familiar open-source workflow.

**Path:**
1. Open Contribute and read the contribution guidelines.
2. Choose the relevant content type and inspect the existing structure and examples.
3. Fork the repository or create an appropriate working branch.
4. Add or update the content and its required metadata.
5. Run the documented validation checks.
6. Open a pull request with a clear summary, sources, attribution, and licence information.
7. Respond to maintainer feedback or requested changes.
8. Follow the pull request until it is merged or closed.

**Success criteria:**
- Guidelines explain the expected structure and quality bar.
- Contributors can identify where and how to add material.
- Automated checks provide actionable feedback.
- Reviewers can trace sources, attribution, and changes.
- The contributor can understand the final review outcome.

### Journey 8 — A contributor submits through the website

**User need:** Propose a resource or improvement without first learning Git or the repository workflow.

**Path:**
1. Open Contribute → Submit through the website.
2. Choose the type of contribution.
3. Complete a guided submission with the relevant title, description, canonical source, attribution, licence information, and category details.
4. Review the submission and send it.
5. Receive a confirmation or reference that allows the contributor to identify the submission.
6. Follow the published status and any requested changes using the available mechanism.
7. Provide corrections or additional information when requested.
8. Receive a final decision or publication reference.

**Success criteria:**
- The form explains what information is needed and why.
- Validation catches missing or malformed fields before submission.
- The contributor receives a meaningful confirmation and reference.
- Status and feedback are understandable.
- Website submissions enter the same review process as pull requests.
- Accepted content is committed to the GitHub repository as the source of truth.

**Security and implementation constraints:**
- Never expose a GitHub write token or other privileged credential in browser-side code.
- Validate and sanitize submitted content on a trusted server-side boundary or through another approved safe intake design.
- Rate-limit and protect the intake against spam and abuse.
- Do not execute submitted code, scripts, prompts, skills, or server packages.
- The exact intake service, storage, notification, and publishing mechanism remains undecided until technical architecture.

### Journey 9 — A contributor corrects an existing entry

**User need:** Report outdated, inaccurate, broken, or incomplete information.

**Path:**
1. Open the relevant resource or guide.
2. Find the correction or contribution route.
3. Identify the affected content and explain the issue.
4. Provide evidence or a corrected source where possible.
5. Submit through GitHub or the website route.
6. Follow review feedback and the final outcome.

**Success criteria:**
- The correction route is discoverable from contribution guidance and relevant content pages.
- Reports can identify the affected entry precisely.
- Reviewers can evaluate the evidence and preserve attribution.
- Accepted corrections update the canonical published content.

## 5. Editorial and maintainer journeys

### Journey 10 — A maintainer reviews a contribution

**User need:** Evaluate a proposal consistently, safely, and transparently.

**Path:**
1. Receive a pull request or website submission.
2. Confirm the submission is complete enough to review.
3. Check relevance, usefulness, clarity, and accuracy.
4. Check canonical sources, attribution, and licence compatibility.
5. Review security-relevant content and instructions, including commands, permissions, external links, and potentially harmful behavior.
6. Run the appropriate automated validation.
7. Decide to request changes, approve, or reject with a reason.
8. For accepted material, commit the approved content to the repository and publish through the normal release process.
9. Ensure the contributor can identify the outcome.

**Success criteria:**
- Both contribution routes use consistent editorial criteria.
- Review decisions are traceable.
- Automated checks support, but do not replace, human review.
- Licence and attribution questions are not silently ignored.
- Editorial review is not represented as a guarantee of safety or a comprehensive security audit.
- Rejected or deferred submissions receive a clear explanation where practical.

### Journey 11 — A returning visitor finds updated knowledge

**User need:** Locate a known resource and understand whether its information has changed.

**Path:**
1. Return to a category, collection, guide, or global search.
2. Search for the known title, task, or topic.
3. Open the canonical entry.
4. Inspect its version, source, and last-verified or updated information where available.
5. Follow links to related guides or alternatives.

**Success criteria:**
- Canonical URLs remain stable where practical.
- Updated information is distinguishable from stale information.
- Source and verification dates are displayed only when maintained.
- Related content helps the visitor continue without relying on personalization.

## 6. Shared experience requirements

Across all journeys:

- Public Discover and Learn content can be read without an account.
- Core content remains understandable and usable when client-side JavaScript is unavailable.
- Navigation and essential tasks work with keyboard and touch input.
- Layouts adapt to phones, foldables, tablets, laptops, and desktop screens.
- Accessibility is considered throughout content structure and interaction design.
- Source, licence, attribution, compatibility, and verification information is shown when relevant and known.
- Unknown details are not fabricated.
- Third-party code and instructions are not automatically executed.
- Privileged credentials and contributor data are protected.
- Review labels describe the checks actually performed.
- Search and related links help users move between Discover and Learn.

## 7. Contribution status model

The shared contribution process uses these conceptual statuses:

1. **Submitted** — received and awaiting review.
2. **Reviewing** — a maintainer is evaluating the contribution.
3. **Changes requested** — additional information or revisions are needed.
4. **Approved** — accepted for publication.
5. **Published** — merged into the canonical content source and made available on the site.
6. **Rejected** — not accepted, with a reason where practical.

The user-facing wording and technical state machine may be refined during implementation planning. A submission must not be labelled Published merely because it was received or approved.

## 8. Explicitly deferred journeys and features

The MVP does not include user journeys that depend on:

- User profiles or account-based personalization.
- Personal bookmarks, notebooks, or private collections.
- Saved learning progress.
- Voting, reputation, or badges.
- Forums, social feeds, or general social networking.
- Personalized or AI-generated recommendations.
- Interactive execution of third-party code, prompts, skills, or MCP servers.
- A templates library or templates marketplace.

These features require separate scope approval before they are added.

## 9. Open implementation questions

The journeys establish expected outcomes, not implementation choices. The following remain open for later stages:

- Whether website submissions use a server-side endpoint, GitHub-backed issue intake, or another secure mechanism.
- How submission references, status updates, and contributor notifications are delivered.
- How automated content validation is organized.
- Which checks are required for each content type.
- How reviewers handle licence uncertainty, security concerns, and takedown requests.
- Which analytics, if any, are appropriate and privacy-respecting.
- How search ranking and filters are implemented.
- How accessibility and responsive behavior are tested across devices.

## 10. Approval boundary

This document records the approved MVP user journeys and their success criteria. It is a product and experience specification, not a technical implementation plan. It does not authorize execution of third-party content or select a backend, framework, database, hosting configuration, or submission service.
