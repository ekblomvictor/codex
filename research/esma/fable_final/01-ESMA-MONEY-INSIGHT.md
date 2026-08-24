# Money-insikten — den starkaste verifierade Challenger-insikten
**2026-08-24 · Fable-verifierad · för mötet 28/8**

---

## Insikten i en mening

> **ESMA:s importupplägg är byggt för EU-försäljning — men hälften av godset lämnar EU igen. Om det godset förtullas till fri omsättning vid ankomst betalar ESMA tull, eventuell antidumpningstull och (från 2026) CBAM på varor som aldrig konsumeras i EU — pengar som inte går att återfå i efterhand.**

Det är en Challenger-insikt därför att den (a) kommer från ESMA:s *egna* publicerade uppgifter, (b) inte handlar om CBAM-rapportering — området John redan behärskar — utan om *tullarkitektur*, och (c) implicerar att den största kostnaden inte är den alla pratar om.

---

## Beviskedjan — vad som är VERIFIERAT

| # | Led | Källa | Status |
|---|---|---|---|
| 1 | Spånga-centret hanterar *"flera tusen ton styckegods årligen, varav ca 50 % exporteras"*, störst till Nord- och Sydamerika + norra Europa | esma.se (logistiksidan) | **VERIFIED — PRIMÄR** |
| 2 | ESMA levererar *"vanligtvis EXW Stockholm"* så att kunden *"aldrig behöver tänka på … tull"* | esma.se | **VERIFIED — PRIMÄR** |
| 3 | EXW Stockholm förutsätter att varan är förtullad och i fri omsättning i Spånga | Incoterms/tullogik | **STARK SLUTLEDNING** |
| 4 | Varor under **tullager eller aktiv förädling** som återexporteras betalar **varken tull, antidumpningstull eller CBAM** | Tullverket (aktiv förädling); EU-kommissionens CBAM-vägledning; finska statsrådet | **VERIFIED — PRIMÄR** |
| 5 | EU har **ingen drawback** — tull på varor i fri omsättning återfås inte vid senare export | UCC-systematik | **VERIFIED** |
| 6 | AD-tull på kinesiska stålfästelement: **86,5 % residual / 39,6 % samarbetande / 22,1–48,8 % namngivna (Yongyi 22,1 · Jinding 46,1 · Junhao 48,8)** (förordning (EU) 2022/191) | EUR-Lex | **VERIFIED — PRIMÄR** *(satserna oförändrade av sommarens ändringar 1788/1785 — löst i två pass)* |
| 7 | CBAM-faktorn: **2,5 % 2026 → 48,5 % 2030 → 100 % 2034**; certifikatpris ~€75/tCO₂e | Kommissionen | **VERIFIED** |

## Ekonomisk mekanism

```
Årligt läckage = ton_återexport_utanför_EU × värde/ton × (tullsats + ev. AD-sats)
              + ton_återexport × EF × €75 × CBAM-faktor          ← växer 20× till 2030
```

**Försiktigt intervall** (endast ordinarie tull 3,7 %, antagna volymer):
- 300–500 ton/år lämnar EU à ~45 000 SEK/ton ⇒ tullvärde 13–23 MSEK ⇒ **läckage ~0,5–0,8 MSEK/år**
- **Citera detta intervall — inte mer.** Om delar av flödet är AD-belagt är beloppet en storleksordning större, men det får sägas som *"och ligger något av det under antidumpning pratar vi helt andra belopp"* — aldrig som en siffra.

## Vad som MÅSTE vara sant (och hur det testas i mötet)

| Antagande | Test | Om falskt |
|---|---|---|
| ESMA är importör i eget namn (inte agentur) | Fråga 2 i liveguiden | Byt spår: kundvänd data/PCF |
| En väsentlig del av exporten lämnar **EU** (Amerika, Norge, UK — inte bara EU-länder) | Fråga 1 | Wedge krymper; CBAM-population + AD-satser tar över |
| ESMA saknar tullager/aktiv förädling i dag | Fråga 1 (förfarandet) | Byt till population-vs-förfarande-avstämning — fortfarande vårt jobb |
| Fri omsättning är inte ett **medvetet val** | Lyssna efter *"vi förtullar allt med flit — kunden slipper tull, det är vår produkt"* | Svar: *"Helt rimligt — därför räknas det netto: läckaget växer 20× till 2030 via CBAM-delen, så ett upplägg som var rätt 2020 kan bli fel 2028. Blir netto negativt efter lagerkostnad säger vi det."* |
| Volym/värde-antagandena är rimliga | En-artikelanalysen | Justera intervallet med deras data |

## Två verifierade stödpunkter (nya 2026-08-24)

1. **Sanktionsbeviskravet gäller redan.** Bilaga XVII till förordning 833/2014 omfattar CN 7318, och Kommissionens FAQ tar *kinesiska fästelement gjorda av ryskt valstråd* som sitt första exempel på förbjuden import. ESMA måste alltså **redan i dag** kunna visa verksintyg (EN 10204 MTC) på att kinesiska leverantörers stål inte är ryskt. **Samma intyg avslöjar stålrutt (EAF/masugn) för CBAM.** En datainsamling — två skyldigheter lösta. [VERIFIED — Kommissionens FAQ, PRIMÄR]
2. **Kinas egna fabriker är nu inne i ETS — men avdraget är ~noll.** Utvidgningen (mars 2025, stål/cement/aluminium; CNY 67–86/t under 2025) ger i första cykeln **fri tilldelning motsvarande hela den verifierade 2024-emissionen** — fabrikerna köper inget, alltså finns i praktiken inget "betalt koldioxidpris" att dra av under art. 9 ännu. Rätt drag: begär ändå leverantörens ETS-verifieringsdata — den är CBAM-användbar och avdraget växer när Kinas fria tilldelning stramas åt. [VERIFIED]

3. **Standardvärdena rättades för tre veckor sedan — retroaktivt.** IR (EU) 2026/1740, i kraft 2026-08-03, rättar fel i standardvärdestabellerna (2025/2621) **retroaktivt från 1 jan 2026** — inklusive felmappade varukoder. Den som räknade sin 2026-exponering i våras räknade på fel tabell och måste räkna om. Direkt fråga till John, och ett levande bevis på varför löpande bevakning är en tjänst. [VERIFIED]

4. **Brick-återbetalningen (IR 2026/1788).** TARIC-koderna för AD-belagda brickor under ex 7318 22 00 rättades i juli 2026 retroaktivt till 2022-02-18 — AD-tull betald på de utgångna koderna ska återbetalas *enligt tillämplig tullagstiftning*, vilket i praktiken betyder att **treårsfristen (UCC art. 121) styr hur långt bakåt man når** — äldre deklarationer preskriberas löpande, därav brådskan. Har ESMA importerat kinesiska brickor finns sannolikt pengar att hämta, mot en ansökan. [VERIFIED — EUR-Lex via agentspår]
5. **Ny AD-åtgärd de kan ha missat:** IR (EU) 2025/2153 (okt 2025) lägger **54,7–72,3 %** på **skruv utan huvud** (stoppskruv/gängstång-familjen) från Kina. [VERIFIED]

6. **Tio nya CBAM-vägledningsdokument 14 aug 2026** (definitiva perioden; 4 generella + 6 sektorsspecifika; operatörsvägledning finns **på kinesiska**) + operatörsportalen i drift sedan 1/1 2025 — fabriker registrerar en gång, alla importörer återanvänder. Vägen för E&K är alltså redan byggd. [VERIFIED]

## Varför detta slår en ren CBAM-pitch
CBAM 2026 kostar ESMA i storleksordningen **100 000 kr** (faktor 2,5 %). Att säga det högt — och att peka på en tullpost som sannolikt är 5–8× större *i år* — visar bättre prioritering och ekonomisk analys än varje konkurrent som ringer om "CBAM-compliance". Metodbeviset: exakt denna typ av flödesanalys (klassificering, förfarande, actuals-mot-default, producent-mappning) är vad Bordic redan gör löpande åt sin referenskund, en svensk stålimportör.
