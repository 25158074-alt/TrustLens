# TrustLens — Scam Message Analyzer

> Before you trust the message, check it.

TrustLens is a browser-based message checker that reviews pasted text for common scam signals—such as urgency, threats, reward lures, sensitive-information requests, payment pressure, and links—and offers safer next steps.

## Live demo

**Try TrustLens:** https://chimerical-babka-22f483.netlify.app

## Features

- Analyze pasted SMS, email, or message text
- Identify common scam-related wording and signals
- Show matched warning categories and plain-language guidance
- Sample messages for quick testing
- Responsive layout and keyboard focus styling
- Browser-side analysis; text is not sent to a TrustLens backend

## How it works

1. Paste or select a sample message.
2. TrustLens checks the text against a small set of predefined JavaScript patterns.
3. Matching categories and safety suggestions are shown.

This is a lightweight **rule-based checker**, not a trained machine-learning model or an LLM. Results are indicators, not a probability or proof that a message is fraudulent. A message with few matches may still be unsafe.

## Run locally

No build step or package installation is required.

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

   For local hosting, you can also run a simple static server from this directory, for example:

   ```bash
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

## Project files

| File | Purpose |
|---|---|
| `index.html` | Semantic page structure and controls |
| `styles.css` | Visual design and responsive layout |
| `app.js` | Input handling, pattern checks, and result rendering |
| `favicon.svg` | Browser icon |
| `404.html` | Simple not-found page |
| `SECURITY.md` | Security notes and reporting guidance |
| `docs/` | Project overview and demo script |

## Limitations

- Pattern matching can miss unfamiliar scams (false negatives).
- Legitimate messages can match warning patterns (false positives).
- The checker does not validate sender identity, inspect link destinations, or prove authenticity.
- It does not replace official support channels or security tools.

## Safety reminder

Do not share OTPs, passwords, PINs, or payment details because a message asks you to. If a message claims to be from a bank, delivery company, employer, or government service, independently open its official app or website to verify it. Avoid clicking unexpected links.

## Contributing

Issues and pull requests that improve usability, accessibility, test coverage, or detection transparency are welcome. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License

MIT. See [`LICENSE`](LICENSE).
