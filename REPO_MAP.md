# GLEAS Portfolio Repo Map

This file is the source-of-truth map for the GitHub repos, websites, and domains.

## Repo labels

| Repo | Clear label | Product | Confirmed/usable domain | Hosting recommendation | Status |
|---|---|---|---|---|---|
| `jsgleas/ad_motion` | `brand-site/ad-motion` | AD Motion advertising agency site | `ad-motion.co` | Vercel | Active |
| `jsgleas/Cookie-Monkey` | `game/cookie-monkey` | Cookie Monkey browser arcade game | `cookiemonkey.co` / `play.cookiemonkey.co` | Cloudflare Pages or Vercel | Active |
| `jsgleas/WAVY` | `game/wavy-surf` | Wavy surf browser game | `wavyswave.com` / `play.wavyswave.com` | Cloudflare Pages or Vercel | Active prototype |
| `jsgleas/gleas.xyz` | `storefront/gleas-xyz` | Umbrella brand/storefront | `gleas.xyz` | Shopify if commerce-first; Vercel/Cloudflare if content-first | Active storefront placeholder |
| Future repo | `brand-site/that-work` | That Work brand/site | `thatwork.co` | Vercel or Shopify depending on product | Domain available for future build |
| `jsgleas/desktop-tutorial` | `archive/desktop-tutorial` | GitHub Desktop tutorial | None | None | Archive |

## Owned/usable domain inventory

These domains were found from account emails and should be treated as the current usable portfolio domains:

| Domain | Best use | Recommended connection |
|---|---|---|
| `gleas.xyz` | Umbrella Shopify storefront / portfolio hub | Shopify primary domain |
| `ad-motion.co` | AD Motion agency site | Vercel project for `jsgleas/ad_motion` |
| `cookiemonkey.co` | Cookie Monkey brand/game | Cloudflare Pages or Vercel project for `jsgleas/Cookie-Monkey` |
| `thatwork.co` | That Work brand, services, or future job/work platform | Future `brand-site/that-work` repo or redirect to `gleas.xyz/thatwork` |
| `wavyswave.com` | Wavy surf game/brand | Cloudflare Pages or Vercel project for `jsgleas/WAVY` |

No current ownership evidence was found for `wavy101.com` or `wavy101.co`, so do not rely on those domains unless they are purchased later.

## Naming convention going forward

Use a product category prefix in each README and in GitHub descriptions/topics:

- `brand-site/*` — business/agency websites
- `game/*` — browser/mobile games
- `platform/*` — social apps, SaaS, tools, CRM products
- `storefront/*` — commerce hubs and portfolio storefronts
- `archive/*` — old tests, tutorials, unused work

## Recommended public web structure

| Public property | Purpose | Should point to |
|---|---|---|
| `gleas.xyz` | Umbrella storefront and portfolio | Shopify store |
| `ad-motion.co` | AD Motion business site | `jsgleas/ad_motion` deployment |
| `cookiemonkey.co` | Cookie Monkey brand/game | `jsgleas/Cookie-Monkey` deployment |
| `play.cookiemonkey.co` | Direct game entry | Same deployment or game-only route |
| `wavyswave.com` | Wavy brand/game | `jsgleas/WAVY` deployment |
| `play.wavyswave.com` | Direct Wavy game entry | Same deployment or game-only route |
| `thatwork.co` | That Work brand/future product | Future repo or redirect to `gleas.xyz/thatwork` |

## Domain connection checklist

1. Pick one hosting provider per product.
2. Deploy the GitHub repo to that host.
3. Add the custom domain inside the hosting dashboard first.
4. Copy the DNS records the hosting dashboard gives you.
5. Add those records at the registrar/DNS provider.
6. Set one canonical domain per product, usually the apex domain, and redirect `www` to it or vice versa.
7. Enable HTTPS/SSL after DNS resolves.

## Specific setup recommendation

### AD Motion

- Host: Vercel
- Repo: `jsgleas/ad_motion`
- Build command: `npm run build`
- Output directory: `dist`
- Domains: `ad-motion.co`, `www.ad-motion.co`

### Cookie Monkey

- Host: Cloudflare Pages or Vercel
- Repo: `jsgleas/Cookie-Monkey`
- Build command: none
- Output directory: `/`
- Domains: `cookiemonkey.co`, `www.cookiemonkey.co`, optional `play.cookiemonkey.co`

### Wavy

- Host: Cloudflare Pages or Vercel
- Repo: `jsgleas/WAVY`
- Build command: none
- Output directory: `/`
- Domains: `wavyswave.com`, `www.wavyswave.com`, optional `play.wavyswave.com`

### GLEAS.xyz

- Primary host: Shopify
- Domain: `gleas.xyz`, `www.gleas.xyz`
- Use this as the umbrella storefront linking to AD Motion, Cookie Monkey, Wavy, That Work, and future brands.

### That Work

- Domain: `thatwork.co`
- Short-term option: redirect to `gleas.xyz/thatwork`.
- Long-term option: create a dedicated `brand-site/that-work` repo and deploy it on Vercel.

## Do not connect

Do not connect `desktop-tutorial` to any domain. It is an archive/sandbox repo only.
