# Platform Language Policy

**Status:** Initial standard  
**Scope:** Commonplace platform development and community educational content  
**Framework:** Not selected  
**Last updated:** 2026-11-20

## 1. Purpose

Commonplace aims to keep platform contributions approachable, maintainable and reviewable. This policy establishes a small, familiar language baseline for the platform without restricting the programming languages represented in educational content.

Language choice alone does not make software secure. Security depends on design, dependency management, validation, permissions, testing and review.

## 2. Core platform languages

The initial platform baseline is:

| Language / format | Intended use | Status |
|---|---|---|
| TypeScript | Main application logic and platform tooling | Core |
| JavaScript | Browser APIs, integrations and ecosystem compatibility | Core |
| HTML | Semantic document structure | Core |
| CSS | Styling, layout, responsive behaviour and themes | Core |
| Markdown | Documentation, guides and knowledge entries | Core |
| JSON | Structured data, metadata and machine-readable configuration | Core |
| YAML | GitHub Actions and supported configuration/frontmatter | Core |

TypeScript is the preferred language for substantial new application logic when it is practical. JavaScript remains welcome where it is the simpler or more compatible choice. HTML, CSS and the content/data formats above are first-class parts of the platform.

This baseline does not select a framework, runtime, build tool or hosting architecture. Those decisions belong in the technical blueprint and require separate review.

## 3. Supporting automation

Python and Bash may be used for focused validation, data processing and repository automation when they provide a clear benefit.

Automation should remain small, understandable and documented. Avoid introducing a language runtime or dependency solely for a task that can be handled safely with existing platform tooling.

## 4. Educational content is language-inclusive

The platform's learning material, examples, explanations and reference content are not restricted to the core platform baseline.

Contributors may create or improve material for languages and technologies including, but not limited to:

- Python, JavaScript and TypeScript
- Java, C, C++ and C#
- Go and Rust
- PHP and Ruby
- Kotlin and Swift
- SQL
- HTML and CSS

New and emerging languages may also be covered when the material is useful and can be reviewed. Content should identify relevant language versions, runtimes, tools and prerequisites where these affect correctness.

## 5. Contribution and quality expectations

Contributions should:

1. Follow the conventions and structure documented for the affected area.
2. Include clear explanations and reproducible examples where appropriate.
3. Avoid unnecessary dependencies and prefer established platform capabilities.
4. Include or update relevant tests and validation when changing executable platform code.
5. Keep documentation accurate, accessible and understandable to the intended audience.
6. Disclose external sources, licences and attribution requirements for reused material.
7. Never include credentials, access tokens, private keys or other secrets.

A contribution written in an approved language is not automatically accepted. All contributions remain subject to the repository's review and security requirements.

## 6. Security requirements

Commonplace will use layered safeguards rather than treating language popularity as a security guarantee.

- Validate structured content and configuration against defined schemas.
- Review and pin automation dependencies where practical; update them through controlled changes.
- Do not execute contributed code merely because it was submitted in a pull request.
- Do not expose write tokens or other secrets in browser-side code, repository content or CI logs.
- Use least-privilege permissions for workflows and integrations.
- Run appropriate automated checks before human review and publication.
- Require human approval for sensitive workflow, permission, dependency or infrastructure changes.
- Treat third-party prompts, skills, MCP server instructions, scripts and configuration as untrusted until reviewed.
- Document the checks performed without implying that a routine content review is a security audit.

The exact CI checks and approval rules will be defined in the technical blueprint and repository governance. This policy does not claim that all safeguards are already implemented.

## 7. Exceptions and future changes

A contribution may use another language when there is a clear technical or educational reason. Platform-level additions to the core baseline should be proposed with their maintenance cost, contributor impact, security implications and deployment requirements.

This is an initial standard. It may evolve as the project grows, but changes should be documented and reviewed rather than introduced implicitly.
