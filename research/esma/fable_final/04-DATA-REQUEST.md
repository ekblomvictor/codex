# Minsta första datapaket
**Princip: be aldrig om mer än nästa steg kräver. Leverantörsnamn krävs aldrig.**

## På mötet (steg 0) — FYRA fält, en artikel
1. **Artikelnummer/benämning**
2. **KN-nummer** som används i dag
3. **Ursprungsland**
4. **Årsvolym i ton** (ungefär)

*Frivilligt, ger extra analys: hållfasthetsklass + ytbehandling (låser systemgränsen), styckvikt (massatest).*

## Uppföljningsmejlet (samma dag, till John — **cc Magnus ENDAST om John sa ja i mötet**)
> Hej John, tack för i dag. De fyra fälten jag behöver: artikelnummer, KN-nummer, ursprungsland, ungefärlig årsvolym i ton. Har du hållfasthetsklass och ytbehandling också blir analysen vassare — då kan jag visa vilka tillverkningssteg som måste ligga i leverantörens siffra. Inga leverantörsnamn behövs. En sak till, oavsett oss: i Tullverkets e-tjänst **Statistik import** kan ni själva dra ut era importdeklarationer till Excel — deklarations-id, varupost, varukoder med mera. Det är halva underlaget för återexportfrågan — importsidan; exportdestinationerna är andra halvan. Säg till så visar jag vilka fält som behövs. /Victor

## Först vid steg 1 (30-dagarsanalysen)
| Prio | Data | Låser upp |
|---|---|---|
| 1 | 12 mån tulldeklarationer **med förfarandekod** | återexport, AD, massa, klassificering |
| 2 | Artikelregister (KN, ursprung, ton, styckvikt, värde) | scope + massaavstämning |
| 3 | Exportdestination per artikel (eller EU/icke-EU-aggregat) | den stora posten |
| 4 | De två CBAM-rapporterna + leverantörsmallar (anonymiserade) | population + datakvalitet |
| 5 | EN 10204 3.1-intyg topp-20 (finns sannolikt hos E&K) | stålrutt utan leverantörskontakt |

**Steg 0 och merparten av steg 1 kräver inga leverantörsnamn** — A/B/C räcker; AD-satskontrollen körs mot **TARIC-tilläggskoderna i era egna deklarationer**, inte mot leverantörslistan. Behöver vi någonsin gå djupare säger vi det i förväg och ni väljer. **Vi ber aldrig om:** inköpspriser per leverantör · kundlista · ERP-åtkomst · marginaler. *(Säg det oombett.)*
