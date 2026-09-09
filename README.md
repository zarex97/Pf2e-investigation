# Pathfinder Class Codex

A single-file, mobile-first reference to **all 29 Pathfinder Second Edition base
classes** (current through *Impossible Magic*, July 2026).

Each class entry covers three things:

* **The engine** — what you actually do on your turn: the signature actions, the
  subclass fork, the resources you spend, and where the class's difficulty lives.
* **At the table** — what the class means as a character: its fantasy, its
  anathema and obligations, and the roleplay hooks baked into its rules.
* **Downtime** — what the class does between adventures, which is often where
  its personality shows most clearly: the alchemist's lab hours, the barbarian
  building a legend in taverns, the rogue's guild, the wizard's schoolwork.

Plus a **Play it if / Skip it if** verdict and a ten-axis Classfinder profile
per class, readable straight from the list without opening anything.

## Two editions

* `index.html` — English
* `index.es.html` — Spanish (*Códice de Clases de Pathfinder*)

Both are complete and independent. The Spanish edition keeps each class's
**English name** beside the translated one, because the Archives of Nethys and
most PF2e tools are English-only; its search matches either, so `fighter` and
`guerrero` both find the Guerrero. Its profile rows are a little taller because
Spanish axis labels are longer ("Cuerpo a cuerpo" vs "Melee").

## Using it

Open `index.html` (or `index.es.html`) in any browser. No build step, no dependencies, no server.
Fonts load from Google Fonts; everything else is inline.

* **Classes** tab — search across names, mechanics and flavour; filter by chassis
  (Martial / Caster / Hybrid) and party role; sort by any axis.
* **Star** any class to favourite it. Favourites persist in `localStorage`.
* **Favourites** tab — the axis bars for every favourite on one shared scale,
  then a sideways-scrolling table comparing them row by row.

## The ten axes

Ratings come from [Classfinder 2e](https://classfinder2e.com/) and run **0-5**:

| Axis | Meaning |
| --- | --- |
| Melee | Holding your own in close quarters |
| Ranged | Contributing from a distance |
| Defenses | Armour, saves, and staying upright |
| Magic | Access to spells and magical effects |
| Support | Buffing allies and improving their turns |
| Healing | Restoring hit points and clearing conditions |
| Skills | Breadth and depth of skill proficiency |
| Questing | Solving problems outside of combat |
| Popularity | How often the class is played - **neither good nor bad**, shown in gold |
| Difficulty | How demanding the class is to play well - a **cost**, shown in grey |

Every axis carries its own colour and glyph everywhere it appears - the class
list, the detail view, and the comparison - so a class's shape is readable
without checking labels each time.

Eight of the ten are capabilities where more is better. The last two are not,
and they are drawn in deliberately muted greys so a tall bar is never misread
as "better".

## Sourcing

The **ratings** are Classfinder 2e's, supplied as data.

The **written summaries** - engine, roleplay, downtime and the play-it-if
verdicts - are drawn from a field guide compiled from the
[Archives of Nethys](https://2e.aonprd.com/), supplied to the build as a file
because the session itself had no outbound network access. Confirm specific
rules against the Archives before you build a character.

Classfinder also rates six Starfinder 2e classes (Envoy, Mystic, Operative,
Solarian, Soldier, Witchwarper). Those are out of scope here.

To change the ratings, edit the `s:{...}` object on each entry in the `CLASSES`
array inside `index.html`; the axis definitions and the `MAX` scale constant sit
together at the top of the same script.

Always confirm rules details against the [Archives of Nethys](https://2e.aonprd.com/)
before building a character.
