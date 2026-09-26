# chandra54-art/claude

A [Claude Code](https://claude.com/claude-code) plugin marketplace.

## Add this marketplace

```
/plugin marketplace add chandra54-art/claude
```

## Install a plugin

```
/plugin install reflect@chandra54-art-marketplace
```

## What's here

- **reflect** — a mid-conversation reflection skill that pauses execution and
  zooms out from detail-mode to honestly reassess direction, assumptions, and
  bias against the original goal. Vendored unmodified from
  [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills)
  under the MIT License (see [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)).

`alirezarezvani/claude-skills` is a much larger library (300+ skills across
engineering, product, marketing, finance, and more). To pull in the full set
instead of just `reflect`, add that marketplace directly:

```
/plugin marketplace add alirezarezvani/claude-skills
```

## Adding your own plugins

Drop a new plugin directory under `plugins/<name>/` with its own
`.claude-plugin/plugin.json`, then add an entry for it to
[`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json) with a
`source` pointing at that directory (e.g. `"./plugins/<name>"`).
