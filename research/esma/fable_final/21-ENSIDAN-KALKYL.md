# 21 — ENSIDAN: KALKYLARK (internt arbetsblad)

> **Internt Bordic-arbetsblad.** Detta ark används för att fylla i ensidan (exponeringsanalysen) till ESMA Försäljnings AB / John Nyman. Ensidan märks alltid: **"Samtalshypotes – ej klassificeringsbesked."** Alla rader i ensidan ska ha källhänvisning; hänvisningarna nedan är verifierade per **2026-08-28** om inget annat anges.
>
> **Regel:** Verifierade värden skrivs rakt av. Ovверifierade värden markeras **[KONTROLLERA …]** och får ALDRIG ersättas med en gissning i den version som går till ESMA:s tullombud.

---

## 1. Indata (från Johns mejlsvar — de sex fälten)

| # | Fält | Värde (exempel/dummy) | Anteckning |
|---|------|----------------------|------------|
| 1 | Artikelnummer | `ESMA-4711` *(dummy)* | Endast referens |
| 2 | KN/TARIC-nummer | `7318 15 88` *(dummy: sexkantsskruv m. huvud, ej rostfri)* | 8 siffror minimum — CBAM-schablon och AD-omfattning styrs per 8-siffrigt KN-nr |
| 3 | Ursprungsland | Kina *(dummy)* | Ursprung ≠ avsändningsland; E&K Shenzhen ⇒ sannolikt CN-ursprung |
| 4 | Årsvolym | 120 ton *(dummy)* | Omvandla till ton om John anger styck/kg |
| 5 | Tullvärde | 4 800 000 SEK/år *(dummy, ≈ 40 SEK/kg)* | Bas för tull + AD |
| 6 | Tullförfarande/destination | 50 % övergång till fri omsättning, 50 % re-export via Spånga *(dummy)* | Avgör re-exportjusteringen (steg 5) |

**Antaganden som alltid markeras [A] i ensidan:**

| Kod | Antagande | Värde | Källa/motiv |
|-----|-----------|-------|-------------|
| [A1] | Växelkurs | 11,00 SEK/EUR | Avrundad arbetskurs; ange datumkurs i slutversion |
| [A2] | CBAM-certifikatpris | 75 €/tCO2e | Faktiskt: Q1 2026 = 75,36 €, Q2 2026 = 75,28 € (kommissionens publicerade kvartalspriser). 2030-pris okänt — antas konstant |
| [A3] | Kinesisk leverantör utan egen företagsspecifik AD-sats | tre scenarier | Se steg 3 |
| [A4] | Re-exportandel hanteras under tullager/transitering (ej fri omsättning) | enligt fält 6 | Måste bekräftas av John/ombudet — avgörande för steg 5 |

---

## 2. Steg 1 — Konventionell tull (MFN)

**Formel:** `Tull = Tullvärde (SEK) × tullsats`

| KN | Tullsats | Status |
|----|----------|--------|
| 7318 15 xx (inkl. 7318 15 42/48 huvudlösa) | **3,7 %** | Verifierad: hela nr 7318 ligger enhetligt på 3,7 % konventionell tullsats (erga omnes). Källa: EU TARIC / KN 2026, bilaga I till förordning (EEG) 2658/87 |
| 7318 16 xx (muttrar), 7318 22 00 (brickor) | **3,7 %** | Samma grund |
| 7616 10 00 (aluminiumfästelement) | **[KONTROLLERA I TARIC — ca 6 %]** | Ej numeriskt återbekräftad denna runda — slå upp i TARIC innan tryck |

**Dummy:** 4 800 000 × 3,7 % = **177 600 SEK/år** (= 1 480 SEK/ton).

> Alltid: slå upp artikelns exakta 10-siffriga TARIC-rad inkl. **tilläggskoder** (AD-tilläggskod styr vilken sats som tas ut vid gränsen).

---

## 3. Steg 2 — Antidumpning, tre scenarier (Kina, järn/stål-fästelement)

**Rättslig bas:** Art. 1(1), IR (EU) 2022/191 (konsoliderad 02022R0191, 29.7.2025), **i ändrad lydelse genom IR (EU) 2026/1785 och 2026/1788 (23 juli 2026)**. Åtgärderna löper ut **18 feb 2027** om ingen översynsbegäran inkommer senast ~18 nov 2026 (tillkännagivande i EUT C-serien 29 maj 2026 — **dokumentnummer ej verifierat, skriv inte ut något C-nummer**).

**Omfattningskontroll (Art. 1(1)) — innan du räknar:**
- I omfattning: träskruvar (utom franska träskruvar/coach screws), självgängande skruvar, andra skruvar och bultar **med huvud** (även med tillhörande muttrar/brickor), brickor. Ej rostfritt.
- **Utanför:** rostfritt stål; franska träskruvar; skruv/bult för räls; **fristående muttrar (7318 16)** — muttrar omfattas endast när de kommer *tillsammans med* sina skruvar/bultar.
- **OBS — ingen ≤6 mm-undantag:** undantaget för svarvade skruvar med skaft ≤ 6 mm fanns i gamla förordning (EG) 91/2009 (och UK AD2108) men finns **INTE** i 2022/191. Småskruv är alltså fullt i omfattning. Citera aldrig 6 mm-undantaget.
- **Huvudlösa skruvar (KN 7318 15 42/48):** egen NY AD-åtgärd **54,7–72,3 %** enligt IR (EU) 2025/2153 — ersätter trescenariospannet nedan om Johns artikel är huvudlös.

**Formel:** `AD = Tullvärde (SEK) × AD-sats(scenario)`

| Scenario | Sats | Tilläggskod-logik | Dummy (4,8 MSEK) |
|----------|------|-------------------|------------------|
| Bästa fall — namngiven exportör (lägst: Jiangsu Yongyi) | **22,1 %** | Leverantören har egen tilläggskod | 1 060 800 SEK |
| Mellanfall — samarbetande, ej stickprov | **39,6 %** | Leverantör på samarbetslistan | 1 900 800 SEK |
| Värsta fall — övriga (residual) | **86,5 %** | Ingen listad tilläggskod | 4 152 000 SEK |

*(Andra namngivna satser som kan bli aktuella: Ningbo Jinding 46,1 %, Wenzhou Junhao 48,8 %.)*

> Fotnot till 2030-kolumnen i ensidan: AD-satserna gäller t.o.m. 18 feb 2027; 2030-scenariot förutsätter att EIFI begär och beviljas översyn (historiskt regel snarare än undantag; tullarna kvarstår under pågående översyn). Per 2026-08-28 finns ingen offentligt rapporterad begäran. Företagsspecifika satser bör dessutom stämmas av mot konsoliderad version efter rättelserna i IR 2026/1785/1788.

---

## 4. Steg 3 — CBAM 2026

**Population:** hela nr **7318** står i CBAM bilaga I (även 7326); **7325 är ute 2026** (föreslås in från 2028 via COM(2025) 989). Aluminium 7616 10 00: kontrollera bilaga I separat.

**Formel (2026):**

```
CBAM 2026 (SEK) = Årsvolym (ton)
                × DV                (schablonvärde tCO2e/ton, FÖRE påslag)
                × 1,10              (påslag 2026, +10 %)
                × 0,025             (CBAM-faktor 2026 = 2,5 % avgiftsbelagt)
                × 75 €/tCO2e [A2]
                × 11 SEK/EUR [A1]
```

**DV = [KONTROLLERA — schablonvärde Kina × Johns exakta 8-siffriga KN-nr, bilaga I till IR (EU) 2025/2621, RÄTTAD genom IR (EU) 2026/1740 (retroaktiv fr. 1 jan 2026) — hämtas ur kommissionens Excel innan slutversion].**
Trianguerat spann tills dess: **ca 3,5–6,0 tCO2e/t före påslag** (centralt ~3,55; tak ~6,0). Sanitetsankare: Vietnam 7318 15 88 = 3,025 (inkl. påslag); Kina stålämne 3,167.

> **Dubbelräkningsvarning:** kommissionens publicerade 2026-tabeller anger värden **med påslaget inräknat**. Om DV tas från publicerad tabell — hoppa över faktorn 1,10. Formeln ovan gäller värde före påslag.

**Dummy (DV = 3,55 [KONTROLLERA], centralt):**
120 × 3,55 × 1,10 × 0,025 × 75 × 11 ≈ **9 700 SEK/år** (≈ 81 SEK/ton)
Takfall (DV = 6,0): ≈ **16 300 SEK/år**

> CBAM-faktorstege (andel avgiftsbelagd): 2026 2,5 % · 2027 5 % · 2028 10 % · 2029 22,5 % · 2030 48,5 % · 2031 61 % · 2032 73,5 % · 2033 86 % · 2034 100 %.
> Kom ihåg administrativt: godkänd CBAM-deklarant krävs sedan 1 jan 2026 (Naturvårdsverket, beslut upp till 120 dagar; Tullverket stoppar sändningar för icke-godkända importörer).

---

## 5. Steg 4 — CBAM 2030

**Formel (2030):**

```
CBAM 2030 (SEK) = Årsvolym (ton)
                × DV [KONTROLLERA]
                × 1,30              (påslag 2028+ = +30 %, IR 2025/2621 rättad genom IR 2026/1740)
                × 0,485             (CBAM-faktor 2030 = 48,5 %)
                × 75 €/tCO2e [A2]
                × 11 SEK/EUR [A1]
```

**Dummy (DV = 3,55):** 120 × 3,55 × 1,30 × 0,485 × 75 × 11 ≈ **222 000 SEK/år** (≈ 1 850 SEK/ton)
Takfall (DV = 6,0): ≈ **375 000 SEK/år**

**Obligatorisk caveat-rad i ensidan:** *"2030-beräkningen antar konstant certifikatpris 75 €/tCO2e [A2] och oförändrade schablonvärden; certifikatpriset följer ETS-auktionspriser och kan avvika väsentligt. Faktiska verifierade utsläppsdata i st.f. schablon kan sänka kostnaden med faktor 3–5 (branschexempel, EFDA)."*

---

## 6. Steg 5 — Re-exportjustering ("zeroing")

ESMA re-exporterar ~50 % via Spånga. Princip:

- Gods som hanteras under **suspensivt förfarande** (tullager/transitering) och lämnar EU utan övergång till fri omsättning ⇒ **varken tull, AD eller CBAM**.
- Gods som **övergår till fri omsättning** och därefter re-exporteras ⇒ tull kan i vissa fall återfås (särskilda förfaranden), men **CBAM saknar exportjustering/återbetalning i den definitiva fasen** — CBAM-kostnaden fastnar.

**Formel:** `Effektiv exponering = Full exponering × (1 − andel via suspensivt förfarande)`

**Dummy (50 % via tullager [A4]):**

| Post | Full exponering | Effektiv (×0,5) |
|------|----------------|-----------------|
| Tull 3,7 % | 177 600 | **88 800** |
| AD 22,1 / 39,6 / 86,5 % | 1 060 800 / 1 900 800 / 4 152 000 | **530 400 / 950 400 / 2 076 000** |
| CBAM 2026 (centralt) | ~9 700 | **~4 850** |
| CBAM 2030 (centralt) | ~222 000 | **~111 000** |

> Om fält 6 visar att re-exporten i praktiken sker EFTER fri omsättning: sätt justeringen till 0 för CBAM och flagga tullagerupplägg som besparingsmöjlighet (det är Bordics säljvinkel — kvantifiera skillnaden).

---

## 7. Summering per scenario (dummy, effektiv exponering 60 t fri omsättning)

| SEK/år | Bästa (22,1 %) | Mellan (39,6 %) | Värsta (86,5 %) |
|--------|---------------:|----------------:|----------------:|
| Tull 3,7 % | 88 800 | 88 800 | 88 800 |
| Antidumpning | 530 400 | 950 400 | 2 076 000 |
| CBAM 2026 | ~4 850 | ~4 850 | ~4 850 |
| **Totalt 2026** | **~624 000** | **~1 044 000** | **~2 170 000** |
| CBAM 2030 (i st.f. 2026-raden) | ~111 000 | ~111 000 | ~111 000 |
| **Totalt 2030** *(AD villkorad, se fotnot steg 2)* | **~730 000** | **~1 150 000** | **~2 276 000** |

---

## 8. Känslighet — vad flyttar svaret mest?

1. **AD-scenariot** (störst): spannet 22,1 → 86,5 % är faktor ~3,9 på den dominerande kostnadsposten. Leverantörens tilläggskod är den enskilt viktigaste uppgiften att få från John/E&K.
2. **Re-exportandel + förfarande:** halverar eller nollställer inte poster linjärt — CBAM saknar exportåterbetalning, så förfarandevalet (tullager före fri omsättning) är binärt avgörande för halva volymen.
3. **CBAM-schablonvärdet:** spann 3,5–6,0 ger ±70 % på CBAM-raderna — försumbart 2026 (~5–8 tkr), betydande 2030 (~110–190 tkr effektivt).
4. **Certifikatpris 2030** [A2]: helt osäkert; linjärt genomslag på 2030-raden.
5. **Växelkurs** [A1]: linjärt, ±5 % — minst viktig.
6. **Huvudlös-frågan:** om artikeln är KN 7318 15 42/48 byts hela AD-spannet mot 54,7–72,3 % (IR 2025/2153) — kontrollera FÖRST.

---

## 9. Checklista — 5 färska uppslag per artikel (görs om för VARJE artikel John skickar)

- [ ] **1. TARIC-uppslag** (10-siffrig kod): konventionell tullsats + samtliga **tilläggskoder** (AD-kod per exportör, ev. skyddsåtgärder) — direkt i EU:s TARIC-konsultation/Tullverkets tulltaxa. *(3,7 % för 7318 verifierad; 7616 10 00 [KONTROLLERA ca 6 %].)*
- [ ] **2. CBAM-schablonvärde:** exakt värde för Johns 8-siffriga KN-nr × Kina ur bilaga I till **IR (EU) 2025/2621, rättad genom IR (EU) 2026/1740** (retroaktiv 1 jan 2026) — kommissionens Excel på CBAM-sidan. Kontrollera om tabellvärdet redan inkluderar påslaget (då: ingen ×1,10/×1,30).
- [ ] **3. AD-omfattning:** artikeln mot Art. 1(1) IR 2022/191 (konsoliderad, i ändrad lydelse genom 2026/1785/1788): rostfri? fransk träskruv? räls? fristående mutter? med/utan huvud? *(Inget ≤6 mm-undantag finns.)*
- [ ] **4. Huvudlös-kontroll:** om KN 7318 15 42 eller 7318 15 48 → IR (EU) 2025/2153 (54,7–72,3 %) i stället för trescenariospannet.
- [ ] **5. CBAM-populationskontroll:** står Johns KN-nr i bilaga I till CBAM-förordningen i nu gällande lydelse? (7318/7326 ja; 7325 nej 2026, föreslagen fr. 2028 via COM(2025) 989 — EP-omröstning väntad sept 2026; 7616 kontrolleras separat.)

**Bonusflaggor (en rad var i ensidan, ingen beräkning):** (i) Steel Reg (EU) 2026/1384 — pågående omfattningsöversyn t.o.m. 28 sep 2026 gäller tråd/insatsvaror = uppströms kostnadssignal 2027; (ii) förordning 833/2014 bilaga XVII/Art. 3g — 7318 omfattas, MTC-ursprungsbevisning krävs redan i dag; (iii) sanktionsavstämning av leverantörskedjan E&K Shenzhen.

---

## 10. Källrader att klistra in i ensidan (per post)

| Post | Källrad |
|------|---------|
| Tull | EU TARIC / KN 2026, bilaga I förordning (EEG) 2658/87 — konventionell tullsats 3,7 % (nr 7318) |
| AD-scenarier | Art. 1(1) IR (EU) 2022/191 (konsoliderad 02022R0191, 29.7.2025), i ändrad lydelse genom IR (EU) 2026/1785 och 2026/1788; utlöper 18 feb 2027 (tillkännagivande i EUT C-serien 29 maj 2026 — skriv ej ut C-nummer) |
| AD huvudlösa | IR (EU) 2025/2153 (KN 7318 15 42/48, 54,7–72,3 %) |
| CBAM-population | CBAM-förordningen (EU) 2023/956, bilaga I; COM(2025) 989 (7325 fr. 2028, förslag) |
| CBAM-faktor | Övergångsstege 2026–2034: 2,5→100 % |
| Schablonvärde + påslag | IR (EU) 2025/2621, rättad genom IR (EU) 2026/1740 (retroaktiv 1 jan 2026); påslag +10/20/30 % (2026/2027/2028+) |
| Certifikatpris | Kommissionens kvartalspris: Q1 2026 = 75,36 €, Q2 2026 = 75,28 € |
| Sverige/deklarant | Naturvårdsverket (godkänd CBAM-deklarant); Tullverket (stopp av sändningar); kommissionens vägledningspaket 14/21/27 aug 2026 |

*Slut på arbetsblad. Ensidan får inte lämna Bordic med kvarstående [KONTROLLERA]-markeringar.*
