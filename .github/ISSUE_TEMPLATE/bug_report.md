---
name: Bug report
about: Report a problem with CrudGenerator
title: ''
labels: bug
assignees: ''
---

## Summary

A short description of what went wrong.

<!--
Thank you for taking the time to file a bug report.

Pull requests are not accepted on this repository — the source code is
private. To get a fix, please describe the problem clearly so it can be
reproduced and fixed in the next release.
-->

## Environment

- **CrudGenerator version**: (visible in *Settings → Plugins → CrudGenerator*, or on the JetBrains Marketplace page)
- **IntelliJ IDEA version**:
- **Operating system**:
- **Java runtime version** (`java -version`):
- **Build tool of the target project** (Maven / Gradle Groovy DSL / Gradle Kotlin DSL):
- **Spring Boot version of the target project** (3.x / 4.x, with the exact patch version when possible):
- **Package structure** (DDD / Layered):
- **Naming profile** (Italian / English):

## Steps to reproduce

1.
2.
3.

## Expected behaviour

What you expected to happen.

## Actual behaviour

What actually happened. Include:

- The exact wording of any IDE error notification, dialog or completion balloon.
- Stack traces and relevant log excerpts (Help → *Show Log in Files / Explorer*).
- Whether generation produced files, refused to start, or aborted partway through.

## Generated artifacts affected

Which generated artifacts are affected (DTOs, support, exceptions, mapper, repository, application services, events, REST controller, tests, ...). A short example of the unexpected output is often more useful than a long description.

## Target project context

Anything relevant about the project CrudGenerator was run on:

- Other JetBrains plugins active in the same IDE session (MCP Server, HATEOAS helpers, Security helpers).
- Large entity graphs, custom field types, nullable embeddables.
- Build-file edits performed by CrudGenerator in earlier runs.

## Screenshot

If applicable, add a screenshot to help explain the problem.
