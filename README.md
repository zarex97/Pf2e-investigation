# Pathfinder Class Codex

A single-file, mobile-first reference to **all 29 Pathfinder Second Edition base
classes** (current through *Impossible Magic*, July 2026).

Each class entry covers two things:

* **The engine** — what you actually do on your turn: the signature actions, the
  subclass fork, the resources you spend, and where the class's difficulty lives.
* **At the table** — what the class means as a character: its fantasy, its
  anathema and obligations, and the roleplay hooks baked into its rules.

Plus a **Play it if / Skip it if** verdict and a ten-axis Classfinder profile
per class, readable straight from the list without opening anything.

## Using it

Open `index.html` in any browser. No build step, no dependencies, no server.
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

Eight are capabilities where more is better. The last two are not, and the app
colours them differently so a tall bar is never misread as "better".

## Sourcing

The **ratings** are Classfinder 2e's, supplied as data.

The **written summaries** - the engine, the roleplay, the play-it-if verdicts -
are this codex's own, composed from knowledge of the Remastered rules. The
session that built this had no outbound network access, so nothing was scraped
from the Archives of Nethys; confirm rules details there before you build.

Classfinder also rates six Starfinder 2e classes (Envoy, Mystic, Operative,
Solarian, Soldier, Witchwarper). Those are out of scope here.

To change the ratings, edit the `s:{...}` object on each entry in the `CLASSES`
array inside `index.html`; the axis definitions and the `MAX` scale constant sit
together at the top of the same script.

Always confirm rules details against the [Archives of Nethys](https://2e.aonprd.com/)
before building a character.
