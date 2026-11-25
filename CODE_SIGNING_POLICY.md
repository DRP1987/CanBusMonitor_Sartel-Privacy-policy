# Code Signing Policy

> Draft for application. Publish this policy after SignPath Foundation accepts the project and signing is configured.

Free code signing provided by SignPath.io, certificate by SignPath Foundation.

## Project and release

- Project: SarTel CAN Bus Monitoring Application
- Source repository: <https://github.com/DRP1987/Sartel_v3.6.14--main>
- Release downloads: <https://github.com/DRP1987/Sartel_v3.6.14--main/releases>
- Licence: MIT for original project materials; third-party notices and terms are listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

## Signing roles

- Authors and maintainers: `DRP1987` and contributors with write access to this repository.
- Reviewers: `DRP1987` reviews and approves changes submitted by contributors who do not have maintainer write access.
- Signing approver: `DRP1987` approves each release signing request after checking the source commit, build, and release contents.

Repository and SignPath accounts used by project members must have multi-factor authentication enabled. Changes to workflow files, build scripts, signing configuration, and release files receive the same review as application code.

## Release signing

Release binaries must be built from this repository using the project's reviewed GitHub Actions workflow and submitted to SignPath through the approved signing policy. Every release signing request requires manual approval. Release archives must include the complete PyInstaller onedir output, preserving the executable and `_internal` directory. Third-party binaries must retain their own notices and must not be represented as original project code.

The release page will identify the signed files, signer, version, and SHA-256 checksum. Users should obtain binaries only from the release page linked above.

## Privacy

The application automatically checks the configured GitHub update manifest after startup and downloads an update only after the user selects the update action. See [PRIVACY.md](PRIVACY.md) for the data and network behavior reviewed for this application.
