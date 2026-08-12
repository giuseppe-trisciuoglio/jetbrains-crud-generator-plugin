# Security Policy

## Supported versions

Only the **latest release** of CrudGenerator published on the JetBrains Marketplace receives security fixes. Older versions are not patched; please upgrade.

## Reporting a vulnerability

If you have discovered a security vulnerability in CrudGenerator, please report it privately. **Do not** open a public GitHub issue and **do not** discuss it in public channels (forums, social media, chat) until a fix is published.

### How to report

Send an email to **<giuseppe.trisciuoglio@gmail.com>** with the subject prefix `[CrudGenerator Security]`.

Please include, where possible:

1. The plugin version and the IntelliJ IDEA build number where the issue was observed.
2. The operating system and the Java runtime version.
3. A clear description of the vulnerability and its impact (data exposure, arbitrary code execution, denial of service, etc.).
4. Step-by-step reproduction instructions, or a minimal project that triggers the problem.
5. Any proof-of-concept code, screenshots, or relevant log excerpts (Help → *Show Log in Files / Explorer*).
6. Whether you intend to disclose the issue publicly and, if so, on what timeline.

### What to expect

- An acknowledgement of the report within **5 business days**.
- An initial triage decision within **15 business days** of acknowledgement.
- Regular status updates while the fix is in progress.
- A coordinated disclosure plan agreed with the reporter, with a target release date for the fix where applicable.

Until a fix is published, please keep the report confidential so that users have time to update.

## Scope

### In scope

The following are considered security vulnerabilities in CrudGenerator:

- Code execution, file system access, or process invocation outside the project the plugin is acting on.
- Sensitive data exfiltration — environment variables, IDE state, project contents, user files.
- Code injection through generated files (unsafe template substitution, reflection, dynamic evaluation).
- Dependency-related vulnerabilities in vendored libraries shipped with the plugin.
- Sandbox or permission bypass that lets generated code or extension points do more than they declare.

### Out of scope

The following are typically not security issues and should be reported as ordinary bugs through [GitHub Issues](https://github.com/giuseppe-trisciuoglio/jetbrains-crud-generator-plugin/issues):

- Behavioural defects in the generated code that have no security impact.
- Crashes or hangs that require crafted local inputs and have no security impact.
- Issues caused by a user's local environment (JDK version, third-party plugins, custom build scripts) that are unrelated to CrudGenerator itself.
- Output that does not match expectations but stays within the user's own project.

## Recognition

Reporters who follow the coordinated disclosure process are credited in the release notes of the fix, unless they prefer to remain anonymous. Public thank-yous are at the reporter's discretion.
