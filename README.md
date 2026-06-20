<div align="center">

# MarkItDown Workbench

**A local workspace for converting, reviewing, cleaning, and exporting documents as Markdown.**

[![Status](https://img.shields.io/badge/status-foundation-7c3aed)](#project-status)
[![Mode](https://img.shields.io/badge/mode-local--first-0f766e)](#design-principles)
[![Issues](https://img.shields.io/github/issues/xinjian0101/markitdown-workbench)](https://github.com/xinjian0101/markitdown-workbench/issues)
[![Last commit](https://img.shields.io/github/last-commit/xinjian0101/markitdown-workbench)](https://github.com/xinjian0101/markitdown-workbench/commits)

</div>

> [!NOTE]
> This repository is in the foundation phase. Product scope and release gates are documented, but no production-ready desktop build is available yet.

## About

MarkItDown Workbench is planned as a visual, local-first companion for document-to-Markdown workflows. It will combine batch conversion, queue management, side-by-side review, output cleanup, diagnostics, and controlled export in one desktop interface.

The project is intended for users who need repeatable document processing rather than a single-file demo. It will preserve source-to-output traceability and avoid silently changing content.

## Planned workflow

```mermaid
flowchart LR
    A[Add documents] --> B[Inspect formats]
    B --> C[Convert locally]
    C --> D[Review Markdown]
    D --> E[Apply cleanup rules]
    E --> F[Export with report]
```

## Planned capabilities

- Batch queues for common document formats.
- Per-file status, elapsed time, warnings, and retry controls.
- Side-by-side source metadata and Markdown preview.
- Configurable output folders and naming rules.
- Cleanup profiles for headings, lists, tables, spacing, and page artifacts.
- Conversion manifests containing source checksum, options, output path, and result state.
- Batch summary reports in JSON and CSV.
- Clear visibility into which converter handled each file.
- Optional handoff to dataset or retrieval preparation tools.

## Interface direction

| Area | Purpose |
|---|---|
| Queue | Add, order, pause, retry, and inspect jobs. |
| Preview | Compare converted Markdown with source metadata. |
| Cleanup rules | Apply named, reviewable transformations. |
| Export center | Choose output layout, naming, and reports. |
| Activity | Review completed, skipped, and failed jobs. |

## Design principles

- Local processing by default.
- No silent replacement of source files.
- Every cleanup action should be reproducible.
- Conversion warnings remain attached to their output.
- Real screenshots and performance claims appear only after measurement.
- Third-party converter names and licenses remain visible.

## Project status

| Workstream | State |
|---|---|
| Product definition | Active |
| Queue and manifest schema | Planned |
| Conversion adapter | Planned |
| Desktop interface | Planned |
| Cleanup profiles | Planned |
| Packaging | Planned |

## Roadmap summary

1. Define conversion-job and manifest schemas.
2. Build a command-line batch prototype.
3. Add the desktop queue and preview interface.
4. Add cleanup profiles and structured reports.
5. Publish checksummed preview builds and real screenshots.

See [ABOUT.md](ABOUT.md) for repository positioning and suggested GitHub metadata.

## Project relationship

This is an independent companion project. It is not an official Microsoft product. Any integration with third-party software will preserve applicable notices and licenses.

## License

The project license will be finalized before executable source is published.