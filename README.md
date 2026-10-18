# Oliblue Evan's DSH plugin index

Add this URL in DSH under **Plugins → Discover → Index sources**:

```text
https://raw.githubusercontent.com/oliblue-evan/dsh-plugin-index/main/index.json
```

The index uses DSH market format 1 and pins each Git source to an exact commit, so a later push to a plugin's default branch cannot silently change the indexed version. `publishTimestamp` values are the Git commit timestamps. Plugin compatibility declarations are included only when the package manifest declares them.

## Included plugins

- `dsh-model-organizer` — Model Menu Organizer
- `dsh-plugin-shelf` — Plugin Shelf
- `dsh-peakclock` — DSH Peak Clock
- `dsh-github-auth` — GitHub Authorization
- `dsh-sidebar-organizer` — Sidebar Organizer
- `dsh-usage-pill` — Usage & Balance Pill

The index is static. To publish a new plugin release, update the version, commit SHA, and commit timestamp in `index.json`, then push the change to `main`.
