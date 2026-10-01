# HSK 1 Flashcards

A browser-based flashcard app to study all 150 HSK Level 1 Chinese vocabulary words.

## Features

- **150 HSK 1 words** — Chinese characters, pinyin, English meaning, and an example sentence
- **Stroke order animations** — animated GIF showing how to write each character (all 150 words covered)
- **Pronunciation audio** — auto-plays the Chinese word when a new card appears; replay with 🔊
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
open index.html
```

**Option 2: Serve locally with Python**
```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## How to Study

1. Cards are shuffled randomly each session
2. Listen to the pronunciation (auto-plays on each new card)
3. Tap the card (or press `Space`) to flip and see the meaning, stroke order, and example sentence
4. Mark **✅ I know it** if you're confident, or **🔄 Review again** if you need more practice
5. Switch to **Study again** mode to drill only the words you're unsure about
6. Use the **Word list** tab to search and see your overall progress

## Progress

Progress is saved automatically in your browser's localStorage — no account needed.  
To reset: open DevTools → Application → Local Storage → delete `hsk1-known` and `hsk1-learn`.

## Sources

- Vocabulary: [hsk.academy/en/hsk-1-vocabulary-list](https://hsk.academy/en/hsk-1-vocabulary-list)
- Stroke order GIFs: [lingust.ru](https://lingust.ru/chinese/chinese-lessons) and [dictionary.writtenchinese.com](https://dictionary.writtenchinese.com)

## Tech

Plain HTML, CSS, and vanilla JavaScript — no build tools, no dependencies, no backend.  
Fonts: [Noto Sans SC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) (Chinese) + [Inter](https://fonts.google.com/specimen/Inter) (UI).  
Audio: Web Speech API (built-in browser TTS, `zh-CN` voice).
