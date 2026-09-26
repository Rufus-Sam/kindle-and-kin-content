# Kindle and Kin — Additional Set

Optional quote pack for the Kindle and Kin app, downloaded only when a user taps **Settings → Get New Quotes**.

- File: `quotes/v1.json` → https://rufus-sam.github.io/kindle-and-kin-content/quotes/v1.json
- Format: `{"version": 1, "quotes": [{"text", "author", "category"}]}` — category is one of `motivation`, `courage`, `gratitude`, `calm`, `success`.
- 1000 original quotes © K&K Digital.

The app validates the file (size cap, known categories, duplicates removed) before saving it. Keep the URL and format stable; publish breaking changes as `v2.json`.
