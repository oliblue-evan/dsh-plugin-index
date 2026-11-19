# Oliblue Evan's DSH plugin index

Add this URL in DSH under **Plugins → Discover → Index sources**:

```text
https://oliblue-evan.github.io/dsh-plugin-index/index.json
```

The short GitHub Pages URL is served from the `main` branch. The index uses DSH market format 1 and pins each Git source to an exact commit, so a later push to a plugin's default branch cannot silently change the indexed version. `publishTimestamp` values are the Git commit timestamps. Plugin compatibility declarations are included only when the package manifest declares them.

The index declares categories, capability labels and sort keys, and each plugin carries matching `metadata`, so DSH's Discover tab can show category pills, tag filters and additional sorting options.

## Included plugins

- `dsh-liao-models` — Model Menu Organizer
- `dsh-liao-shelf` — Plugin Shelf
- `dsh-liao-peakclock` — DSH Peak Clock
- `dsh-liao-github` — GitHub Authorization
- `dsh-liao-sidebar` — Sidebar Organizer

The index is static. To publish a new plugin release, update the version, commit SHA, and commit timestamp in `index.json`, then push the change to `main`.
