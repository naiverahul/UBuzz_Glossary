# UBuzz — Business Vocabulary, Mastered

A lightweight, single-file web app to master 65+ business terms.
**Zero login. Zero accounts. Progress saves automatically.**

---

## How progress is saved (no login required)

UBuzz uses a **dual-layer storage system** baked into every visitor's browser:

| Layer | Tech | When used | Expiry |
|---|---|---|---|
| Primary | `localStorage` | Always | Until user clears browser data |
| Fallback | Cookie | If localStorage blocked | 1 year, auto-renewed |

Everything is stored as a single JSON blob on the **user's own device**. No server, no database, no accounts. Data never leaves the browser.

**What's saved:**
- Mastered terms (per term)
- Quiz history (last 50 sessions)
- Current streak & last visit date
- Last flashcard position & category
- Total quizzes taken

---

## Running Locally

**Simplest — just open the file:**
```
Double-click index.html → opens in browser
```

**Recommended — local server (better font loading):**
```bash
# Python (Mac/Linux built-in)
cd ubuzz
python3 -m http.server 3000
# Open http://localhost:3000

# Node.js
npx serve .
```

---

## Features

| Feature | Detail |
|---|---|
| Flashcards | 3D flip, category sidebar, keyboard shortcuts, shuffle |
| Quiz | 10 MCQs, score ring animation, all results saved |
| Glossary | Full search + category filter, mastered dots |
| Progress | Per-category bars, full quiz history, storage inspector |
| Export/Import | Download JSON backup, restore anytime |
| Keyboard nav | `←` `→` navigate · `Space` flip · `M` master |
| Streak | Daily visit streak tracked automatically |
| Offline | Works with no internet after first load |

---

## Customising Terms

All terms are in the `TERMS` array inside `<script>` in `index.html`.

```js
// Add your own:
{t:"Your Term", d:"Your definition.", c:"Finance"},
```

Available categories:
`Finance` · `Marketing` · `Strategy` · `Operations` · `HR & Mgmt` · `Startup` · `Accounting` · `Business Law`

---

## Privacy

- No cookies set by servers (only by your own browser)
- No analytics, no tracking, no ads
- No data ever sent anywhere
- All storage is read/write only by you, on your device
