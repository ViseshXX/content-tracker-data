# Content Tracker

This repository holds the current state of the content, collection, and multilingual records, and a report for every sync that shows exactly what changed.

---

## What's in here

| Folder | What it contains |
|---|---|
| `data/content/<language>/` | All content records for that language, one file per language |
| `data/collection/` | All collection records |
| `data/multilingual/` | Multilingual translation records |
| `reports/` | Excel reports — one file per sync, per language |

---

## How to see what changed

Open the `reports/` folder and find the date of the sync you want to review.

Each Excel report has four sheets:

- **Summary** — counts of what was added, changed, and removed
- **Added** — full details of every new record
- **Modified** — every field that changed, with the before and after value
- **Deleted** — full details of every removed record

---

## Languages

| Code | Language |
|---|---|
| `en` | English |
| `hi` | Hindi |
| `ta` | Tamil |
| `kn` | Kannada |
| `gu` | Gujarati |
| `te` | Telugu |
| `or` | Odia |
