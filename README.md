# HSK 1 Flashcards

A browser-based flashcard app to study all 150 HSK Level 1 Chinese vocabulary words.

## Features

- **150 HSK 1 words** — Chinese characters, pinyin, English meaning, and an example sentence
- **Flip animation** — tap the card (or press `Space`) to reveal the answer
- **Track progress** — mark each word as ✅ Know or 🔄 Review again
- **Study again mode** — focus only on words you marked for review
- **Word list** — searchable table of all words with their status
- **Progress saved** — stored in browser localStorage, survives page refreshes
- **Keyboard shortcuts** — `Space`/`F` to flip, `←`/`→` to navigate, `1` = review, `2` = know

## How to Run

No installation needed — it's a single HTML file.

**Option 1: Open directly in browser**
```
open hsk1-flashcards.html
```

**Option 2: Serve locally with Python**
```bash
python3 -m http.server 8080
# then open http://localhost:8080/hsk1-flashcards.html
```

## How to Study

1. Cards are shuffled randomly each session
2. Tap the card (or press `Space`) to flip and see the meaning + example sentence
3. Mark **✅ I know it** if you're confident, or **🔄 Review again** if you need more practice
4. Switch to **Study again** mode to drill only the words you're unsure about
5. Use the **Word list** tab to search and see your overall progress

## Progress

Progress is saved automatically in your browser's localStorage — no account needed.  
To reset: open DevTools → Application → Local Storage → delete `hsk1-known` and `hsk1-learn`.

## Word List Source

Vocabulary from [hsk.academy/en/hsk-1-vocabulary-list](https://hsk.academy/en/hsk-1-vocabulary-list)

## Tech

Plain HTML, CSS, and vanilla JavaScript — no build tools, no dependencies.  
Fonts: [Noto Sans SC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) (Chinese) + [Inter](https://fonts.google.com/specimen/Inter) (UI).
