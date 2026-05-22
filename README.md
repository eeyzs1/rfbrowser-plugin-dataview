# Dataview Plugin for RFBrowser

SQL-like queries over your notes. Filter, sort, and display notes in tables and lists.

## Features

- Query notes by tags, title, content, and metadata
- Display results as sortable tables and lists
- Filter with SQL-like syntax (`WHERE`, `ORDER BY`, `LIMIT`)
- Embed live-updating views in your notes

## Installation

1. Open RFBrowser
2. Go to **Settings > Plugins > Marketplace**
3. Find "Dataview" and click **Install**

Or via the built-in install dialog:
1. Settings > Plugins > Install from URL
2. Paste: `https://github.com/eeyzs1/rfbrowser-plugin-dataview`

## Usage

Create a code block with the `dataview` language in any note:

````markdown
```dataview
TABLE title, tags
FROM "notes"
WHERE contains(tags, "project")
SORT title ASC
```
````

## Permissions

This plugin requires:
- `knowledgeRead` — to query your notes

## Development

```
rfbrowser-plugin-dataview/
├── manifest.yaml    # Plugin metadata
└── ...              # Plugin source code
```

## License

MIT