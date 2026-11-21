# Commonplace Contribution Guidelines

**Status:** Approved v0.1  
**Audience:** Anyone contributing resources, learning content, corrections, or project improvements

Thank you for helping make useful developer knowledge easier to discover, understand, and share. You do not need to be an experienced developer to contribute. Clear corrections, useful sources, careful reviews, and beginner-friendly explanations all matter.

For repository-wide contribution and pull request instructions, also see the root [CONTRIBUTING.md](../../CONTRIBUTING.md). All contributors must follow the [Code of Conduct](../../CODE_OF_CONDUCT.md).

## 1. What you can contribute

### Discover

The MVP accepts entries in these five categories:

- Prompts
- Skills
- MCP Servers
- Developer Tools
- Rules & Configurations

A useful resource submission explains what the item is, what problem it addresses, who may benefit, where its canonical source is, and what a reader should know before using it.

### Learn

You may contribute or improve:

- Start Here material.
- Developer Fundamentals.
- AI Engineering and AI-assisted Development.
- Secure Development.
- Software Architecture.
- SEO & Website Growth.
- GEO & AI Search Visibility.
- UI/UX & Accessibility.
- Testing & QA.
- Deployment & Infrastructure.
- Legal Awareness.
- Practical guides, tutorials, articles, explainers, references, checklists, and learning tracks.

Commonplace also publishes original technical material written and maintained by its editorial team. Community contributions and Commonplace editorial content are distinct origins; both are subject to review and clear attribution.

### Other useful contributions

You can report factual errors, broken links, outdated instructions, accessibility problems, missing attribution, licence concerns, or potentially unsafe content. You can also improve documentation, tests, accessibility, and project tooling.

## 2. Ways to contribute

There are two intended contribution routes. Both feed into the same review and publication process.

### A. GitHub pull request

The GitHub route is available now:

1. Check existing issues and pull requests to avoid duplicate work.
2. For substantial or uncertain changes, open an issue or discuss the proposal with maintainers first.
3. Fork the repository and create a focused branch.
4. Make the change and check formatting, links, accuracy, attribution, and relevant validation.
5. Open a pull request against `main`.
6. Explain what changed, why it is useful, and what you checked.
7. Respond to review feedback and update the pull request as needed.

Keep pull requests focused. Do not bundle unrelated changes or remove existing work without a clear reason.

### B. Guided website submission

A guided website-based submission route is an approved MVP requirement, but it is not available yet. Until it launches, use GitHub issues for suggestions and pull requests for proposed changes.

When implemented, the website route must use a secure server-side or otherwise safe GitHub-backed intake process. It must not expose a privileged GitHub write token or other secrets in browser code. Website submissions will enter the same review pipeline as GitHub contributions; submitting through the website will not mean automatic publication.

## 3. What makes a strong resource entry

Where relevant, include:

- Resource name and concise purpose.
- Canonical website or source repository.
- Publisher, author, and maintainer, if known.
- Intended audience and useful use cases.
- Installation, setup, or usage documentation.
- Supported versions, platforms, and compatibility.
- Licence or reuse terms, or an explicit note that they are unknown.
- Maintenance signals and the date you checked them.
- Required permissions, data access, network access, and security considerations.
- Known limitations, risks, and relevant alternatives.

Prefer official sources. Do not claim that a resource is official, secure, maintained, verified, or endorsed unless you can support the statement and explain what was checked.

## 4. What makes strong learning content

A guide, tutorial, article, or reference should make its purpose and intended audience clear. Include prerequisites, steps or reasoning, examples, expected outcomes, limitations, and reliable sources where relevant.

For code and command examples:

- State relevant language, tool, runtime, platform, and version assumptions.
- Prefer safe defaults.
- Explain destructive or security-sensitive actions before the reader performs them.
- Include expected results and troubleshooting guidance when useful.
- Say whether examples were tested; never invent test results.
- Do not include real credentials, access tokens, private data, or secrets.

Write in your own words. Cite source material for claims and ideas. Do not copy third-party documentation or articles without permission and appropriate licensing.

## 5. Attribution, permissions, and licensing

Only submit work you created or are authorised to contribute. Identify third-party content, authors, sources, and applicable licences. A publicly accessible page or repository is not automatically free to copy, modify, or republish.

The project's source-code licence, editorial-content licence, and contributor terms have not yet been finalised. Do not assume that submitting content grants a particular licence or transfers ownership. Maintainers must communicate the applicable terms before accepting contributions that depend on them.

## 6. Safety, privacy, and security

Never include passwords, API keys, access tokens, private user data, or other secrets in issues, pull requests, commits, screenshots, examples, or documentation.

Do not submit malicious code, harmful instructions, or content intended to compromise users or systems. Do not submit executable payloads disguised as resources. Commonplace does not execute contributed prompts, skills, scripts, MCP servers, or other code as part of editorial review.

For legitimate security education, clearly state authorisation assumptions and safe test environments. Report suspected vulnerabilities privately using the process in [SECURITY.md](../../SECURITY.md), not in a public issue with exploitable details.

## 7. Review process

Both contribution routes use one shared process:

1. **Submitted** — the contribution has entered the intake process.
2. **Reviewing** — maintainers are evaluating it.
3. **Changes requested** — clarification, corrections, sources, or revisions are needed.
4. **Approved** — the contribution has been accepted for publication.
5. **Published** — the contribution is publicly available.
6. **Rejected** — the contribution will not be published, with an explanation where practical.

These are workflow statuses, not quality badges. A contribution may be edited for clarity, accessibility, structure, consistency, or accuracy while preserving the contributor's meaning and credit.

Review may consider relevance, accuracy, sources, attribution, licence, safety, accessibility, metadata, compatibility, and maintainability. Not every item receives a formal security review. Editorial review is not a guarantee of correctness, legal compliance, or security.

Submitting a contribution does not guarantee acceptance or publication. Maintainers may ask for changes, defer work, or decline material that does not fit the project's scope or standards.

## 8. Feedback and corrections

Be constructive and specific when reviewing another contribution. Explain the issue, provide evidence or a source where possible, and suggest a path to improvement.

If you find an error in published content, report the affected page or file, describe what is wrong, and include reliable supporting information. For urgent safety or security concerns, use the appropriate private reporting channel.

## 9. Contributor checklist

Before submitting, check that:

- [ ] The contribution has a clear purpose and fits the approved project scope.
- [ ] Existing content and issues have been checked for duplication.
- [ ] Claims are accurate and supported by relevant sources.
- [ ] Authors, sources, and third-party material are attributed.
- [ ] Licence and permission information is accurate or explicitly unknown.
- [ ] Prerequisites, compatibility, limitations, and risks are stated where relevant.
- [ ] Examples are safe and their test status is honest.
- [ ] No secrets or private data are included.
- [ ] Links, formatting, and relevant validation have been checked.
- [ ] The pull request or proposal explains what changed and why.

## 10. Maintainer responsibilities

Maintainers should review contributions consistently and respectfully, explain requested changes or rejection where practical, preserve attribution, and avoid implying checks that were not performed. They are responsible for applying the editorial policy, maintaining transparent status, and routing security reports appropriately.

The review process should be fair to new contributors and should not favour volume over usefulness. Editorial and community contributions should meet the same standards for accuracy, clarity, safety, and source quality while retaining clear provenance.

## 11. Related documents

- [Repository contribution instructions](../../CONTRIBUTING.md)
- [Content model](../content/content-model.md)
- [Editorial policy](editorial-policy.md)
- [Code of Conduct](../../CODE_OF_CONDUCT.md)
- [Security policy](../../SECURITY.md)
