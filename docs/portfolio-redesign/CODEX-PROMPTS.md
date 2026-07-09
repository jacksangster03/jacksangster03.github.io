# Codex Prompts

Use these prompts only after the relevant docs have been reviewed.

## Research prompt

Inspect the existing portfolio repo and `docs/portfolio-redesign/`. Do not edit code.
Produce a short implementation plan for the next smallest safe change. Respect:

- portfolio code lives in this repo;
- Obsidian contains pointer and evidence notes only;
- MCSBT evidence mapping lives in `~/.claude/context/mcsbt/08-portfolio-projects.md`;
- generated assets must be tracked in `ASSET-LEDGER.md`;
- reduced-motion and mobile fallbacks are required.

## Implementation prompt

Implement only the approved phase from `BUILD-SEQUENCE.md`. Do not rewrite the whole
site in one pass. After editing:

- run the local validation available for this repo;
- inspect desktop and mobile layout;
- report changed files;
- do not commit without approval.

## Asset-production prompt

Create or process only assets listed in `ASSET-LEDGER.md`. Keep prompts, source files,
model names, settings and dates beside the asset record. Generated visuals must not
replace factual project evidence.
