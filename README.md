# Wordle Solver

A small browser-based Wordle helper that filters a five-letter word list using the clues you enter. No AI, backend, account, or API is required.

## Features

- Five rows of guess tiles (up to five guesses).
- Enter letters with the keyboard; typing advances to the next tile.
- Backspace clears a tile and moves backward; arrow keys navigate.
- Mark tiles gray, green, or yellow by clicking them.
- Combines clues to find possible words from a dictionary.
- Automatically loads `five_letter_words.txt` when hosted online beside `index.html`.
- Manually load a different `.txt` word list, copy results, or export matches.

## Use it online with GitHub Pages

1. Put these files in the **root** of the same GitHub repository:
   - `index.html`
   - `five_letter_words.txt`
   - `README.md` (this file)
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/(root)`, then click **Save**.
5. Open the Pages URL GitHub gives you. The app should fetch `five_letter_words.txt` automatically.

**Important:** the dictionary filename must be exactly `five_letter_words.txt` and it must be in the same folder as `index.html`. The dictionary should contain one word per line; the app keeps unique five-letter words made of A–Z. A public repository means the dictionary file is public too.

## Run locally

You can open `index.html` in a browser. Some browsers block automatic dictionary fetching from a `file://` page, so if it doesn't load automatically, click **Choose word-list file** and select `five_letter_words.txt`. When hosted with GitHub Pages, automatic loading works over the website URL.

## Notes

The results depend on the dictionary you provide. A broad English word list may contain words that the official Wordle game does not accept. This is a clue-filtering helper, not an official Wordle service.
