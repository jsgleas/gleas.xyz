# GLEAS.xyz

**Current repo:** `jsgleas/gleas.xyz`  
**Preferred future repo name:** `gleas-storefront`  
**Repo role:** umbrella storefront, brand hub, and commerce directory  
**Primary domain:** `gleas.xyz`  
**Recommended commerce backend:** Shopify  
**Deploy target:** Shopify for commerce-first; Vercel/Cloudflare Pages for custom website-first  
**Status:** umbrella brand hub

## Purpose

GLEAS.xyz is the central umbrella for the GLEAS ecosystem. It should point people to AD Motion / AD GLEA, Cookie Monkey, Wavy 101, Wen, Conejo Jo, That Work, merch, services, and future products.

This repo should not become a giant app containing every project. Treat it as the mall, not every store.

## Portfolio map

| Brand | Repo | Role | Domain target |
|---|---|---|---|
| AD Motion / AD GLEA | `jsgleas/ad_motion` | advertising business / 1 LUCKY Ad | `ad-motion.co`, future AD GLEA domain |
| Cookie Monkey | `jsgleas/Cookie-Monkey` | game + character IP | `cookie-monkey.co` |
| Wavy 101 | `jsgleas/WAVY` | game + character IP | `wavy101.com` / `wavy101.co` |
| Wen | `jsgleas/wen-app` needed | social app + landing page | TBD |
| Conejo Jo | `jsgleas/conejo-jo` needed | local media/community brand | TBD |
| That Work | `jsgleas/that-work` needed | future brand/site | `thatwork.co` if owned |
| GLEAS.xyz | `jsgleas/gleas.xyz` | umbrella storefront | `gleas.xyz` |

## Recommended structure

```txt
/
  index.html or app shell
  shop/
  brands/
    ad-motion/
    cookie-monkey/
    wavy101/
    wen/
    conejo-jo/
  docs/
    REPO_MAP.md
```

## Shopify role

Use Shopify as the commerce source of truth when selling merch, products, services, or brand collections.

Recommended collections:

```txt
AD Motion / AD GLEA
Cookie Monkey
Wavy 101
GLEAS
```

GLEAS.xyz can either stay on Shopify directly or become a custom front end that points to Shopify checkout.

## Branch strategy

```txt
main            live production

dev             active testing
feature/*       specific changes
```

Recommended feature branch names:

```txt
feature/brand-directory
feature/shopify-collections
feature/custom-homepage
feature/domain-routing
feature/analytics
```

## Domain setup

### Shopify-first

1. Connect `gleas.xyz` inside Shopify domain settings.
2. Make Shopify the primary commerce experience.
3. Link out to the standalone brand sites.

### Vercel/custom-front-end-first

1. Deploy this repo on Vercel.
2. Connect `gleas.xyz` and `www.gleas.xyz`.
3. Use Shopify only for checkout and product data.
4. Link to each brand’s standalone domain.

## Repo standard

This repo is labeled:

```txt
storefront/gleas-xyz
```

Future rename target:

```txt
storefront/gleas-storefront
```
