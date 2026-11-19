# KTUKit — Your KTU Supplementary Exams, War-Room Ready

Ten KTU supplementary papers stand between you and your B.Tech degree. KTUKit is a
single-file war room for all of them: live countdowns, a revision queue, module
checklists, formula flashcards, mock-test tracking and the exact ESE score each
paper needs — all stored on your device, no account, no backend.

**Live:** https://abhiramunni.github.io/ktukit/

## The ten papers

| Code | Paper | Exam | Internal | ESE needed |
| --- | --- | --- | --- | --- |
| MAT101 | Linear Algebra & Calculus (S1) | Tue 15 Dec 2026, 9:30 AM | 36 | 40 |
| MAT102 | Vector Calculus, Differential Equations & Transforms (S2) | Thu 17 Dec 2026, 9:30 AM | 29 | 46 |
| PHT100 | Engineering Physics (S1) | Mon 28 Dec 2026, 9:30 AM | 36 | 40 |
| HUT300 | Industrial Economics & Foreign Trade (S6) | Mon 28 Dec 2026, 1:30 PM | 28 | 47 |
| CYT100 | Engineering Chemistry (S2) | Wed 30 Dec 2026, 9:30 AM | 36 | 40 |
| EST100 | Engineering Mechanics (S2) | Fri 1 Jan 2027, 9:30 AM | 31 | 44 |
| EST130 | Basics of Electrical & Electronics Engineering (S2) | Fri 8 Jan 2027, 9:30 AM | 28 | 47 |
| MAT203 | Discrete Mathematical Structures (S3) | Mon 18 Jan 2027, 9:30 AM | 28 | 47 |
| ITT202 | Principles of Object Oriented Techniques (S4) | Thu 4 Feb 2027, 1:30 PM | 22 | 53 |
| ITT204 | Computer Organization (S4) | Sat 6 Feb 2027, 1:30 PM | 30 | 45 |

Dates come from the revised KTU examination calendar published 16 Nov 2026.
**HUT300's date (Mon 28 Dec, afternoon) is deduced from its slot, not confirmed** —
the app flags it "date to confirm" and the final word is the hall ticket.

## What it does

- **Live countdown** to the next paper (MAT101, 15 Dec), ticking every second.
- **Registration alert** — HUT300 (S6) registration closes without fine on Sun 22 Nov 2026
  (with fine 25 Nov, super fine 27 Nov). S1/S2 registration is already paid
  (₹1,260, ref MP_KTU4437430).
- **The war wall** — all ten papers in exam order, each with a days-left ring, internal
  marks, the ESE score needed, best mock score, best grade still possible, and a
  5-module progress bar. Tap a paper to open its file.
- **Paper files** — module checklist (5 revision steps per paper), the target maths
  (internal, ESE needed, 75/150 rule, best possible grade), that paper's mocks,
  and a "mark ready" toggle.
- **Revision queue** — nearest paper first, least-ready first. 28 December is flagged
  as a double-exam day (Physics morning, Economics afternoon).
- **Formula flashcards** — 17 cards across the ten papers (Laplace transforms,
  eigenvalues, Nernst, Schrödinger, handshaking lemma, Amdahl's law, GDP identity…).
  Tap to flip; filter by paper.
- **Mock-test log** — log previous-year papers (score /100, date, note). A chart plots
  scores against the dashed 40-mark ESE pass line, with pass-pace / below-target
  verdicts per mock.
- **Today's focus + study timer** — logs study minutes in 30/60/90-minute taps, with a
  150-minute daily target bar and a streak counter (60+ minutes a day).
- **Results strip** — S6 30 Mar 2027, S1/S2 6 Apr, S3 1 May, S4 15 May.
- **Six guides** — the 40-mark rule, grade boundaries (S 135+ … P 75+), the double-exam
  day plan, hall-ticket checklist, registration & results, and the last-week plan.
- **Copy exam summary** — one-tap plain-text summary of every paper and your progress.
- Sample data (2 seeded mocks, a few ticked modules, 2 seeded study days) is clearly
  marked and removable with one tap; "Erase everything" resets to a clean slate.

## The 40-mark rule (KTU 2019 scheme)

You need **at least 40 out of 100 in the end-semester paper** and **at least 75 out
of 150 overall** (internal + ESE). Each paper's "ESE needed" is the bigger of the
two — e.g. ITT202 needs 53 because its internal is only 22.

## Privacy

Everything is stored in your browser's localStorage under the key `ktukit_v1`.
Nothing leaves your device. No account, no tracking, no server.

## Run locally

Open `index.html` in any modern browser. To run the headless QA suite:

```bash
node qa-test.js
```

## Tech

Single self-contained HTML file (HTML + CSS + vanilla JS, no framework). Two
AI-generated warm-editorial photographs embedded as data URIs. Fraunces + Inter
via Google Fonts, with system fallbacks. No build step.
