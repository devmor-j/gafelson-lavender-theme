# Dark Lavender × Gafelson (Zed theme)

A **Zed editor theme** — the set of rules that define how Zed looks: its
backgrounds, text, syntax colors, and UI. This theme blends **two** source
themes into one:

- **Dark Lavender** — a VS Code dark theme with purple/lavender accents.
- **Gafelson** — a native Zed theme, used as the structural base.

## Layout

```
reference/          # the two source themes — READ ONLY, never edit
  dark-lavender-default.json    # VS Code Dark Lavender
  gafelson-dark-nomal.json      # Zed Gafelson
schema/             # the official Zed theme schema — READ ONLY
  zed-theme-schema-v0.2.0.json
themes/             # THE OUTPUT — the only place to edit
  gafelson-lavender.json
```

## Rules

- **Only edit** `themes/gafelson-lavender.json`.
- `reference/` and `schema/` are **read-only** — never change them.
- When choosing colors, prefer **Gafelson** (the native Zed theme)
  over Dark Lavender.

## Make sure it's still valid

```
python3 -c "import json; json.load(open('themes/gafelson-lavender.json')); print('ok')"
```
