# GLEAS Repository Map

This is the operating map for the GLEAS website ecosystem.

## Existing repos

| Priority | Repo | Label | Purpose | Domain target | Status |
|---:|---|---|---|---|---|
| 1 | `jsgleas/ad_motion` | `brand-site/ad-motion` | AD Motion / AD GLEA premium landing page and 1 LUCKY Ad funnel | `ad-motion.co`, future AD GLEA domain | Exists |
| 2 | `jsgleas/Cookie-Monkey` | `game/cookie-monkey` | Cookie Monkey browser game, character IP, future merch funnel | `cookie-monkey.co` | Exists |
| 3 | `jsgleas/gleas.xyz` | `storefront/gleas-xyz` | Umbrella storefront and portfolio map | `gleas.xyz` | Exists |
| 4 | `jsgleas/WAVY` | `game/wavy101` | Wavy 101 browser game and character IP | `wavy101.com` / `wavy101.co` | Exists |

## Repos still needed

| Priority | Repo to create | Label | Purpose | Notes |
|---:|---|---|---|---|
| 5 | `jsgleas/wen-app` | `platform/wen` | Wen social app landing page, mobile app, admin, feed, chat, discovery | Should probably become a monorepo later: `apps/web`, `apps/mobile`, `apps/admin` |
| 6 | `jsgleas/conejo-jo` | `brand-site/conejo-jo` | Conejo Jo local media/community page | Keep lightweight and social-first |
| 7 | `jsgleas/that-work` | `brand-site/that-work` | Future brand/site | Hold until the offer is clearer |

## Final target naming

```txt
jsgleas/ad-glea
jsgleas/cookie-monkey
jsgleas/wavy101
jsgleas/wen-app
jsgleas/gleas-storefront
jsgleas/conejo-jo
jsgleas/that-work
```

Current existing repos do not need to be renamed immediately. Rename only when domains, Vercel projects, and internal references are ready.

## Branch standard

Every production repo should use:

```txt
main      = live production

dev       = active testing
feature/* = focused changes
```

Suggested branch names:

```txt
feature/premium-hero
feature/shopify-checkout
feature/mobile-layout
feature/analytics
feature/contact-form
feature/leaderboard
feature/waitlist
```

## Deployment standard

### Vite apps

```txt
Framework: Vite
Build command: npm run build
Output directory: dist
```

### Static game prototypes

```txt
Framework: Other / None
Build command: none
Output directory: project root or static output folder
```

### Shopify storefront

Use Shopify as the commerce source of truth. GLEAS.xyz may either live fully on Shopify or use a custom front end that links to Shopify checkout.

## Rules

1. One serious brand per repo.
2. One production domain per brand.
3. One Vercel/static host project per website.
4. Keep GLEAS.xyz as the umbrella, not the place where every app lives.
5. Never commit real `.env` files or private keys.
6. Use `AGENTS.md` in each repo as the operating instructions for future coding work.
