# Repository Guidelines

## SDLC Skill Source of Truth
- This repository follows the Claude SDLC skill suite in `~/.claude/skills/` (orchestrator, phases 00‑14, support). Treat those `SKILL.md` files as binding development requirements.
- Review `~/.claude/skills/README.md` and the specific phase skill before creating artifacts or changing workflow; record any intentional deviations in the matching `docs/NN_phase-name/` deliverable and call them out in your PR.

## Project Structure & Module Organization
- `docs/` stores phase deliverables such as `docs/01_business-idea/competitor-analysis.md`; add new folders using the `NN_phase-name/` pattern as phases progress.
- Place source modules in `src/`, automation in `support/` or `scripts/`, and mirrored tests under `tests/` once code lands.

## Build, Test, and Development Commands
- Lint docs: `npx markdownlint "docs/**/*.md"` (run before submitting to keep Markdown consistent).
- Format docs: `npx prettier --check "docs/**/*.md"`; use `--write` when alignment is needed.
- No build pipeline exists yet—propose toolchain additions in your PR so the orchestrator flow can evolve deliberately.

## Coding Style & Naming Conventions
- Markdown: wrap near 100 characters, prefer sentence-case headings, and use bullets for procedures.
- Follow `NN_phase-name` directories and kebab-case filenames (`competitor-analysis.md`).
- For future TS/JS code: 2-space indentation, camelCase for variables/functions, PascalCase for classes/components, concise JSDoc for non-trivial logic.

## Testing Guidelines
- No automated tests yet. When you add code, pair each module with `tests/<module>.spec.ts` (Vitest or Jest preferred).
- Target ≥80 % coverage on new surfaces; document justified gaps in the PR.
- Describe any new test commands or fixtures directly in the pull request so reviewers can run them.

## Commit & Pull Request Guidelines
- Use Conventional Commit prefixes (`feat:`, `fix:`, `docs:`, `chore:`) plus an imperative summary, e.g., `docs: add competitor analysis for project marketplace`.
- PR checklist: purpose & rationale, links to affected SDLC phases/issues, verification notes (lint/tests/manual review), screenshots or artifact diffs when helpful.
- Request review from the maintainer covering the impacted phase/system and wait for approval before merging.
