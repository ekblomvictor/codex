# Kvantifieringsmodell — formler, indata och räkneexempel
**2026-08-24 · Bordic**

> **Läsanvisning:** Varje siffra är märkt **[K]** = källbelagd, eller **[A]** = antagande som ska ersättas med ESMA:s faktiska data. Inga siffror i denna fil är påhittade. Räkneexemplen är **illustrationer av mekanism**, inte prognoser för ESMA.

**Valutaantagande:** 1 EUR ≈ 11,0 SEK **[A]** — justera vid behov.

---

## DEL A — Verifierade indata

### A1. CBAM-certifikatpris
| Period | Pris | Källa |
|---|---|---|
| Q1 2026 | **€75,36 /tCO₂e** | Kommissionen, publ. 2026-04-07 **[K]** |
| Q2 2026 | **€75,28 /tCO₂e** | Kommissionen, publ. 2026-07-06 **[K]** |
| EUA-snitt maj 2026 | ~€74,04 | **[K]** |
| Q1 2026 spann | €66–90 | **[K]** |

Priset sätts **kvartalsvis 2026**, därefter **veckovis från 2027** **[K]**.
→ **Planeringsvärde: €75/tCO₂e ≈ 825 SEK/tCO₂e.** Använd inte högre — det vore falsk precision.

### A2. CBAM-faktorn (utfasning av fri tilldelning i EU ETS)
| År | 2026 | 2027 | 2028 | 2029 | 2030 | … | 2034 |
|---|---|---|---|---|---|---|---|
| **CBAM-faktor** | **2,5 %** | **5 %** | **10 %** | **22,5 %** | **48,5 %** | … | **100 %** |

**[K]** Största enskilda hoppet: **2029 → 2030 (22,5 % → 48,5 %)**.

> **Detta är den enskilt viktigaste strategiska insikten i hela modellen:** CBAM kostar nästan ingenting 2026 och blir 20× dyrare till 2030. Den som säljer 2026-panik har fel. Den som inte förbereder 2030 har också fel.

### A3. Utsläppsvärden för stål — **läs varningen först**

| Värde | tCO₂e/ton | Not | Källa |
|---|---|---|---|
| Kinesiskt **råstål/slab** (default) | **3,167** | ⚠️ **gäller INTE fästelement** | **[K]** |
| Benchmark BF-BOF (masugn) | 1,370 | | **[K]** |
| Benchmark DRI (gasbaserad) | 0,481 | | **[K]** |
| Benchmark EAF (skrotbaserad) | 0,072 | | **[K]** |
| **Påslag på default** | **+10 % 2026, +20 % 2027, +30 % 2028+** | | **[K]** |

> ### 🚨 KORRIGERING — viktig, och den skiljer oss från amatörer
>
> **1. 3,167 är ett RÅSTÅLS-default. Det får inte appliceras rakt av på KN 7318.**
> Det default som faktiskt styr ett fästelement är ett **färdigvarudefault** som redan innehåller slab + varmvalsning + tråddragning + kallformning + värmebehandling + ytbehandling. Det är alltså **högre** än 3,167 — men jämförelsen mot actuals blir en annan.
>
> **2. Spannet default-mot-actual är INTE 4–40× för ett fästelement.**
> Realistiskt förhållande för ett kinesiskt kallformat kolstålsfästelement är **ca 1,3×**, inte 3×. Skälet: **endast ~10 % av Kinas råstål är EAF/skrotbaserat.** Sannolikheten att en given kinesisk fästelementleverantör sitter på en lågkoldioxidrutt är alltså **låg**.
>
> **3. Konsekvens: actuals-vinsten är mycket mindre än den naiva modellen antyder, och den är koncentrerad till ett fåtal leverantörer.**
>
> **Säg detta i mötet.** John har läst CBAM-material i två år. Alla som ringt honom har vinklat spannet uppåt. Att vi vinklar det *nedåt* och förklarar varför är den enskilt starkaste trovärdighetssignal vi kan ge.

**Detekteringsheuristik (använd i mötet):** *Varje rapporterad emissionsfaktor för ett fästelement under ~0,5 tCO₂e/ton utesluter nästan säkert prekursorstålet.* Det är ett omedelbart test på om en leverantörs siffra är trovärdig.

**Motintuitiv men viktig:** för **svarvade/bearbetade detaljer** allokeras prekursorutsläpp på **insatsmassa**, inte färdig vikt. Spånavverkning kan ge en emissionsfaktor per levererat ton som är **1,5–2,5× ett fästelements**. ESMA säljer precisionssvarvade detaljer — **deras dyraste CBAM-artiklar per ton är sannolikt inte fästelementen.**

### A4. Tullsatser
| Post | Sats | Källa |
|---|---|---|
| KN 7318 tredjelandstull (erga omnes) | **≈3,7 %** | **[K]** |
| **Antidumpning, järn-/stålfästelement Kina (residual)** | **86,5 %** | Förordning (EU) 2022/191 **[K]** |
| — samarbetande, listade i bilagan | **39,6 %** | **[K]** |
| — tre namngivna producenter | **22,1 – 48,8 %** | **[K]** |
| Ny stålförordning (EU) 2026/1384, utomkvotstull | **50 %** | från 2026-07-01 **[K]** |

⚠️ Reg. 2022/191 ändrades av **Kommissionens genomförandeförordning (EU) 2026/1788 av 2026-07-23**. **Kontrollera aktuella satser i TARIC innan de används skarpt.** (UNKNOWN vad ändringen innebär — verifiera.)

### A5. ESMA:s egna publicerade volymuppgifter **[K, PRIMÄR]**
- **"flera tusen ton styckegods årligen"** genom logistikcentret i Spånga
- **"varav ca 50 % exporteras"** — största exportländer i **Nord- och Sydamerika samt norra Europa**
- **importerar från 32 länder, levererar till 39**
- tillverkare i **Japan, Taiwan och Kina** samt **Tyskland och Schweiz**

### A6. Scoping-regler som skär bort volym **[K]**
- **Schweiz är CBAM-undantaget** (bilaga III — ETS-länkat). Tyskland är EU.
  → **Enbart det asiatiska flödet är CBAM-relevant.**
- **KN 7318 (fästelement av järn/stål) ligger i CBAM bilaga I sedan 2023-10-01.**
- **KN 7326 är endast delvis täckt** — bara vissa 8-siffriga undernummer.
  → **Scope-städning är verkligt arbete med verkligt utfall.**
- Plastdetaljer (Vespel®, PUR) ligger **utanför** CBAM.

---

## DEL B — Formlerna

### F1 · Årlig CBAM-kostnad
```
CBAM_år = Σ_artiklar [ ton_i × EF_i (tCO₂e/ton) × P_cert × Faktor_år ] − Cpris_ursprung
```
| Term | Betyder |
|---|---|
| `ton_i` | Ton av artikel *i* **övergått till fri omsättning** i EU (ej återexport under tullager/aktiv förädling) |
| `EF_i` | Inbäddade utsläpp: **actual** (verifierad) eller **default × påslag** |
| `P_cert` | €75/tCO₂e **[K]** |
| `Faktor_år` | 2,5 % (2026) … 100 % (2034) **[K]** |
| `Cpris_ursprung` | Avdrag för koldioxidpris betalt i ursprungslandet (Kinas ETS) — **verifiera tillämplighet** |

### F2 · Värdet av actuals istället för default, per leverantör
```
Värde_actuals = ton × (EF_default×påslag − EF_actual) × P_cert × Faktor_år
Beslut: gör det om  Värde_actuals (nuvärde 2026–2034) > Kostnad_att_hämta_och_verifiera
```
**Detta är value-of-information-formeln.** Den avgör *vilka leverantörer som är värda att jaga* — och, lika viktigt, **vilka som inte är det**.

### F3 · Klassificeringsvärde
```
Årlig effekt   = tullvärde × (fel_tullsats − rätt_tullsats)
Retroaktivt    = årlig effekt × upp till 3 år   (återbetalning enl. UCC, 3-årsfrist)
```
⚠️ **Retroaktiv återbetalning gäller överdebiterad tull vid felklassificering** — den gäller **inte** som "drawback" för återexporterade varor. Blanda inte ihop dem. (Se F4.)

### F4 · Återexport under särskilt tullförfarande *(det stora, förbisedda*)
```
Besparing_framåt = ton_återexport_utanför_EU × värde/ton × (tullsats + ev. AD-sats)
                 + ton_återexport × EF × P_cert × Faktor_år        (bortfallen CBAM)
```
**Rättslig grund [K]:**
- *Aktiv förädling* (Tullverket): *"du behöver inte betala tull … du behöver **inte heller betala antidumpningstullar** eller ha någon importlicens"*
- *CBAM:* varor under aktiv förädling/tullager som **återexporteras utlöser ingen CBAM-skyldighet**; skyldigheten uppstår först vid **övergång till fri omsättning** (EU-kommissionens CBAM-vägledning; finska regeringen)

⚠️ **Detta är en framåtriktad besparing, inte en retroaktiv.** EU har inte amerikansk "duty drawback". Har varan redan gått i fri omsättning är pengarna borta. **Därför är varje månad utan beslut en månad med förlorad besparing** — det är en äkta brådska, inte en påhittad.

### F5 · Tröskelvärdet
```
Om Σ ton CBAM-varor (fri omsättning, per importör, per år) < 50 ton  ⇒  skyldigheten faller i praktiken bort
```
**[K]** 50-tonströskeln infördes genom CBAM-omnibus (antagen 2025-10-08, i kraft 2025-10-20).
För ESMA: **osannolikt under tröskeln** — men **återexportvolymen räknas inte in**, vilket sänker den relevanta massan.

### F6 · Kassaflöde
```
Likviditetseffekt = CBAM_2026 betalas tidigast feb 2027; deklaration 2026-09-30 2027
```
**[K]** Certifikatförsäljning öppnar **2027-02-01**; deklaration för 2026 ska in **2027-09-30**. Bufab redovisar redan **"CBAM-related accruals"** som påverkar europeisk verksamhet och kassaflödestiming **[K]** — dvs. en noterad jämförbar bokför detta som en reell post.

---

## DEL C — Räkneexempel (illustration, ej prognos)

**Antaganden [A] — ska ersättas i mötet:**
| Variabel | Antagande | Grund |
|---|---|---|
| Total volym genom Spånga | 4 000 ton/år | mittpunkt av "flera tusen ton" **[K]** |
| Asiatisk andel av tonnage | 40 % → 1 600 ton | **[A]** |
| Andel därav i CBAM-scope | 85 % → **1 360 ton** | exkl. plast **[A]** |
| Snittvärde | 45 SEK/kg = 45 000 SEK/ton | **[A]** |
| Andel återexport utanför EU | 30 % av importen → **408 ton** | ESMA: 50 % exporteras, varav en del inom EU **[A]** |

### C1 · CBAM med standardvärden
```
1 360 t × 3,484 tCO₂e/t          = 4 738 tCO₂e
4 738 × €75                       = €355 350   (full, ofaktoriserad kostnad)
```
| År | Faktor | Kostnad EUR | Kostnad SEK |
|---|---|---|---|
| **2026** | 2,5 % | **€8 884** | **≈98 000 kr** |
| 2028 | 10 % | €42 000* | ≈460 000 kr |
| 2030 | 48,5 % | **€172 345** | **≈1,9 MSEK** |
| 2034 | 100 % | **€355 350** | **≈3,9 MSEK** |

\* med 30 % påslag från 2028 blir talet högre; se F1.

> **Slutsats: CBAM kostar ESMA storleksordningen 100 000 kr 2026 — och 20–40× mer per år vid decenniets slut.**
> **Säg detta rakt ut i mötet.** Det är den enda meningen som skiljer Bordic från alla andra som ringt honom.

### C2 · Värdet av actuals — **korrigerat nedåt**

Med realistiskt förhållande **1,3×** (default ÷ actual) istället för det naiva 3×:

Antag färdigvarudefault ≈ 3,6 tCO₂e/t och actual ≈ 2,8 tCO₂e/t ⇒ **Δ ≈ 0,8 tCO₂e/t** **[A]**
```
1 360 t × 0,8 × €75 = €81 600/år ofaktoriserat
2026:  × 2,5 %  = €2 040     ≈ 22 000 kr     ← försumbart
2030:  × 48,5 % = €39 576    ≈ 435 000 kr
2034:  × 100 %  = €81 600    ≈ 900 000 kr
```

**Tre slutsatser som måste sägas rakt ut:**

1. **Att jaga actuals 2026 är ekonomiskt irrationellt.** Verifieringskostnaden överstiger vinsten med bred marginal.
2. **Verifieringskostnad tas per anläggning, inte per ton.** Break-even styrs därför av **ton per fabrik** — inte total volym. **Att konsolidera volym på färre fabriker förbättrar CBAM-ekonomin direkt.** Det är ett *inköpsbeslut*, inte ett rapporteringsbeslut. Det är Johns beslut.
3. **Break-even-tonnaget per leverantör faller ~40× mellan 2026 och 2034.** Det som är fel beslut i år är rätt beslut 2029.

> ⚠️ **Och den obekväma sanningen som ingen konkurrent kommer att säga:**
> **Actuals kan bli sämre än schablonen — och när de väl är verifierade måste de användas.**
> Att fråga en leverantör som sitter på en ineffektiv masugnsrutt kan alltså **förstöra värde**. Därför är rätt första steg att *uppskatta* vilken rutt varje leverantör har **innan** man frågar.

### 🔑 Och så kan man göra det — utan att kontakta en enda leverantör
**EN 10204 3.1-materialintyg** som ESMA och E&K med största sannolikhet **redan har i sina ankomstkontrollpärmar** namnger **den faktiska stålverkstillverkaren**. Därmed går det att avgöra EAF vs BF-BOF-rutt — och alltså **beräkna storleken på vinsten innan man ber någon om något.**

Dessutom: **ESMA:s egen artikeldata bevisar vilka processteg som MÅSTE ligga innanför systemgränsen.**
- Hållfasthetsklass **8.8 eller 10.9** ⇒ kräver **seghärdning** (quench & temper)
- **Zinklamellbeläggning** ⇒ kräver **härdugn**

⇒ Får ESMA in en leverantörssiffra som inte kan rymma de stegen, är siffran fel — **och det går att bevisa med ESMA:s egen data, utan leverantörens medverkan.**

**Detta är den mest imponerande enskilda saken Bordic kan visa på fredag.**

### C3 · Återexport under tullager/aktiv förädling — **den stora posten 2026**
```
408 ton × 45 000 SEK/ton = 18,4 MSEK tullvärde
```
| Scenario | Sats | Årlig besparing |
|---|---|---|
| Endast ordinarie tull | 3,7 % | **≈680 000 kr/år** |
| Om AD-belagd (samarbetande) | +39,6 % | **≈7,3 MSEK/år** |
| Om AD-belagd (residual) | +86,5 % | **≈16 MSEK/år** |
| Plus bortfallen CBAM 2030 | | +≈570 000 kr/år |

**Även det försiktigaste scenariot (endast 3,7 %) ger ~7× mer pengar 2026 än hela CBAM-kostnaden.**
**Om någon del av flödet är antidumpningsbelagd är det två storleksordningar mer.**

⚠️ **WORKING HYPOTHESIS (konf. 55).** Vi vet **inte** att ESMA saknar tullager eller aktiv förädling. De säljer redan "dokumenthantering i samband med import/export", vilket tyder på tullkompetens. **Detta är en fråga, inte ett påstående.** Se fil 09, fråga 2.

### C4 · Klassificering
```
250 MSEK inköp × ca 60 % från tredje land = 150 MSEK tullvärde  [A]
Vid 1,0 procentenhets snittfel:  1,5 MSEK/år  +  upp till 4,5 MSEK retroaktivt
```
Verkligt utfall beror helt på artikelregistrets kvalitet. **UNKNOWN** tills vi ser data.

---

## DEL D — Sammanställning: var pengarna faktiskt finns

| Spår | Effekt 2026 | Effekt 2030 | Bevistid | Säkerhet |
|---|---|---|---|---|
| **Återexport under tullförfarande** | **0,7–16 MSEK** | samma + CBAM | 2–4 veckor | Hypotes, hög hävstång |
| **Klassificering + retroaktiv återbetalning** | 0–1,5 MSEK/år + retro | samma | 3–6 veckor | Hypotes, mätbar |
| **Scope-städning (7326 delvis, plast ut, Schweiz ut)** | Sänker hela underlaget | ackumulerar | 1–2 veckor | Hög |
| **Actuals vs default** | ~0 | 1,2–2,6 MSEK/år | 3–9 mån | Hög på sikt |
| **Massaavstämning (styckvikt ↔ tullnettovikt)** | Korrigerar **hela** underlaget | varje år | **1–2 v** | **Mycket hög** |
| **CBAM-certifikat i sig** | **≈0,1 MSEK** | 1,9 MSEK | — | Hög |

### 🥇 Det säkraste 30-dagarsvärdet: massaavstämning
Det enda värdeposten som **inte kräver någon leverantör, ingen utsläppssiffra och ingen myndighet**: stäm av **styckvikt × antal** mot **deklarerad nettovikt** i tulldeklarationerna.
**Ett procentfel i massa är samma procentfel i CBAM-kostnad — varje år, för alltid.** Och det är också fel tullvärdesunderlag.
Detta är den enda leverans Bordic kan **garantera** på 30 dagar.

### 🎯 Den avgörande formuleringen till John
> *"CBAM kostar er ungefär hundratusen kronor i år. Det är inte där pengarna finns 2026. Men den datan ni bygger i år bestämmer vad ni betalar 2030 — och under tiden misstänker jag att det ligger betydligt mer pengar i vad som händer med de femtio procent ni exporterar vidare."*

Den meningen gör tre saker samtidigt: den **avväpnar** (vi överdriver inte), den **positionerar oss som expert** (vi kan faktorn), och den **öppnar det verkliga hålet**.
