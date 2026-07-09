# Portfolio Redesign

This folder is the canonical implementation planning area for the portfolio redesign.
It belongs in the portfolio repo because it governs the public site build, scene specs,
asset ledger, motion rules and Codex implementation prompts.

## Source-of-truth boundaries

| Area | Canonical location |
|---|---|
| Portfolio code | `/Users/jack/Github/jacksangster03.github.io/` |
| Portfolio redesign docs | `/Users/jack/Github/jacksangster03.github.io/docs/portfolio-redesign/` |
| Raw research package | `research/jack-portfolio-scrollytelling-research-plan-updated.md` |
| Original DOCX package | `research/Jack_Sangster_Portfolio_Scrollytelling_Redesign_Updated.docx` |
| Older research versions | `research/archive/` |
| Strategic pointer note | `/Users/jack/Documents/Obsidian/Claude/Strategic/Portfolio-Redesign.md` |
| MCSBT portfolio evidence mapping | `/Users/jack/.claude/context/mcsbt/08-portfolio-projects.md` |

Obsidian should point here. It should not duplicate the full build spec. Claude context
should route here when the task is about implementing or redesigning the public
portfolio, but it should not mirror these documents.

## Current status

Phase A organisation only:

- Loose research files copied into this repo.
- Original loose folder left untouched.
- No changes made to `index.html` or `style.css`.
- No implementation work started.

## Work order

1. Review the raw research package in `research/`.
2. Confirm or edit the strategy, design, motion and storyboard docs.
3. Populate scene specs before editing portfolio code.
4. Use `ASSET-LEDGER.md` for every generated or captured asset.
5. Use `BUILD-SEQUENCE.md` to keep implementation incremental.
6. Use `CODEX-PROMPTS.md` as the agent handoff surface.

## Documents

| File | Purpose |
|---|---|
| `PORTFOLIO-STRATEGY.md` | Audience, narrative, project hierarchy and content architecture |
| `DESIGN.md` | Visual identity, typography, layout and domain accents |
| `MOTION.md` | Motion grammar, scroll behaviour, reduced-motion constraints |
| `STORYBOARD.md` | Page-wide chapter sequence |
| `ASSET-LEDGER.md` | Asset inventory, generation settings, provenance and usage |
| `BUILD-SEQUENCE.md` | Incremental implementation phases |
| `CODEX-PROMPTS.md` | Research and implementation prompts for coding agents |
| `scenes/` | One spec per major scrollytelling scene |
| `research/` | Full research package and archived older versions |
