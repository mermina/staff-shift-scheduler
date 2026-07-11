# Organisation shifts scheduler

A self-contained, data-driven staff **shift scheduler** for care homes, hospitals, elderly homes, production lines — any organisation that runs on shifts. It builds a fortnightly/monthly rota automatically from a simple staff list and a set of coverage rules, then shows an hours-and-contract balance check for each person.

Everything runs in a single HTML file. No installation, no server, no accounts, no dependencies — just open it in a browser.

**🌐 Live demo:** _<add your GitHub Pages link here>_

> The live demo uses **fictional names and data** for illustration only.

## What it does

- **Auto-generates a rota** from each person's contract %, the shift types they can work, and coverage targets per shift and day.
- **Respects real-world rules:** always a night person on, a supervisor each weekday, one early "opener", 11-hour rest between shifts, a cap on consecutive shifts, weekend cover, and rotating the opener.
- **Keeps fixed patterns** for staff who always work the same days, and auto-schedules everyone else around them.
- **Tracks the hours balance** (over / under contract) per person, with weighting coefficients for evening, weekend, night and public-holiday hours.
- **Bilingual:** Icelandic and English, switchable with one button.
- **Editable in the browser** — change staff, coverage, coefficients and rules, then regenerate. Changes auto-save locally.

## How to use it

1. Open the live demo link above, or download `index.html` and open it in any modern browser.
2. Edit the **Staff**, **Time**, **Shifts & coverage** and **Rules** tabs.
3. Click **Generate schedule**.
4. Review the **Timetable** and the hours/contract check, and export to Excel if needed.

## Data & privacy

- This repository holds **code only** — no real staff data. The demo uses **fictional placeholder names**.
- Real staff information is personal data under GDPR and must live in a private, access-controlled place (e.g. a private sheet shared only with the manager) — **never** in this repo or on GitHub Pages.
- Scope: **staff scheduling data only — no resident or patient data.**
- Data you enter in the tool stays only in your own browser (local storage); nothing is uploaded anywhere.

## Notes

- Designed to be reusable: nothing is hard-coded to one workplace — it's all driven by the data you enter.
- A companion Google Sheets version (same scheduling engine) exists for teams who prefer a shared sheet.
