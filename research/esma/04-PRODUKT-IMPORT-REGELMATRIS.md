# Produkt-, import- och regleringsmatris
**2026-08-24 · Bordic · ESMA Försäljnings AB**

> ⚠️ **Användningsregel:** KN-nummer nedan är **arbetshypoteser för samtal**, inte klassificeringsbesked. Slutlig kod kräver objektiva fakta om varje artikel (material, dimension, huvudtyp, hållfasthet, gängning, ytbehandling, användning). **Ange aldrig en KN-siffra för John som ett faktum om vår artikel.** Säg *"det här brukar hamna i…"*.

---

## 1. Huvudmatrisen — produktfamilj → KN → CBAM → tull → handelspolitik

| ESMA-familj | Trolig KN | **CBAM?** | Tull (MFN) | Antidumpning | Övrigt |
|---|---|---|---|---|---|
| **Fästelement, stål** (skruv, bult, mutter, bricka, nit) | **7318** (hela rubriken) | ✅ **JA** | ~3,7 % | ⚠️ **Kina: 22,1 / 39,6 / 86,5 %** | Största posten |
| Fästelement, **rostfritt** | 7318 (rostfria undernr) | ✅ **JA** | ~3,7 % | ❌ **Nej — uttryckligen undantaget** | Viktig avgränsning |
| Fästelement, **svarvade, skaft ≤6 mm** | 7318 | ✅ JA | ~3,7 % | ❌ **Nej — undantaget i 2022/191** | 💰 Kontrollera! |
| Fästelement, **aluminium** | **7616 10 00** | ✅ **JA** | **~6,0 %** | – | Ofta glömt |
| Fästelement, **koppar/mässing** | 7415 | ❌ **NEJ** (kap. 74 utanför CBAM) | ~3,0–3,7 % | – | Scope-städning |
| **Gjutgods** — "andra gjutna varor av järn/stål" | **7325** | ❌ **NEJ** | ~1,7–2,7 % | Ev. gjutjärn (2018/140, snävt) | 💰 **Se §2** |
| **Smide / stansning / pressning** | **7326** | ✅ **JA** | ~2,7 % | – | 💰 **Se §2** |
| **Fjädrar** | **7320** | ❌ **NEJ** | ~3,7 % | – | Ut ur populationen |
| **Rördelar, flänsar, kopplingar** | **7307** | ✅ **JA** | ~1,7–3,7 % | – | |
| **Sintrade detaljer** (AMES + Kina) | 7326 / kapitelvarierande | ⚠️ **Beror på kod** | varierar | – | Ursprung: AMES har verk i **Wuhu, Kina** |
| **Svarvade / bearbetade maskindelar** | 84xx / 85xx / 87xx **eller** 7326 | ⚠️ **Avgörs av kod** | 2,2–8,0 % | – | 💰 **Se §3 — störst hävstång** |
| **Plastdetaljer** (Vespel®, PUR) | 3926 90 | ❌ **NEJ** | ~6,5 % | – | Ut ur CBAM |
| **Metal Binder Jetting** (AMES, från dec 2025) | 7326 / maskindel | ⚠️ Beror | varierar | – | Ny familj |

**CBAM täcker endast sex sektorer:** cement, el, gödsel, **järn & stål**, **aluminium**, väte.
**Utanför CBAM helt:** koppar/mässing (kap. 74), plast (kap. 39), färdiga maskiner/fordon (avd. XVI & XVII).

---

## 2. 💰 Den mest lönsamma gränsdragningen i hela matrisen: 7325 vs 7326

> **CN 7325 ("andra gjutna varor av järn eller stål") ligger UTANFÖR CBAM.**
> **CN 7326 ("andra varor av järn eller stål") ligger INNANFÖR CBAM.**

**Samma fysiska konsol, samma kund, samma ritning — bär CBAM-skyldighet eller ingen alls, beroende på om den klassas som *gjuten* eller som *smidd/stansad/bearbetad*.**

ESMA gör **både gjutning och smide och stansning**. Det betyder att gränsdragningen 7325/7326 löper rakt igenom deras katalog.

**Bordic-insats:** identifiera alla artiklar i 7326 som i själva verket är gjutna ⇒ 7325 ⇒ **ut ur CBAM-populationen permanent** (och lägre tull: ~1,7–2,7 % mot 2,7 %).

**Detta är den enskilt mest konkreta scope-städningsposten och den är helt laglig.**

---

## 3. 💰 Klassificering avgör CBAM-skyldighet — "parts of general use"

**Ingenting i avdelning XVI (kap. 84–85, maskiner/el) eller avdelning XVII (kap. 87, fordon) ligger i CBAM bilaga I.**

⇒ **En komponent klassad som maskindel är CBAM-fri. Identiskt föremål klassat som vara av järn/stål under 73xx är CBAM-pliktigt.**

Men riktningen är låst av lag, inte valfri:

**Anm. 2 till avd. XV** definierar *delar med allmän användning*: bl.a. varor enligt **7307, 7312, 7315, 7317 och 7318** samt fjädrar enligt 7320.
**Anm. 1 g till avd. XVI** och **anm. 2 b till avd. XVII** **utesluter** dessa uttryckligen från kap. 84/85 respektive 87.

⇒ **En bult som sitter i en växellåda är inte en växellådsdel. Den är 7318. Alltid.**
⇒ **Omvänt:** en bearbetad detalj som **inte** är en del med allmän användning ska enligt anm. 2 b till avd. XVI klassas till maskinens nummer — och lämnar då kap. 73 **legitimt, och därmed CBAM**.

**Bordic-insats:** gå igenom (a) artiklar i 84/85/87 som borde vara 7318/7320 (risk: felaktigt CBAM-fria i dag ⇒ underdeklaration) och (b) artiklar i 7326 som är identifierbara maskindelar (möjlighet: legitimt ut ur CBAM).

**Detta är ett tveeggat svärd och måste presenteras så.** Samma genomgång som hittar överbetalning hittar underbetalning. Se §7.

---

## 4. 💰 BKB — ett instrument, tre utfall samtidigt

**Ett bindande klassificeringsbesked (BKB / BTI) låser KN-numret. Men eftersom CBAM:s omfattning definieras av KN-nummer — inte av produktbeskrivning — låser ett BKB samtidigt:**

1. **tullsatsen**
2. **antidumpningsstatusen**
3. **CBAM-skyldigheten (in eller ut)**

| Fakta om BKB | Uppgift |
|---|---|
| Rättslig grund | **Art. 33 UCC** (förordning 952/2013) |
| Ansöks hos | **Tullverket**, via EU:s Customs Trader Portal |
| Handläggning | Accept/avslag inom **30 dagar**; beslut inom **120 dagar** efter accept |
| Giltighet | **3 år**, bindande för tullmyndigheterna i **hela EU** |
| Motsvarighet för ursprung | **BUI / Binding Origin Information** — 3 år, rätt instrument för omlokaliserad asiatisk leverantör |
| EBTI | EU:s publika databas över **andras** anonymiserade BKB — övertygande men inte bindande för icke-innehavare |

> **Detta är Bordics starkaste "vi vet vad vi gör"-kort.** Ingen CBAM-mjukvara säljer BKB. Ingen speditör föreslår det. Det är ett hantverksmässigt trade-operatörsdrag.

---

## 5. Ursprung, preferenser och den bortglömda pengaposten

| Ursprung | Preferens? | Instrument | Kommentar |
|---|---|---|---|
| **Kina** | ❌ Ingen | – | **Ingen GSP sedan 2015-01-01**, inget frihandelsavtal ⇒ full MFN |
| **Schweiz** | ✅ **Tullfritt** | EUR.1 / ursprungsdeklaration (godkänd exportör >€6 000), PEM | **Även CBAM-undantaget (bilaga III)** |
| **Japan** | ✅ **EU–Japan EPA** | Ursprungsförsäkran | 💰 **Krävs den? Om inte — överbetalning varje dag** |
| **Taiwan** | ❌ Ingen | – | Full MFN |
| **Turkiet** | ✅ Tullunion | A.TR | |
| Norge/Island/Liechtenstein | ✅ EES | | Även CBAM-undantagna |

### 💰 Retroaktiv preferensåtervinning
Ett ursprungsintyg kan utfärdas **i efterhand** ("issued retrospectively") och godtas i regel **upp till 2 år** efter export. Återbetalningskravet kan gå **3 år** bakåt (UCC art. 117/121).
⇒ **Har ESMA importerat japanskt utan att åberopa EPA, ligger det pengar på bordet — retroaktivt.**

### ⚠️ Asymmetrin i leverantörsdeklarationer
Faller en långtidsleverantörsdeklaration vid verifiering (INF 4), betalar **IMPORTÖREN** tullen retroaktivt i upp till 3 år **plus ränta** — inte leverantören. Risken är helt ensidig och ligger hos ESMA.

### Melt-and-pour
Ursprung/kvalificering bestäms av **var stålet smältes och göts**, oavsett efterföljande bearbetning.
⇒ Ett fästelement kallformat i Vietnam av kinesiskt smält valstråd är **kinesiskt stål** i melt-and-pour-mening.
**Icke-preferentiellt ursprung** (UCC art. 60.2) avgörs av sista väsentliga bearbetning; listregler i bilaga 22-01.

---

## 6. Regelverk utanför CBAM — den bredare exponeringen

| Regelverk | Träffar ESMA? | Tidpunkt | Kommentar |
|---|---|---|---|
| **Sanktioner — art. 3g, förordning 833/2014** | ✅ **JA, GÄLLER REDAN** | **Löpande nu** | 🚨 Importör måste **bevisa** att järn-/stålvaror bearbetade i tredjeland **inte** använt ryskt insatsmaterial. **En melt-and-pour-liknande bevisbörda som redan binder ESMA i dag.** Ofta helt förbisett. |
| **REACH art. 33 + SCIP** | ✅ Ja | Löpande | SVHC >0,1 % w/w i vara. **Bly** i automatstål/mässing, **Cr(VI)** i passivering |
| **PFAS universell begränsning** | ⚠️ Sannolikt | RAC-yttrande **mars 2026** | Zinklamell/friktionsbeläggning. **ESMA har själva publicerat om PFAS** |
| **Ny stålförordning (EU) 2026/1384** | ⚠️ Ej i dag | **Gäller sedan 2026-07-01** | 26 kategorier, **50 % utomkvotstull**, melt-and-pour. Fästelement sannolikt **utanför** — men scope-review **31 dec 2026** och nedströms **30 juni 2027** |
| **CBAM nedströms** | ⚠️ Kommande | **2028-01-01** | COM(2025) 989, ~180 produkter, rådsposition 2026-06-12 |
| **AD-åtgärder fästelement, utgång** | ✅ Ja | **~17–18 feb 2027** | 🚨 5-årsutgång om ingen översyn inleds. **6 månader bort** |
| **CBAM-deklarant** | ✅ Ja | Ansökan **31 mars 2026 (passerad)** | Handläggning 120–180 dagar |
| **CSRD/CSDDD** | ❌ Ej direkt | | Men **indirekt via kundkrav** — se H12 |
| **PPWR** | ⚠️ Delvis | från aug 2026 | Emballage från Asien |
| **CE / maskinförordning 2023/1230** | ⚠️ Delvis | **jan 2027** | Om delvis fullbordad maskin |
| **CPR — EN 14399 / EN 15048** | ⚠️ Om konstruktionsskruv | Löpande | CE-märkning av bultförband — ofta missat hos fästelementdistributörer |
| **EUDR** | ⚠️ Endast träemballage/pallar | | Kontrollera |
| **GPSR** | ❌ Sannolikt ej | | B2B-komponenter |

---

## 7. ⚠️ Tveeggat: varje genomgång kan hitta underbetalning

**UCC art. 117** — återbetalning av **för mycket** debiterad tull, **3 år** bakåt.
**UCC art. 105** — myndighetens **efterkrav** för **för lite** betald tull, **samma 3 år** (längre vid brott).
Sverige tillämpar dessutom **tulltillägg** vid oriktig uppgift — men **självrättelse** ger normalt lindring.

> **Detta måste sägas till John innan han frågar.** Att presentera en klassificeringsgenomgång som ren uppsida är oärligt och han kommer att genomskåda det.
> **Rätt formulering:** *"Det här är tveeggat. Samma genomgång som hittar pengar tillbaka kan hitta att något legat fel åt andra hållet. Skillnaden är att om ni hittar det själva och rättar är det en självrättelse med lindring — hittar Tullverket det vid revision är det tulltillägg. Det är därför man gör det frivilligt, och det är därför man gör det nu."*

**Det argumentet är starkare än ren besparing, för det säljer på riskkontroll — och riskkontroll är vad en delägare köper.**

---

## 8. Tullvärde — den tredje, förbisedda sömmen

**EU har ingen "first sale for export"-regel.** Köps varan genom ett **närstående handelsbolag** är tullvärdet i regel **det pris EU-importören betalar** — inte fabrikspriset.

🚨 **ESMA har ett eget dotterbolag: ESMA HONG KONG LTD.**
Koncernomsättning 420,1 MSEK vs svenska bolaget 354,3 MSEK ⇒ **~66 MSEK gap**, sannolikt HK-armen.

⇒ Går varan **fabrik → ESMA Hong Kong → ESMA Sverige**, beräknas tullen sannolikt på **HK-priset inklusive HK-marginal** — inte fabrikspriset.
⇒ **Det höjer tullvärdet, tullen, eventuell antidumpningstull och CBAM-underlagets värdedel.**

Vidare: **inköpsprovision ingår inte** i tullvärdet medan **försäljningsprovision ingår**; EU-transport efter införselplatsen ska räknas av.

**Detta är en materiell, närstående-transaktionsfråga inne i deras egen koncern som nästan garanterat aldrig granskats ur tullvärdesperspektiv.** Fråga varsamt — det gränsar till internprissättning.
