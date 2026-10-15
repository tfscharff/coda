# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Status

Coda is a music-focused project whose scope and stack are not yet chosen. No build, lint or test
commands exist yet. Add them here once a stack is picked.

## Conventions

- Remote: https://github.com/tfscharff/coda (public), default branch `main`.
- Commits: Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`…). `.gitmessage` is the commit
  template (enabled per-repo via `git config commit.template .gitmessage`).
- Versioning: SemVer. The current version lives in `VERSION`. A release means: bump `VERSION`, move
  `[Unreleased]` entries in `CHANGELOG.md` under a new version heading and update the compare links,
  commit as `chore(release): vX.Y.Z`, then tag `vX.Y.Z` and push with `--follow-tags`.
- Once a language is chosen, keep its manifest version (e.g. `package.json`) in sync with `VERSION`.
