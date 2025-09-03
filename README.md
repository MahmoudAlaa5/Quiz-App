# Quiz App (HTML/CSS/JS)

A simple, modern quiz application with categories, randomized questions/answers, progress bullets, score, and timer.

## Project Structure

```
├── index.html        # App markup
├── main.css          # Styles (modern, subtle elevation)
├── script.js         # App logic
├── Questions.json    # Question bank per category
└── README.md         # This file
```

## Features

- Randomized question order per chosen category
- Answers shuffled per question
- Next/Previous navigation
- Progress bullets (active bullet reflects current question)
- Score tracking (increments on correct answer)
- Running timer (mm:ss)
- Clean, lightweight UI

## Getting Started

Because the app fetches `Questions.json`, you should run it via a local server (not opening the file directly), otherwise `fetch` may fail due to browser security rules.

### Quick start with Python
- PowerShell / Terminal:
```bash
python -m http.server 5500
```
- Then open:
```
http://localhost:5500/index.html
```

### Or with Node (if installed)
```bash
npx serve . -l 5500 --single
```
Open `http://localhost:5500/index.html`.

## Usage
1. Choose a category
2. Click Start
3. Click an answer to receive immediate feedback
4. Use Next/Previous to navigate; bullets indicate position
5. Score updates on correct answers; timer runs until the last question

## Customization
- Add or edit questions in `Questions.json` (keys match category names: `islamicHistory`, `science`, `programming`, `math`)
- Tweak styles in `main.css` (colors, spacing, elevation)

## License
MIT
