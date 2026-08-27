# Ismael Torres Cabrera

**I build autonomous systems — and most of the work goes into teaching them when *not* to act.**

Self-taught engineer working on agent orchestration, trading automation, and local-first AI. I care about the unglamorous parts: what happens when the session expires at 3am, what the system does with a half-finished run, and why the default answer should usually be "skip."

---

## What I'm building

**[prediction-market-bot](https://github.com/Djisma/prediction-market-bot)** · Python · *public*
A four-stage research pipeline over Polymarket built on the Claude Agent SDK. Filters the market universe by liquidity and residual uncertainty, gathers real context from Reddit, RSS and spot-price APIs, forms an independent probability estimate, then applies a fractional Kelly gate that defaults to no action. Read-only by design — it researches and sizes, it does not trade.

**[Right Seat](https://rightseat-cfi.higgsfield.app)** · JavaScript · *live*
A companion web app for flight instructors (CFI / CFII / MEI), built as a single self-contained page with offline-capable local persistence. Started as a tool I needed for my own students and shipped as a product.

**HeroBot** · Python · *private*
An unattended trading system running against a live brokerage account. Hard mechanical risk limits — daily loss cap, per-trade risk ceiling, maximum concurrent positions, correlation guard — enforced in code rather than left to judgment. Structured logging and out-of-band alerting, with API credentials kept entirely outside the source tree.

**Agent Dungeon** · JavaScript · *private*
A multi-agent orchestration cockpit built on two non-negotiable rules: agents never fabricate data to fill a gap, and no consequential action executes without explicit human approval. The interesting design problem was making "I don't know" a first-class result.

**Local voice stack** · Python · *private*
Speech synthesis and inference running entirely on local hardware — no third-party API calls, no audio leaving the machine.

---

## How I work

- **Fail loudly, never silently.** A run that dies with a non-zero exit beats one that quietly overwrites good state with garbage.
- **Persist incrementally.** Partial results are worth keeping. Crashing at step 4 of 5 shouldn't cost you steps 1 through 3.
- **Isolate faults.** One bad item in a batch logs an error and moves on; it doesn't take the run down with it.
- **Secrets never touch the source.** Config through environment, gitignored, with a checked-in example that contains only thresholds.
- **Bound everything that grows.** Logs rotate, history gets capped, caches expire.

## Stack

`Python` · `JavaScript / Node` · `Bash / PowerShell` · `Linux / WSL` · `SQLite / JSON state` · `REST APIs` · `LLM agent orchestration` · `Whisper / XTTS` · `Tailwind`

## Background

- Cyber Defense Professional Certificate — University of Central Florida, 2020
- Coursework in Computer Science and Aerospace Engineering — University of Central Florida
- FCC Restricted Radiotelephone Operator Permit
- FAA Certified Flight Instructor — which is where the aviation software comes from
- Field technical background: satellite installation supervisor and instructor trainer, where I wrote the training curriculum and compliance checklists

Working with LLM tooling since early 2023 — back when running a model locally meant wrestling MPT-7B onto your own GPU.

## Reach me

[LinkedIn](https://www.linkedin.com/in/ismael-torres-cabrera)
