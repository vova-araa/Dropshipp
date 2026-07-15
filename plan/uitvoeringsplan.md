# Uitvoeringsplan — wie doet wat

**Doel:** volledige operatie (store, producten, fulfilment, service) zo ver mogelijk door de agent laten draaien, met de eigenaar alleen op punten waar dat wettelijk of technisch niet anders kan.

**Fase-check (pijplijn §1):** we zitten in Fase 1. De store (Fase 3) wordt pas gebouwd zodra minstens één product Fase 2 (validatie) haalt. De voorbereiding hieronder loopt parallel zodat er geen tijd verloren gaat.

---

## 1. Rolverdeling — eerlijk afgebakend

### Wat ik volledig overneem (zodra toegang geregeld is)

| Taak | Hoe |
|---|---|
| Productresearch & validatie | Research-templates, marge-berekeningen, GO/SKIP-verdicts |
| Store bouwen op Shopify | Via Shopify Admin API: thema, product pages, collecties, navigatie, policies-pagina's, checkout-instellingen |
| Product-copy & branding | Hero, benefits, social proof-structuur, trust-elementen — conform copy-regels (§4) |
| Producten in de store zetten | Import vanuit leverancier + herschreven titels/copy/prijzen per 3x-regel |
| Fulfilment-automatisering | Leverancier-koppeling (order → automatisch doorgestuurd → track & trace naar klant). "Producten binnenkrijgen" bestaat in dropshipping niet fysiek: de leverancier verzendt rechtstreeks aan de klant; ik regel dat die keten zonder handwerk loopt |
| E-mail & service-templates | Orderbevestiging, verzendupdate, retourflow, FAQ, standaardantwoorden |
| Klantenservice-afhandeling | Periodieke check van het support-postvak (via koppeling), concept- of automatische antwoorden binnen vastgesteld beleid; escalatie naar jou alleen bij geschillen/refunds boven drempel |
| Ads-voorbereiding | Hooks, scripts voor creatives, testmatrix, kill-criteria |
| Monitoring | Routines die voorraad/sync, openstaande orders en supportqueue checken en rapporteren |

### Wat alleen jij kunt (eigenaarschap — eenmalig, ±1-2 uur)

| Taak | Waarom jij |
|---|---|
| Shopify-account aanmaken (trial kan) | Betaalgegevens + eigenaarschap |
| Mij API-toegang geven | Shopify Admin → Apps → "Develop apps" → custom app → Admin API-token. Daarmee bouw ik alles |
| Leveranciersaccount (BigBuy of alternatief — advies volgt uit lopende research) | Contract + betaling staan op jouw naam |
| Betaalprovider activeren (Shopify Payments/Mollie) | KYC: identiteit, bank, KVK |
| KVK-inschrijving (als die er nog niet is) + bedrijfsgegevens voor footer/policies | Wettelijk verplicht; ook nodig voor GPSR-vermelding |
| Domein kiezen/kopen | Eigenaarschap (ik kan voorstellen doen) |
| Support-mailbox aanmaken + koppelen | Eigenaarschap; daarna handel ik hem af |
| Ad-accounts (TikTok/Meta) + budget | Betaalgegevens en accountbeleid staan op jouw naam |

### Wat structureel niet kan

- Ik kan geen rechtspersoon zijn: contracten, BTW/OSS-aangifte en aansprakelijkheid staan op jouw naam. Ik bereid alles voor (incl. OSS-registratie-instructie), jij klikt op bevestigen.
- Fysieke goederenstromen raak ik niet aan — in dit model ook niet nodig.
- Refunds/chargebacks boven een drempel en juridische kwesties: ik stel voor, jij beslist.

---

## 2. Volgorde van uitvoering

```
NU (loopt):     Fase 1 product-niveau — kandidaten huisdierniche + leveranciersvergelijking
DAARNA:         Fase 2 validatie van beste 1-2 producten (marge-keten incl. CPA, angle)
PARALLEL (jij): checklist hierboven — Shopify + API-token is het enige harde blok voor mij
NA VALIDATIE:   Fase 3 store-bouw via API (1-2 dagen werk voor mij)
DAN:            Fase 4 launch — creatives + testbudget + kill-criteria vooraf
```

## 3. Automatiseringsarchitectuur (zodra toegang er is)

1. **Orders:** Shopify → leveranciers-app/koppeling → automatische orderplaatsing bij leverancier → tracking automatisch terug naar klant. Doel: 0 handelingen per order.
2. **Voorraad/prijs-sync:** dagelijkse sync leverancier → store; wekelijkse geautomatiseerde afwijkingscheck (bekende zwakte bij BigBuy) met rapport.
3. **Service:** support-mailbox gekoppeld; standaardvragen (waar is mijn order, retour, maat/gebruik) automatisch of door mij afgehandeld volgens vast beleid; dagelijkse samenvatting; escalaties naar jou.
4. **Bewaking:** terugkerende routine die checkt: onverwerkte orders > 24u, tracking ontbreekt > 48u, supportvragen > 24u onbeantwoord, voorraad hero-product < drempel.

## 4. Servicebeleid (vast te stellen vóór eerste ad — Learned Rule 1 + §9)

- Levertijd communiceren zoals leverancier waarmaakt (onderbeloven, overleveren)
- 14 dagen herroepingsrecht (EU-verplicht) + wie betaalt retourzending → vastleggen
- Refund-drempel: tot €X handel ik zelfstandig af, daarboven jouw akkoord (X stellen we samen vast)
- Reactietijd support: < 24u werkdagen

---

**Status:** wacht op (a) uitkomst productresearch (loopt), (b) jouw checklist hierboven. Het enige dat mij nu blokkeert voor de store-bouw is een Shopify-store + Admin API-token.
