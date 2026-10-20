# THE SMOKE — Covenant Design Website

A **standalone six-page website dedicated exclusively to The Smoke** tabletop roleplaying game.

Created by Covenant Design, using actual vector faction emblems, illustrated London maps, venue maps, player rulebook and game data from the supplied **The Smoke v0.5.6 Foundry development package** and the **Homebrewery v0.5.0 player book**.

## Opening locally

Unzip the folder. Double-click `index.html`. The whole public site works as static HTML/CSS/JS with no build system, analytics or external dependencies. Links to the existing GitHub project and to real radio station homepages need an internet connection.

If your browser restricts local files, serve the directory in a terminal:

```
python -m http.server 8080
```

Then visit http://localhost:8080

## Deploying

Upload the *contents* of this folder (the file `index.html` at the repository root) to a new dedicated GitHub Pages repository or any static host (Cloudflare Pages, Netlify, etc.). **Do not upload this website into the Foundry system distribution repository unless you deliberately want to mix releases and web content.**

GitHub Pages example: create a new repository named `the-smoke-website`, upload all files, then under Settings → Pages choose Deploy from a branch → `main` → `/ (root)`.

There is **no invented signup backend**, no user login, no purchases, no database, no radio stream bundled, and no claims that a local Foundry build is already published. The Blower is an informational demo.

## Pages

- `index.html` — branded landing page, city/crew overview, interactive Heat demo.
- `city.html` — actual 20-zone interactive atlas plus venue interiors.
- `factions.html` — twelve genuine faction emblems, descriptions, patrons and dossier overlays.
- `rules.html` — stats, exact d6 Effort + exploding stat die test roll and outcomes, driving/Heat/Rep primer.
- `missions.html` — publicly safe teaser board (15 selected jobs), without GM-only campaign spoilers.
- `play.html` — player book resource, Foundry project and compatibility notes.

## Editing

- Main visual styles: `css/site.css`.
- Interactions: `js/site.js`.
- Game data: `js/content.js` (generated from the game, but human-editable JavaScript).
- Copy and page structure: the six HTML files.
- Game artwork: `assets/`. These are compressed web-sized exports of supplied art. Full-resolution assets remain in the Foundry package.
- Source player book: `downloads/The-Smoke-Player-Rulebook-Homebrewery.txt`.

## Disclosure / versioning

The local Foundry **v0.5.6** ZIP supplied to build this site was described as release-ready but *not yet confirmed published or live-tested*. The website links to the GitHub **releases listing** instead of claiming that version is installed. The public player book remains the **v0.5.0 Homebrewery edition**.

The currently shipped Foundry self-play mode requires an **online active GM client** for world state. The site does not imply autonomous online hosting or fully automatic NPC conversations. `125` jobs counts 12 opening + 93 further faction commissions + 20 local cases.

## Legal / credits

The Smoke: A Covenant Design production. Game materials credit Benjamin Vale / Pacts & Polyhedrals. Covenant Dice System © 2026 Dracouroboros Ltd., Benjamin Vale and Paige Kibodeaux; all rights reserved. Foundry VTT is a trademark of Foundry Gaming LLC. Icon artwork includes game-icons.net contributions under CC BY 3.0 when used. Radio links point to independent broadcasters; no stream is bundled.

All real location names and geography are used in an invented tabletop game; venue interiors, companies and crimes are fictional and do not describe real locations or organisations.

Only player-facing material is intentionally in the deployable site. **Do not publicly add or link the GM-only Campaign Book or GM journal datasets** if you want players to discover the mystery in play.
