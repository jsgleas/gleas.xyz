# GLEAS.xyz

**Repo label:** `storefront/gleas-xyz`  
**Primary product:** Umbrella site/storefront for Gleas brands, services, games, and products  
**Recommended domain:** `gleas.xyz`  
**Stack:** Not yet implemented in this repo  
**Deploy target:** Shopify if commerce-first; Vercel/Cloudflare Pages if custom website-first  
**Status:** Domain/brand hub placeholder

## What this repo is for

GLEAS.xyz is the umbrella website for the rest of the Gleas portfolio: AD Motion, Cookie Monkey, Wavy, Wen, That Work, merch, services, and future products.

Use this repo as the central map for all public properties, even if the actual ecommerce store stays on Shopify.

## Recommended structure

- `/` — umbrella homepage
- `/ad-motion` — advertising services landing page or redirect to `ad-motion.co`
- `/cookie-monkey` — Cookie Monkey product/game page or redirect to `cookiemonkey.co`
- `/wavy` — Wavy product/game page or redirect to `wavy101.com`
- `/wen` — Wen waitlist/landing page
- `/shop` — merch/products; Shopify recommended

## Domain setup

### If using Shopify

Use Shopify as the source of truth for `gleas.xyz` and connect the domain in Shopify’s domain settings.

### If using Vercel or Cloudflare Pages

Build this repo into a real website first, then connect `gleas.xyz` and `www.gleas.xyz` inside the hosting dashboard.

## Naming standard

This repo should be labeled as:

`storefront/gleas-xyz`

It should not hold every app directly. Keep the actual products in separate repos:

- `brand-site/ad-motion`
- `game/cookie-monkey`
- `game/wavy-surf`
- `platform/wen`
- `archive/desktop-tutorial`
