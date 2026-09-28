# Phos & Kin — Quote packs

Original quotes for the Phos & Kin app, written natively for each language (not translated). © Sustain Digital.

| Path | What |
|---|---|
| `packs/<lang>/basic.json` | Basic Set (~1,000 quotes + greeting-card messages). Bundled into the app at build time via `tool/sync_content.sh` in the app repo, so it works offline from first launch. |
| `packs/<lang>/additional.json` | Additional Set (~1,000 quotes). Downloaded only when a user taps **Settings → Get New Quotes**. Served at `https://rufus-sam.github.io/phos-and-kin-content/packs/<lang>/additional.json`. |
| `quotes/v1.json` | Legacy English Additional Set used by app builds before multilingual support. Keep until those builds are gone. |

Languages: `en`, `hi`, `ta`, `zh` (Simplified), `ja`, `ko`, `ar`, `de`, `fr`.

Format: `{"version": 1, "language": "hi", "set": "basic", "quotes": [{"text", "category", "author"?}], "greetings"?: {"birthday": [...], ...}}`
- `category`: `motivation` | `courage` | `gratitude` | `calm` | `success`
- `author` defaults to "Phos & Kin"
- `greetings` keys: `birthday`, `anniversary`, `holiday`, `congratulations`, `thankYou`, `getWell`, `other`

The app validates every file (size cap, known categories, duplicates removed). Keep paths and format stable; bump `version` for content updates.

**Review status:** non-English packs were written by AI and still need native-speaker review before marketing.
