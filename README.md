# The Human Library — Telegram Mini App demo

A responsive, self-contained website made for LKC PsychSIG's Human Library promotion.

## Features

- Purple editorial design inspired by PsychSIG's Instagram identity
- Swipeable six-book carousel, with one open preview and five locked books
- "Anxiety — How it feels like" hardcover that animates open
- Two short readable preview pages with a page-flipping animation
- Runs on narrow smartphones, iPhones, Android, desktop browsers and inside Telegram
- No sign-in, database, tracking, third-party images, or secrets

## How to test

Double-click `index.html` in a desktop browser or host the file with a local server. For phones, use the public HTTPS link from GitHub Pages.

## Publish with GitHub Pages

1. Create a **new** GitHub repository, e.g. `psychsig-human-library`. Upload `index.html` to the repository root.
2. Open the GitHub repository **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, choose `main`, then `/ (root)`, and save.
3. Open the HTTPS link GitHub Pages gives you (typically `https://YOUR_USERNAME.github.io/psychsig-human-library/`).
4. Open the URL inside Telegram as a Mini App, using your bot's inline web_app button or menu button. The app can also be opened directly in any browser.

For your `@larrytheteddybot`, you can use the same bot for another Mini App URL. Its bot token should stay only in your private Termux environment, **not** in this public repo. To use a fresh bot instead, create one with BotFather.

## Customisation

- App colors are in the `<style>` block under `:root`.
- Cover text is in the `makeTile(...)` function and the `#cover` HTML section.
- Preview page text is in the JavaScript array `pageContents` near the bottom of `index.html`.
- All other books are intentionally locked in the demo; see `books` array.

**Privacy note:** Text on the book is illustrative demo copy, not an actual sharer's quotation. Replace with exact content approved by the relevant sharer before using this for your event. Anything in a public static web app can be seen by its visitors even when a book appears visually "locked". Never put confidential stories into the HTML or JavaScript.

## Files

Just `index.html` is required to run the app. It has no bundled assets or package-install step.
