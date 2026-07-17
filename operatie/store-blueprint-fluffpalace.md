# Store-blueprint FluffPalace (fluffpalace.shop)

Bouwvolgorde zodra API-token binnen is. Doel: teststore live in 1 dag, conversie-klaar.

## Structuur

```
Homepage        → minimaal: logo, hero richting hero-product, trust-strip (bijzaak, §4)
/products/
  sunspot-raamhangmat     ← TEST 1 (ads landen hier)
  drybuddy-drooghandjas   ← TEST 2
  + upsell-producten (3-5, geen ads): speeltje, borstel — na leverancierscheck
/pages/
  over-ons, contact, faq
/policies/
  retourbeleid (14 dgn), privacybeleid, algemene voorwaarden, verzendbeleid
```

## Instellingen

- Taal NL, valuta EUR, iDEAL via Shopify Payments
- Domein fluffpalace.shop koppelen
- Checkout: gast-checkout aan, telefoonnummer optioneel
- Footer: KVK + bedrijfsgegevens eigenaar (GPSR/wettelijk verplicht) — **gegevens nodig van eigenaar**

## Thema

Gratis thema (Dawn/vergelijkbaar), aangepast: rustige basis, veel wit, productfoto's groot, sticky add-to-cart mobiel (ads = 90%+ mobiel verkeer). Geen countdown-timers of nep-schaarste (Learned Rule 3 / §9).

## Apps (minimaal, §8)

| App | Doel | Kosten |
|---|---|---|
| Leveranciers-app (CJ of GOGETTERS) | product-import + auto-fulfilment | €0–30/mnd |
| Judge.me of Shopify-reviews | echte reviews verzamelen | gratis tier |
| Upsell-app (post-purchase) | AOV verhogen | gratis tier eerst |

Meer apps pas als een test wint.

## Copy

Klaar: `operatie/copy/test1-raamhangmat.md`, `test2-drooghandjas.md`. Invulvelden (prijs, specs, levertijd) na leverancierskoppeling.

## Checklist launch-gate (vóór eerste ad)

- [ ] Betaalprovider actief (iDEAL getest met testorder)
- [ ] Policies + KVK in footer
- [ ] Retourbeleid definitief
- [ ] Landed cost bekend → prijs via 3x-regel
- [ ] Kill-criteria in testlog bevestigd
- [ ] Tracking: Shopify-pixel + TikTok/Meta-pixel
