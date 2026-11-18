# SleepGuard - Bed Phone Tracker

> Note: this repository is named `Solver` for historical reasons. The project in it is **SleepGuard**.

SleepGuard is a small progressive web app (PWA) that helps you build the habit of not using your phone in bed.

## How it works

1. Place an NFC sticker on your bedside table or charging point.
2. Open SleepGuard on your phone and tap the NFC tag before sleeping to start a session.
3. While the session runs, the app counts the time you spend on the SleepGuard page.
4. If the counted time passes your limit (default 30 minutes), your streak breaks.
5. End the session in the morning to see your streak and recent sessions.

## Features

- NFC tag start (Web NFC API)
- Session timer with streak counter
- Session history stored in LocalStorage (no backend; data stays on the device)
- Installable as a PWA

## Honest limitations

- Web NFC works on Android Chrome only; iOS does not support Web NFC, so NFC start is unavailable there.
- Usage tracking counts only the time while the SleepGuard page itself is open and visible in the browser. It pauses when the page is hidden and the session ends when the page is closed. It does **not** measure phone-wide screen time or usage of other apps.
- This is an early hackathon prototype, not a finished product.

## Run it

Static files only - serve this folder (for example with GitHub Pages) and open `index.html`.

## Tech

HTML5 + vanilla JavaScript, Web NFC API, LocalStorage, PWA manifest.

## License

MIT - see [LICENSE](LICENSE).
