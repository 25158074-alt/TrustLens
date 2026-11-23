# TrustLens project overview

## Problem
Scam messages often use urgency, fear, rewards, impersonation, links, or payment requests to pressure recipients into risky actions.

## Goal
Give users a quick, understandable review of common warning signals and practical advice to verify messages safely.

## Current implementation
A static frontend built with HTML, CSS, and JavaScript. JavaScript pattern checks identify known indicator categories. The app presents matching signals and recommendations. It runs locally in the browser without a TrustLens server or database.

## Technical choices
- HTML for structure and semantic controls
- CSS for styling and responsive behavior
- Vanilla JavaScript for input, pattern matching, and UI updates
- Static hosting (Netlify) for public deployment

## Limitations and future ideas
Patterns are not contextual understanding. False positives and false negatives are expected. Potential future work includes a test corpus with labeled examples, measurable precision/recall, multilingual patterns, and privacy-reviewed contextual analysis.
