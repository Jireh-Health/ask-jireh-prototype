# Ask Jireh — AI Assistant Prototype (v3)

Interactive prototype of Ask Jireh, the AI assistant inside the Jireh Health patient app.

**Live demo:** https://jireh-health.github.io/ask-jireh-prototype/

## What this prototype demonstrates

**User-initiated + AI-initiated entry points**
- Tap the **Ask Jireh FAB** on the dashboard → opens the Welcome screen with 8 job flows
- Or wait for a **proactive nudge** to appear on the dashboard → tap it to open the chat with that specific scenario pre-loaded

**Demo controls sidebar** (right of the phone)
Pick one of 8 modes:

1. **User taps the FAB (no trigger)** — starts on the Welcome screen with all 8 jobs
2. **Payment request for a dependent** — school-clinic PayLink for Kimathi (Top banner)
3. **Suggest Circle invite from history** (Inline card)
4. **Introduce Circle to solo users** (FAB pulse)
5. **Prompt after taking a loan** (Speech bubble)
6. **Cashback recap for partner regulars** (Inline card)
7. **Non-partner spend recap** (Speech bubble)
8. **Discount matched to care pattern** (Top banner)

**The 8 wired flows** (via FAB → Welcome screen or via job chips)
- Pay a bill (multi-source split — Care Fund + M-Pesa + discount code, STK Push)
- Get help paying (PayLink via SMS to family)
- Cover treatment costs (0% credit line, M-Pesa disbursal)
- Find care nearby (partner-first search + payment point code entry)
- Ask a health question (grounded, escalates to a Jireh partner doctor)
- Send cashback to family (Care Fund → recipient's Care Fund)
- Grow my Circle (SMS invite draft)
- What Jireh does for you (personalised explainer)

## How to run locally

The file is self-contained HTML (React + Tailwind + Babel via CDN — no build step). Just open `index.html` in a browser, or serve from any static host.

## Key design decisions

- **AI composes, user confirms.** Every money move goes through a typed confirmation card. The AI never executes money on its own.
- **Care Fund = Cashback wallet.** They're the same balance. "Cashback" is what you earn (5% of M-Pesa payments to Jireh partner facilities); "Care Fund" is where it sits.
- **Kiswahili + voice input are v2+.** v1 is English-only, chip-driven interaction.

## Related

- Product plan: `2026-08-27-ask-jireh-product-plan.md` (workspace root)
- Nudges design showcase: `jireh-ai-nudges-showcase.html` (workspace root)

---

_Prototype for demonstration only. Bills, contacts, and M-Pesa flows are simulated. Brand-styled per the Jireh Health guidelines._
