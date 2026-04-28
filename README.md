# Content Audit Trail

Versioned mirror of three Mongo collections: **content**, **collection**, **multilingual**.

**Last baseline:** 2026-04-26 (tag: `baseline-2026-04-26`)
**Last sync:** 2026-04-28 — content (en +937 ~660 −101), (gu ~462), (hi +264 ~1159 −146), (kn +684 ~949 −878), (or ~885 −1), (ta ~20), (te +915 ~170 −8052) · collection +68 ~277 −1 · multilingual ~589

---

## Repo layout

```
data/
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
reports/                        Human-readable change summary per sync
CHANGELOG.md                    Every sync listed, most recent first
tracker-config.example.json     Config template (copy to .tracker-config.json and update paths)
```

---

## How to read the history

- **CHANGELOG.md** — quick list of every sync with record counts
- **reports/** — full added/modified/deleted breakdown per sync, grouped by language
- **Git log** — each commit is one collection's worth of changes; use
  `git log --oneline` to browse or `git show <hash>` to see a diff

---

## Collections tracked

| Collection | Records | Languages |
|-----------|--------:|----------|
| content | ~56,000 | en, gu, hi, kn, or, ta, te |
| collection | ~997 | — |
| multilingual | ~589 | — |
