# Ecosysteem: de Testfabriek

**Doel:** veel producten snel testen en winnaars uitbouwen — als systeem, niet als losse acties.

## Waarom niet "2 shops per dag"

| Probleem | Cijfer |
|---|---|
| Shopify-kosten | 60 stores/mnd × ±€36 = €2.100+/mnd aan lege schappen |
| Ad-budget per serieuze test | ±€100–150 minimum (bron: $20–30/dag, 3-5 dagen) → 60 tests = €6.000–9.000/mnd |
| Betaalprovider | KYC per store; tientallen aanvragen tegelijk = weigeringen/holds |
| Ad-accounts | Verse accounts + verse domeinen in bulk = hoog ban-risico (je echte asset, §9) |
| Service | Tientallen mailboxen/policies bijhouden = precies de hoofdpijn die je niet wilde |

**Inzicht: een test valideert een product + creative, geen store.** Dat kan op een productpagina. Een eigen store bouw je pas voor een bewezen winnaar.

## Het systeem (3 lagen)

```
LAAG 1 — FABRIEK (vast, 1x bouwen)
  1 generieke teststore ("vitrine", bijv. per categorie-cluster)
  + 1 leverancier met Shopify-koppeling + 1 betaalaccount + 1 support-mailbox
  + geautomatiseerde product page-generator (ik) + creative-templates

LAAG 2 — TESTBAND (doorlopend)
  Per week: 3-6 nieuwe producten als pagina + ads erop
  Dag 2-3: CTR/CPC-check → creative kill of door
  Dag 4-6: CPA-check → product KILL of WINNAAR
  Alles gelogd in de repo (testlog), data beslist

LAAG 3 — UITBOUW (alleen winnaars)
  Winnaar → eigen one-product niche-store met branding (ik bouw, 1-2 dagen)
  → schalen; vitrine test intussen door
  Elke maand: 1 categorie-webshop overwegen ALS meerdere winnaars in
  dezelfde categorie vallen (dan is er bewijs, geen speculatie)
```

## Cadans (realistisch vs. gevraagd)

| | Gevraagd | Systeem |
|---|---|---|
| Producttests | 60/mnd (2 stores/dag) | 12-24/mnd (pagina's) — zelfde leersnelheid |
| Nieuwe stores | 60/mnd | 1-3/mnd (alleen winnaars) |
| Vaste kosten | €2.000+/mnd | ±€40-80/mnd (1-2 stores + apps) |
| Ad-budget nodig | €6.000-9.000/mnd | schaalbaar: vanaf ±€1.500/mnd (12 tests) |
| Ban-risico | hoog | laag (accounts bouwen historie op) |

## Kill-criteria per test (vast, vóór launch)

- Creative: CTR < 1% na ±€20 spend → creative kill
- Product: geen winstgevende CPA-indicatie na testbudget (±€100-150) én geen duidelijk pad → product kill
- Winnaar: CPA onder break-even bij stabiele CTR → door naar Laag 3

## Wat dit van jou vraagt

1. **Maandelijks ad-budget vaststellen** → bepaalt de testcadans (€1.500/mnd ≈ 3 tests/week)
2. Eenmalig: Shopify + API-token, leveranciersaccount, betaalprovider, support-mailbox
3. Daarna: wekelijks 10 min de killlijst/winnaars bevestigen — de rest draait

## Automatisering (ik)

- Product pages genereren vanuit leverancier-feed + eigen copy
- Testlog bijhouden in repo, dagelijkse datacheck-routine, kill-adviezen automatisch
- Winnaar-stores bouwen via API
- Support-afhandeling + monitoring zoals in `uitvoeringsplan.md`
