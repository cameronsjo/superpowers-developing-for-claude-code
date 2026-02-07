# Superpowers: Developing for Claude Code - Fork Maintenance

## Fork Relationship

- **Origin (push)**: `cameronsjo/superpowers-developing-for-claude-code`
- **Upstream (pull)**: `obra/superpowers-developing-for-claude-code`

## Syncing Upstream

```bash
git fetch upstream
git merge upstream/main
```

Documentation-heavy repo. Upstream updates `references/` frequently via scraping scripts. Accept those freely.

## Where Customizations Live

- `README.md` — re-owned header
- `CLAUDE.md` — this file (fork-only)
- Skill content modifications in `skills/`

## What Not to Touch When Merging

- `skills/working-with-claude-code/references/` — auto-generated docs, accept upstream
- `skills/working-with-claude-code/scripts/` — update scripts, accept upstream
- `.claude-plugin/plugin.json` version bumps — accept upstream
