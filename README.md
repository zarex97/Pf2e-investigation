# Pathfinder Class Codex

A single-file, mobile-first reference to **all 29 Pathfinder Second Edition base
classes** (current through *Impossible Magic*, July 2026).

Each class entry covers two things:

* **The engine** — what you actually do on your turn: the signature actions, the
  subclass fork, the resources you spend, and where the class's difficulty lives.
* **At the table** — what the class means as a character: its fantasy, its
  anathema and obligations, and the roleplay hooks baked into its rules.

Plus a **Play it if / Skip it if** verdict and an eight-axis profile per class.

## Using it

Open `index.html` in any browser. No build step, no dependencies, no server.
Fonts load from Google Fonts; everything else is inline.

* **Classes** tab — search across names, mechanics and flavour; filter by chassis
  (Martial / Caster / Hybrid) and party role; sort by any axis.
* **Star** any class to favourite it. Favourites persist in `localStorage`.
* **Favourites** tab — the axis bars for every favourite on one shared scale,
  then a sideways-scrolling table comparing them row by row.

## The eight axes

Six are upsides (higher is better): Damage, Survivability, Support, Control,
Utility, Versatility. Two are **costs**, drawn in grey — Complexity and
Bookkeeping. A high cost bar means the class asks more of its player, which some
people want and some don't.

## Sourcing

The session that produced this had **no outbound network access**, so the
write-ups were composed from knowledge of the Remastered rules rather than
scraped from the Archives of Nethys, and the eight bars are this codex's own
editorial read — they are **not** the ratings from classfinder2e.com.

To swap in real numbers, edit the `s:{...}` object on each entry in the
`CLASSES` array inside `index.html`; the axis list itself lives in `AXES` at the
top of the same script.

Always confirm rules details against the [Archives of Nethys](https://2e.aonprd.com/)
before building a character.
