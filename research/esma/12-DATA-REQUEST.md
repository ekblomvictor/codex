# Data request-lista
**2026-08-24 · Bordic**

**Designprincip:** minimera vad ESMA måste lämna ut och maximera vad vi kan hämta själva. **Leverantörsnamn krävs aldrig.**

---

## Nivå 0 — vad vi ber om PÅ mötet (fyra fält, en artikel)

| # | Fält | Varför |
|---|---|---|
| 1 | Artikelnummer / benämning | Identifikation |
| 2 | KN-nummer som används i dag | Testa 7325/7326 och *parts of general use* |
| 3 | Ursprungsland | CBAM in/ut, AD, preferens |
| 4 | Ungefärlig årsvolym i ton | Kostnadsberäkning |

**Frivilligt men värdefullt:** hållfasthetsklass, ytbehandling, styckvikt.
*Hållfasthetsklass + ytbehandling gör att vi kan visa systemgränsanalysen (fil 07) — det mest imponerande draget.*

---

## Nivå 1 — 30-dagarsanalysen

### Från ESMA
| # | Underlag | Format | Kritikalitet |
|---|---|---|---|
| 1 | **Artikelregister**: artikelnr, benämning, KN, ursprungsland, årsvolym (st **och** kg), styckvikt, inköpsvärde | Excel/CSV | 🔴 Måste |
| 2 | **Tulldeklarationer 12 mån** — inkl. **förfarandekod**, tullvärde, nettovikt, AD-tilläggskod | Excel/PDF | 🔴 Måste |
| 3 | **Exportdestination per artikel** (eller aggregerat EU/icke-EU) | valfritt | 🔴 Måste — H1 |
| 4 | De **två inlämnade CBAM-rapporterna** | som inlämnat | 🟠 Hög |
| 5 | Leverantörsmallar/utsläppsdata från rapporterna — **anonymiserade** | valfritt | 🟠 Hög |
| 6 | **EN 10204 3.1-materialintyg**, topp 20 artiklar (E&K har dem sannolikt) | PDF | 🟠 Hög — avslöjar stålrutt |
| 7 | Ytbehandlingsspecifikationer + hållfasthetsklasser | valfritt | 🟡 Medel |
| 8 | Befintliga **tulltillstånd** (tullager, aktiv förädling, AEO) | PDF | 🟠 Hög |
| 9 | **Beslut om godkänd CBAM-deklarant** från Naturvårdsverket | PDF | 🟠 Hög |
| 10 | Ursprungsintyg för JP/CH/TR-flöden (EUR.1, ursprungsförsäkran, A.TR) | PDF | 🟡 Medel |
| 11 | Flödesbeskrivning: går varan fabrik → ESMA HK → Sverige, eller direkt? | samtal | 🟡 Medel |

### Vad vi INTE ber om
❌ Leverantörsnamn och adresser ❌ Inköpspriser per leverantör ❌ Kundlista ❌ ERP-åtkomst ❌ Marginaler

> **Säg detta högt i mötet.** Att aktivt avstå kronjuvelen är starkare än varje sekretessförsäkran.

### Vad Bordic hämtar själv (ESMA behöver inte lyfta ett finger)
| Källa | Vad |
|---|---|
| **TARIC / Tulltaxan** | Tullsatser, AD-tilläggskoder, kvoter, suspensioner |
| **EBTI** | Andras BKB på jämförbara artiklar |
| **EUR-Lex** | Reg. 2022/191 + ändringen 2026/1788; reg. 2026/1384; CBAM-akterna |
| **Naturvårdsverket / Tullverket** | Deklarantprocess, BKB-process, självrättelse |
| **Kommissionens CBAM-standardvärden** | Färdigvarudefault för 7318 |
| **Bolagsverket** | Ägarandelar (verklig huvudman, gratis e-tjänst); årsredovisning ~250 kr |
| **Eurostat / SCB** | Sveriges import av KN 7318 från Kina — rimlighetskontroll |

---

## Nivå 2 — löpande relation
- Nya artiklar vid införande (klassificering vid källan)
- Kvartalsvis tulldeklarationsutdrag
- Leverantörssvar inför deklarationen 30 sep 2027
- Förpackningsdata per artikel (PPWR)
- Materialdeklarationer (REACH/SCIP, ELV/IMDS)

---

## 🔑 Öppningsdraget: hämta deras egen importhistorik åt dem

**Ett svenskt bolag kan begära ut sina egna importdeklarationer från Tullverket** (e-tjänster/Mina sidor, alternativt skriftlig begäran).

> *"Vill du att jag hjälper dig begära ut era egna tolv månaders importdeklarationer från Tullverket? Det är er data, den är gratis, och den finns oavsett om vi jobbar ihop eller inte."*

**Varför detta är rätt första drag:**
- Det ger ESMA något av värde **innan** de betalar något
- Det kräver **ingen** konfidentiell information
- Det ger oss exakt det underlag H1, H2, H3 och H7 behöver — **förfarandekod, tullvärde, nettovikt, AD-kod**
- Det är omöjligt att säga nej till

**Detta är det bästa enskilda draget efter mötet.** Sätt det i uppföljningsmejlet.

---

## Prioriterad ordning om vi bara får tre saker
1. **Tulldeklarationer 12 mån med förfarandekod** — låser upp H1, H2, H3, H7 samtidigt
2. **Artikelregister med KN, ursprung, ton och styckvikt** — låser upp massaavstämning + scope
3. **Exportdestination per artikel** — låser upp den största posten
