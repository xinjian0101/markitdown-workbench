# Security Policy

## Current status

MarkItDown Workbench is in the foundation phase. No version should be treated as production-ready until a preview release is explicitly published.

## Reporting a problem

Do not attach confidential documents, private output, or detailed reproduction material to a public Issue. Use GitHub private vulnerability reporting when available. Otherwise open a minimal Issue requesting a private communication channel.

A useful report includes the affected commit, operating system, input format, sanitized sample, reproduction steps, and observed impact.

## Sensitive areas

- Reading files outside the selected input set.
- Writing outside the selected output directory.
- Unsafe archive extraction or path handling.
- Embedded content that triggers unexpected external access.
- Temporary files that are not removed or protected.
- Logs or previews that expose document contents.
- Plugins that receive broader file access than required.

## Expected safeguards

The application should use explicit input and output selections, sanitize paths, isolate temporary work, clearly display overwrites, and avoid external network access unless the user enables it.

## Disclosure

Validated reports will be investigated privately where practical. Public release notes should identify affected versions and remediation without exposing user documents.