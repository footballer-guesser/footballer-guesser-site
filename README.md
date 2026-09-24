# Footballer Guesser

A Wordle-style Premier League guessing game. One static site, no server, no build step.

## Files

| File | What it is |
|---|---|
| `index.html` | The game, with all 6,874 players built in |
| `about.html` | About page (fill in the bracketed bits) |
| `favicon.svg` | Browser-tab icon |
| `og-image.png` | Preview image for WhatsApp, X, LinkedIn etc. (1200×630) |
| `robots.txt`, `sitemap.xml` | For Google |

## Site settings


| Setting | Value |
|---|---|
| Domain | footballer-guesser.com |
| Buy Me a Coffee | Already set to buymeacoffee.com/footballerguesser |
| GA4 | G-XZY1JG4QCR (Search Console verified by DNS) |

If you rename the game, also search for `Footballer Guesser`.

## Analytics

- GA4 loads with Consent Mode v2 set to "denied". Nothing is stored until the visitor clicks **Accept** on the cookie banner, which keeps you on the right side of UK cookie rules.
- Custom events: `game_start` (difficulty), `game_end` (result, guesses, difficulty) and `share`. Mark `game_end` as a key event in GA4 if you want it in reports.

## Deploy (GitHub + Netlify)

1. Create a new GitHub repo and upload everything in this folder.
2. In Netlify: **Add new site > Import from Git**, pick the repo. No build command, publish directory is the root.
3. **Domain management > Add a domain**, then follow Netlify's DNS steps. HTTPS is set up automatically.
4. In Search Console, add the domain property, verify, then submit `https://footballer-guesser.com/sitemap.xml`.

## Data

Squads: Kaggle "All Premier League team and players (1992–2026)", built from Transfermarkt. Goals, appearances and some birth-year fixes are compiled from publicly available Premier League records. Transfermarkt's terms limit reuse of its data, so keep the credit on the About page.
