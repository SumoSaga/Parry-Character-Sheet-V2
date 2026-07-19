# ⚔ PARRY

**A dark-fantasy tabletop RPG of duels, guard-breaks, and hard-won victories.**
*A Revelry project.*

This repo is the Parry website — rules reference, gear and trait libraries, and a fully interactive character sheet. It's a plain static site: **no build step, no dependencies.**

## 🔗 Live site

Enable **GitHub Pages** (Settings → Pages → Deploy from branch → `main` / root) and the site goes live at your Pages URL. `index.html` is the landing page.

## Pages

| File | Page |
|---|---|
| `index.html` | Home — what Parry is and how the core loop works |
| `sheet.html` | **Interactive character sheet** — auto-calculating, with pip trackers and a maneuvers flyout |
| `rules.html` | Core rules — opposed rolls, margins, maneuvers, Setups, movement, Grit & Wounds, Poise |
| `gear.html` | Weapons, shields and armor with their Expertise verbs |
| `traits.html` | Trait Slots and the trait library |
| `assets/style.css` | Shared styling for the whole site |

## The system in brief

Both sides roll a d20. The **difference** between the rolls is your **margin**, and margin is a currency:

| Margin | Points |
|---|---|
| 1–4 | 1 |
| 5–9 | 2 |
| 10+ | 3 |

Spend points on damage — or on **Shove, Opening, Feint, Disarm, Trip, Drive Back, Sunder, Rally,** or a lasting **Wound**.

- **Perfect Parry** — matching natural dice turn the blow and snap initiative back.
- **Press-your-luck initiative** — roll even and keep going, roll odd and the spotlight flips.
- **Grit & Wounds** — Wounds permanently shrink your maximum until treated.
- **Poise** — bosses die by having their guard broken, not by attrition.

## The character sheet

`sheet.html` runs entirely in the browser and saves to local storage:

- Attribute point-buy with a live budget
- Auto-calculated **Atk / Def** from attribute + gear, with the breakdown shown
- Hand management — one two-handed weapon, or a one-hander plus off-hand weapon or shield (the **primary** sets your stats)
- **Grit and Armor Slot pip tracks** that start full and tick down
- **Wounds** that reduce maximum Grit as you add them
- Trait slots, expertises, and a **Maneuvers flyout** with distances that scale off your attributes
- Prints cleanly for table use

## Status

In active development. The combat engine, health model, gear, traits, and boss Poise system are drafted and partly validated by simulation. Character creation, the bestiary, magic, and the adventure loop are still being built. Numbers are provisional and tuned at the table.

## License

*To be decided.* Until a license is added, all rights are reserved by the author.

---

*Built by Hayden. Playtests, comments, and broken bones welcome.*
