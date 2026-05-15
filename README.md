# IQ Test

A small browser-based IQ test I built as a side project. It's 30 questions, timed at 25 minutes, and it scores you at the end with a rough IQ estimate plus a breakdown of how you did in each category. Inside the app itself it's called "The Cognition Index".

The whole thing is one HTML file. No frameworks, no build step, nothing to install. You open it and it runs.

## Running it

Download `index.html` and open it in any browser. That's the entire setup.

If you want other people to be able to take it, the file is fully self-contained, so any static host works (GitHub Pages, Netlify, Cloudflare Pages, and so on).

## What's in the test

The 30 questions are split evenly across five types of reasoning:

- Numerical reasoning: number sequences and how values relate
- Verbal reasoning: analogies and word relationships
- Logical deduction: inference and consistency puzzles
- Abstract patterns: letter and symbol series
- Spatial reasoning: shapes, rotation, and folding

Questions are interleaved by type so you're not answering six number puzzles in a row. There's a countdown timer at the top, and it auto-submits when it hits zero. You can move forwards and back through the questions, and answer with the mouse or with the A to D keys.

## Scoring

At the end you get:

- An estimated IQ number
- A label for the band you landed in (average, superior, and so on)
- A score for each of the five categories
- A full answer review showing what you picked next to the correct answer

The IQ number is mapped from your raw score out of 30. It is not a real measurement. A proper IQ test is normed against a large population and given under controlled conditions, which this obviously is not. Treat the number as a bit of fun, not a diagnosis.

## How it's built

- One `index.html` file containing the markup, styles, and script
- Plain HTML, CSS, and JavaScript. No React, no libraries, no bundler
- The only external thing it loads is a few fonts from Google Fonts, so it looks best with a connection but still works offline
- All state lives in memory. Nothing is saved or sent anywhere, so each person's run stays on their own machine

The questions and answers live in one array near the top of the script, so they're easy to edit or add to if you want to make your own version.

## Things I might add later

- More questions, and a way to randomise which ones show up
- Image-based spatial puzzles instead of text descriptions
- A harder difficulty mode
- Saving past scores so you can see whether you improve

## Disclaimer

This is for entertainment and self-reflection only. It is not a clinically validated or proctored assessment, and the score should not be used for anything that actually matters.
