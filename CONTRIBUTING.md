# Contributing to MarkItDown Workbench

MarkItDown Workbench is planned as a local document-processing workspace with batch conversion, preview, diagnostics, and controlled export.

## Before starting

1. Read `README.md`, `ABOUT.md`, and `ROADMAP.md`.
2. Search existing Issues and pull requests.
3. Open an Issue before changing the job model, output layout, plugin contract, or document-processing pipeline.
4. Keep format-support claims tied to reproducible fixtures.

## Useful contribution areas

- File queue and batch-progress interface.
- Conversion adapters and plugin boundaries.
- Side-by-side source and Markdown preview.
- Table, heading, link, and image-path preservation.
- Cancellation, retry, diagnostics, and recovery behavior.
- Cross-platform packaging, tests, sample files, and documentation.

## Quality requirements

A conversion change should include a small legal-to-distribute fixture, expected output, and a clear explanation of known information loss. Do not commit confidential documents, copyrighted sample books, or private business files.

Use focused Conventional Commit messages: `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, and `chore:`.

Pull requests should describe the problem, affected formats, output differences, validation steps, performance impact, compatibility impact, and documentation changes.

Contributors remain responsible for correctness, licensing, and review of submitted material. Be precise and respectful in technical discussions.