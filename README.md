# CrudGenerator

> Generate a complete Spring Boot CRUD layer from a single JPA entity — right-click, pick an action, get a production-ready module in seconds.

[![JetBrains Plugin](https://img.shields.io/jetbrains/plugin/v/io.laborinto.crudgenerator.svg)](https://plugins.jetbrains.com/plugin/io.laborinto.crudgenerator)
[![License: Proprietary Freeware](https://img.shields.io/badge/license-Proprietary%20Freeware-lightgrey.svg)](EULA.md)

CrudGenerator is a free IntelliJ IDEA plugin published on the JetBrains Marketplace. From a single `@Entity` class it writes a complete, clean-architecture CRUD layer — DTOs, MapStruct mappers, Spring Data repositories, application services, REST controllers, domain events and tests — targeting Spring Boot 3 and Spring Boot 4 projects.

The plugin source code is **not public** and is **not open to external contributions**. This repository exists for two purposes only:

- **Issue tracking** — bug reports and feature requests.
- **Security reports** — coordinated disclosure of vulnerabilities.

---

## Installation

Install from the JetBrains Marketplace:

1. Open IntelliJ IDEA (`2026.1` or later).
2. Go to **Settings → Plugins → Marketplace**.
3. Search for **CrudGenerator**, click **Install**, then restart the IDE.

Plugin page: <https://plugins.jetbrains.com/plugin/io.laborinto.crudgenerator>

---

## See it before you install

The [CrudGenerator example projects](https://github.com/giuseppe-trisciuoglio/jetbrains-crud-generator-plugin-examples) repository contains four ready-to-run Maven Spring Boot applications that cover the configuration matrix:

- **Package structure:** DDD and Layered
- **Spring Boot:** 3.x and 4.x

Each example starts with a single `Project` entity and nothing else. Running the generation action on it writes the entire CRUD layer shown in the example — exactly as CrudGenerator would write it in your own project.

---

## What it generates

CrudGenerator writes the following artifacts in your project through the IntelliJ PSI tree:

- DTOs (Request / Response) with Bean Validation and OpenAPI annotations
- Support builder classes for readable test fixtures
- Custom exceptions shared across the bounded context
- MapStruct mappers between entities, DTOs and embeddable types
- Spring Data repositories wired to the entity's package
- Application services orchestrating persistence and domain events
- Domain events and listeners (event-driven create / update flow)
- REST controllers with the standard CRUD endpoints
- Unit and integration tests for every generated artifact

Generation is **idempotent**: running it twice on the same entity leaves the tree unchanged.

---

## Reporting issues

Bug reports and feature requests are tracked through GitHub Issues. Please use the templates — they capture the information needed to reproduce or evaluate the request:

- **Bug report:** [issues/new?template=bug_report.md](https://github.com/giuseppe-trisciuoglio/jetbrains-crud-generator-plugin/issues/new?template=bug_report.md)
- **Feature request:** [issues/new?template=feature_request.md](https://github.com/giuseppe-trisciuoglio/jetbrains-crud-generator-plugin/issues/new?template=feature_request.md)

Pull requests are not accepted — the source code is private. If you want to contribute, the fastest path is to open an issue describing the change you would like to see; well-scoped requests are welcome.

---

## Reporting security issues

Please **do not** open a public GitHub issue for security problems. See [`SECURITY.md`](SECURITY.md) for the coordinated disclosure policy and the private contact channel.

---

## Maintainer

CrudGenerator is maintained by **Giuseppe Trisciuoglio**.

- Email: <giuseppe.trisciuoglio@gmail.com>
- GitHub: [@giuseppe-trisciuoglio](https://github.com/giuseppe-trisciuoglio)

---

## License

CrudGenerator is distributed free of charge, in binary form only, under the terms of the [End-User License Agreement](EULA.md). The plugin source code is proprietary and is not disclosed.
