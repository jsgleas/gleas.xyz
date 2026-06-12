# Agent Instructions

## Repo purpose

This repo is only for GLEAS.xyz: the umbrella storefront, brand directory, commerce hub, and top-level links across the GLEAS portfolio.

Do not build the full AD Motion, Cookie Monkey, Wavy, Wen, Conejo Jo, or That Work products directly inside this repo. Link to those standalone repos and domains.

## Stack rule

Keep this repo lightweight unless the user explicitly asks for a full custom storefront.

Recommended directions:

```txt
Shopify-first for commerce
Vercel/custom front end only if the user wants a custom GLEAS homepage
```

## Portfolio rule

GLEAS.xyz is the mall, not every store. It should organize and point to:

- AD Motion / AD GLEA
- Cookie Monkey
- Wavy 101
- Wen
- Conejo Jo
- That Work
- merch and services

## Branch convention

```txt
main = production

dev = testing
feature/* = focused changes
```
