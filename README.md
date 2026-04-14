# QuickQuizJSON

A simple quiz app built with a single HTML file (with embedded CSS and JS) that reads quiz data from JSON.

## Features
- Loads quiz questions from JSON
- Multiple-choice questions
- Score tracking
- Lightweight, no build tools

## Run locally
1. Clone/download this repo
2. Open the HTML file in your browser

## JSON Format
Each quiz should include:
- `id` (string, unique)
- `title` (string)
- `questions` (array)

Each question should include:
- `id` (string, unique within quiz)
- `prompt` (string)
- `choices` (array of strings)
- `answerIndex` (number; zero-based index in `choices`)
- `explanation` (optional string)

## JSON format
Example:
```json
[
  {
    "question": "What is the capital of France?",
    "options": ["Berlin", "Madrid", "Paris", "Rome"],
    "answer": "Paris"
  }
]
```

## Project structure
- `QuickQuizJSON.html` — app UI + styles + logic
- `*.json` — quiz data files, there's some examples in the `examples` folder

## Notes
This is a small personal project, so the setup is intentionally minimal.
