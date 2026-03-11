---
description: Key project conventions and repository layout notes
updated: '2026-03-11'
tags:
  - project
  - conventions
  - layout
---
# Project Notes

## Repository Layout

- `repo/` — contains source code for all IPA services:
  - `repo/data-lake-ingester/`
  - `repo/event-hub/`
  - `repo/event-manager/`
  - `repo/event-manipulation-service/`
  - `repo/event-streamer/`
  - `repo/event-transformer/`
  - `repo/eventcatalog/`
  - `repo/stream-events-to-data-lake/`

## Conventions

- When working on a service, look in `repo/<service-name>/` for source code, GitHub Actions workflows (`.github/workflows/`), etc.
- Beans issue tracker lives in `.beans/` — always `beans prime` before any beans operation.
