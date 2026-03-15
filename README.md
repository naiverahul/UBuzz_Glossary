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

## Visit[ Ubuzz](https://ubuzz.netlify.app/)

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

All terms are stored in the `TERMS` array inside the `<script>` section of `index.html`.

You can contribute by adding new business or startup terms in two ways:

1. **Edit directly on GitHub** and add the term to the `TERMS` array.
2. **Email the term suggestion** if you think it would be useful to include.

📧 Email: [Rahul23418@iiitd.ac.in](mailto:Rahul23418@iiitd.ac.in)

### Example

```js
// Add your own:
{t:"Your Term", d:"Your definition.", c:"Finance"},

Available categories:
`Finance` · `Marketing` · `Strategy` · `Operations` · `HR & Mgmt` · `Startup` · `Accounting` · `Business Law`

---

## Privacy

- No cookies set by servers (only by your own browser)
- No analytics, no tracking, no ads
- No data ever sent anywhere
- All storage is read/write only by you, on your device
