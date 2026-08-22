# Mindivy Resources

Resource packs distributed to the Mindivy desktop app. The app fetches these
packs through its built-in resource installer — no manual steps are required.

## Repository layout

| Directory | Learning agent | Pack |
|-----------|----------------|------|
| `english/` | English | `graded-readers-v1.zip` — Graded Readers (A1–B1) |
| `python/`  | Python  | `python-foundations-v1.zip` — Python Foundations (Novice–Intermediate) |

Each directory contains a `catalog.json` describing its packs, alongside the
pack archives themselves.

## Packs

| Pack | Entries | Size | Levels | Version | Updated |
|------|---------|------|--------|---------|---------|
| english — Graded Readers | 12 | 0.01 MB | A1, A2, B1 | 1.0 | 2026-07-26 |
| python — Python Foundations | 10 | 0.04 MB | Novice, Intermediate | 1.0 | 2026-08-06 |

- **Graded Readers**: Aesop's fables and short educational articles for
  beginning readers.
- **Python Foundations**: hands-on Python files covering CLI tools, data
  analysis, web scraping, decorators, generators, context managers, testing,
  and type checking.

## How the app consumes this repository

The Mindivy app fetches `catalog.json` from the mirror it can reach (GitHub
raw with Gitee as fallback), then downloads pack archives from the same
source. `download_url` entries in `catalog.json` are relative paths, resolved
against the catalog's own URL.

## Content notes

- The Aesop's fables are in the public domain.
- The original learning materials and Python sample files were written for
  Mindivy.
- Content is provided for use within the Mindivy app. No license to
  redistribute or modify is granted.

## Mirrors

- GitHub: <https://github.com/ruth-zhangx/mindivy-resources>
- Gitee: <https://gitee.com/ruth-zhangx/mindivy-resources>
