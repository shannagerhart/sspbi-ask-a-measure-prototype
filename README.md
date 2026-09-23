# Ask-a-Measure — NL-to-DAX Prototype

A small prototype for SSPBI: type a plain-English question about AIM data (occupancy, NOI variance, recoveries, rent, returns) and get back the matching measure name, a one-line explanation, and its DAX — instead of hunting through the Data Pane folder tree by hand.

This repo is a demonstration artifact for the **AI-driven product management** prototype requirement: a working prototype built through an AI coding assistant (Claude), committed via a **read-only-verified GitHub connection**.

## What it shows

Open `index.html` in a browser (or GitHub Pages, if enabled on this repo — see below). Type a question, or click one of the example chips, and it returns:

- The matching SSPBI measure name
- A confidence tag ("high match" / "partial match")
- A one-line explanation
- The measure's DAX

## How the matching works (important caveat)

This is **not** a live language model. It's a small local keyword rule set covering five common CRE BI question types (NOI/budget variance, occupancy, recoveries, rent, returns). It's meant to demonstrate the *interaction pattern* — ask in plain English, get a measure back — not to be a production NLP pipeline. See `PROTOTYPE_NOTES.md`.

## Why this exists

RealPage's AI-driven product management practice asks PMs to show they can (a) connect AI tooling to GitHub with read access and (b) produce a small working prototype through that connection. This repo is that evidence, and the concept itself — natural-language access to measures — is also a real product idea worth exploring further for SSPBI, not just a throwaway demo.

See `PROTOTYPE_NOTES.md` for build notes and next-step ideas if this concept is worth taking further.
