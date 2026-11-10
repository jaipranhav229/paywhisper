# PayWhisper

Pay by voice. Say it, check it, confirm it.

PayWhisper turns a spoken sentence like "Send $20 to Ravi" into a payment request. It parses the intent, shows a confirmation card, and asks for a second confirmation on large amounts.

## Live demo
This repository hosts an **interactive demo with simulated payments**. No real money moves.
Open the GitHub Pages link in this repo's About section.

## How it works
1. **Speech to text:** Web Speech API in the demo (Whisper in the full build).
2. **Intent parsing:** extracts amount, currency and recipient from the sentence.
3. **Guardrails:** every payment needs confirmation; amounts above 100 need two.
4. **Payment:** simulated in this demo (PayPal API in the full build).

## What we learned
Voice interfaces need strong guardrails around money, and good intent parsing matters more than raw transcription accuracy.

## Built with
React, Flask, Node.js, Python, Claude API, Whisper, Web Speech API, PayPal

## What's next
Multi-language voice support (including Hindi), recurring payments, split bills and spending summaries.

## Run the demo locally
Open `index.html` in Chrome. No build step needed.

## Author
Jaipranhav (@jaipranhav229)
