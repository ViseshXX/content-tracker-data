# Content Audit Trail

Versioned mirror of three Mongo collections: **content**, **collection**, **multilingual**.

For instructions on running the weekly sync, see the
[content-tracker-scripts README](../content-tracker-scripts/README.md).

---

## Repo layout

```
content/
    en/content.ndjson       English content records
    hi/content.ndjson       Hindi
    kn/content.ndjson       Kannada
    gu/content.ndjson       Gujarati
    ta/content.ndjson       Tamil
    te/content.ndjson       Telugu
    or/content.ndjson       Odia
collection/
    collection.ndjson       Collection records
multilingual/
    multilingual.ndjson     Multilingual records
reports/                    Human-readable change summary per sync
CHANGELOG.md                Every sync listed, most recent first
.tracker-config.json        Input paths + safety settings (edit before each sync)
```

---

## How to read the history

- **CHANGELOG.md** — quick list of every sync with record counts
- **reports/** — full added/modified/deleted breakdown per sync
- **Git log** — each commit is one collection's worth of changes; use
  `git log --oneline` to browse or `git show <hash>` to see a diff

---

**Last baseline:** 2026-04-26 (tag: `baseline-2026-04-26`)
