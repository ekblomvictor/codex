# 12 rankade hypoteser om ESMA:s importflöden och produktfamiljer
**2026-08-24 · Bordic**

Rankade efter **(sannolik smärta × ekonomiskt värde × brådska × Bordics rätt att vinna × bevistid)**.
Varje hypotes: bevis → smärta → Bordics insats → ekonomisk mekanism → confidence → **exakt första fråga till John** → data som krävs.

**Läsning av confidence:** avser sannolikheten att hypotesen är *materiellt sann för ESMA*, inte att mekanismen finns (mekanismerna är verifierade).

---

## H1 · Återexportflödet betalar tull och CBAM det inte behöver betala
**Confidence: 62** — *högsta värde per bevistimme i hela listan*

**Bevis [K, PRIMÄR]:** esma.se: logistikcentret i Spånga hanterar *"flera tusen ton styckegods årligen, varav ca 50 % exporteras"*, störst till **Nord- och Sydamerika samt norra Europa**. ESMA levererar till 39 länder. Rättsläget: varor under **tullager/aktiv förädling** som återexporteras utlöser **varken tull, antidumpningstull eller CBAM** (Tullverket; EU-kommissionens CBAM-vägledning).

**Smärta:** Om godset går i fri omsättning vid ankomst till Spånga och sedan exporteras till USA/Brasilien/Norge/UK, betalar ESMA tull (och ev. AD-tull) på varor som aldrig konsumeras i EU. Pengarna är **oåterkalleligt förlorade** — EU har ingen amerikansk drawback.

**Bordics insats:** Kartlägg import→lager→exportdestination per artikel i 12 månader. Kvantifiera den andel som lämnar EU. Räkna besparingen vid tullager respektive aktiv förädling. Ta fram ansökningsunderlag till Tullverket.

**Ekonomisk mekanism:** `ton_återexport × värde/ton × (3,7 % + ev. AD-sats)` + bortfallen CBAM. Vid 408 ton och 45 kSEK/ton: **0,68 MSEK/år enbart på ordinarie tull**; **7–16 MSEK/år om AD-belagt**.

**⚠️ Motbevis att ta på allvar:** ESMA säljer *"dokumenthantering i samband med import/export"* — de kan mycket väl redan ha tullager. Ställ frågan öppet.

**Exakt första fråga:**
> *"Av de ungefär femtio procent som går på export igen från Spånga — hur mycket av det lämnar EU, och går det ut från fri omsättning eller från ett tullagerförfarande?"*

**Data som krävs:** Exportdestinationer per artikel 12 mån; tullförfarandekod på importdeklarationerna; ev. befintliga tulltillstånd.

---

## H2 · Antidumpningsexponering på kinesiska fästelement
**Confidence: 70** att exponering finns; **45** att den är felhanterad

**Bevis [K]:** Förordning (EU) 2022/191 lägger definitiv antidumpningstull på vissa järn-/stålfästelement från Kina: **86,5 % residual**, **39,6 %** för samarbetande listade, **22,1–48,8 %** för tre namngivna. Berörda KN-nummer inkluderar 7318 12 90, 7318 14 91, 7318 14 99, 7318 15 58 m.fl. Ändrad genom **(EU) 2026/1788 (2026-07-23)**. ESMA:s största produktfamilj **är** fästelement och de köper från **Kina**.

**Smärta:** Skillnaden mellan 86,5 % och 39,6 % (eller 22,1 %) är **enorm** och avgörs av **vilken producent varan faktiskt kommer från** — inte vilket handelsbolag som fakturerar. Köper ESMA via handelsbolag/E&K-samlastning finns en reell risk att residualsatsen tillämpas där en producentspecifik sats vore korrekt, eller omvänt att fel producent anges.

**Bordics insats:** Matcha varje kinesisk fästelementartikel mot **faktisk tillverkare**, kontrollera mot bilagan i 2022/191, verifiera aktuella satser i TARIC efter 2026/1788, säkra dokumentation.

**Ekonomisk mekanism:** `tullvärde × Δ AD-sats`. På 5 MSEK kinesiskt fästelementvärde är skillnaden 86,5→39,6 **2,3 MSEK/år**. Felaktigt *för låg* sats = efterbeskattning + tulltillägg. Felaktigt *för hög* = återbetalning 3 år bakåt.

**Exakt första fråga:**
> *"Vilka av era kinesiska fästelementartiklar ligger under antidumpning i dag, och är satsen kopplad till en namngiven producent eller till residualsatsen?"*

**Data:** Artikellista kinesiska fästelement m. KN-nr, tillverkarnamn, AD-kod i deklaration, TARIC-utfall.

---

## H3 · Scope-städning: hur många artiklar ligger i CBAM som inte borde
**Confidence: 80** — *snabbast bevisbara, lägst risk*

**Bevis [K]:** **KN 7318 ligger i CBAM bilaga I sedan 2023-10-01.** **KN 7326 är endast delvis täckt** — bara vissa 8-siffriga undernummer. **Schweiz är CBAM-undantaget (bilaga III)**, Tyskland är EU. Plast (Vespel®, PUR) ligger utanför. ESMA importerar från **32 länder** med tyngdpunkt Tyskland/Schweiz **och** Asien.

**Smärta:** Ett artikelregister med tusentals rader klassade grovt på 4-siffrig nivå drar in för mycket i CBAM-populationen. Varje felaktigt inkluderad artikel kostar arbete, leverantörsjakt och (från 2029) pengar.

**Bordics insats:** Gå från 4- till 8-siffrig nivå på CBAM-populationen; skilj EU/EFTA-ursprung från tredjeland; skilj täckta från icke-täckta 7326-undernummer; ta bort plast.

**Ekonomisk mekanism:** Sänker underlaget i F1 permanent — verkar på **varje år 2026–2034**. Sänker också leverantörsjakten (färre fabriker att kontakta).

**Exakt första fråga:**
> *"När ni byggde CBAM-populationen — gjorde ni det på fyrsiffrig KN-nivå eller åttasiffrig, och plockade ni bort schweiziskt ursprung?"*

**Data:** Nuvarande CBAM-population, artikelregister m. KN + ursprungsland.

---

## H4 · Trader-vs-installation: emissionsdata som hör till fel enhet
**Confidence: 78**

**Bevis:** ESMA köper via **systerbolaget E&K i Shenzhen** som gör **samlastning av små volymer** — dvs. många små fabriker konsolideras. Kinesiska fästelementkedjor löper: valstråd → dragning → kallslagning → värmebehandling → **ytbehandling (ofta separat underleverantör)** → handelsbolag → EU-importör. CBAM:s "installation" är producenten, inte handelsbolaget.

**Smärta:** Data kan komma från handelsbolaget, från koncernen istället för anläggningen, från fel produktlinje, fel period, eller sakna **prekursorer** och **ytbehandlingssteget**. Vid verifiering 2027 faller sådan data.

**Bordics insats:** Artikel → faktisk anläggning-mappning; identifiera systemgränser; upptäck återanvända generiska emissionsfaktorer; bygg revisionsspår per fält.

**Ekonomisk mekanism:** Undviker underkänd verifiering (omtag + förseningsavgift) och undviker att ett för högt tal låses in i baslinjen inför 2029–2034.

**Exakt första fråga:**
> *"När ni fick in utsläppsdata i era två rapporter — kom talen från fabrikerna själva eller från handelsbolagen, och kunde ni se om ytbehandlingen låg innanför systemgränsen?"*

**Data:** Leverantörsmallar från rapport 1 & 2, ev. monitoring-planer.

---

## H5 · Ytbehandling — regulatorisk och klassificeringsmässig blind fläck
**Confidence: 72**

**Bevis [K, PRIMÄR]:** esma.se: *"alla typer av ytbehandlingar i Europa och Asien, från enkel förzinkning till zinklamellbehandling"*. ESMA har **själva publicerat** artikeln *"EU takes action against PFAS – Time to re-think"*. ECHA:s RAC lämnade **slutyttrande om universell PFAS-begränsning i mars 2026**.

**Smärta:** Zinklamell-system (Delta-Tone/Geomet-typ) och friktionsmodifierare har historiskt innehållit **PFAS**; passivering kan innehålla **Cr(VI)** (SVHC). Detta träffar REACH art. 33, **SCIP-anmälan till ECHA**, och kundkrav. Dessutom: ytbehandling utförd i **tredje land av underleverantör** ligger ofta utanför den emissionsdata fabriken lämnar.

**Bordics insats:** Koppla ytbehandlingsspec → kemikalieinnehåll → SVHC/PFAS-status → SCIP-skyldighet, och parallellt → CBAM-systemgräns.

**Ekonomisk mekanism:** Undviker kundstopp och omkonstruktion; ESMA har redan signalerat att de tänker på det → **låg övertygelsekostnad, hög trovärdighet**.

**Exakt första fråga:**
> *"Ni skrev själva om PFAS — har ni kartlagt vilka av era ytbehandlingar som faktiskt innehåller PFAS eller sexvärt krom, artikel för artikel?"*

**Data:** Ytbehandlingsspecar, SDS från behandlare, kundkrav.

---

## H6 · Melt-and-pour under nya stålförordningen 2026/1384
**Confidence: 50** för direkt träff nu; **85** att det kommer

**Bevis [K]:** **Förordning (EU) 2026/1384** i kraft **2026-06-25**, tillämpas **från 2026-07-01**: kvot 18,3 Mt, **50 % utomkvotstull**, **melt-and-pour-krav**, 26 varukategorier. Kommissionen ska **senast 2026-12-31** bedöma utvidgning till fler KN-nummer och **senast 2027-06-30** bedöma **nedströms stålprodukter — uttryckligen inklusive fästelement**.

**Smärta:** Fästelement ligger sannolikt **utanför** de 26 kategorierna i dag — men bedömningen pågår **nu**. Om nedströms tas in måste ESMA kunna bevisa **var stålet smältes och göts**, för varor köpta via samlastning från många små fabriker. Det är inte gjort över en natt.

**Bordics insats:** Kartlägg vilka artiklar som redan träffas; bygg melt-and-pour-bevisrutin med leverantörerna **innan** kravet utvidgas; delta i Kommissionens pågående scope-konsultation.

**Ekonomisk mekanism:** 50 % utomkvotstull är existenshotande på berörda flöden. Att ha beviskedjan klar är en **optionspremie**.

**Exakt första fråga:**
> *"Har ni någon artikel som ligger i någon av de 26 stålkategorierna sedan första juli — och kan era kinesiska leverantörer i dag visa var stålet smältes?"*

**Data:** KN-nummer mot bilagan i 2026/1384; leverantörernas materialintyg (EN 10204 3.1).

---

## H7 · "Parts of general use" — klassificeringsfällan för komponenthandel
**Confidence: 65**

**Bevis:** Anm. 2 till avd. XV i KN tvingar **delar av allmän användning** (bl.a. fästelement enl. 7318, fjädrar enl. 7320) **ut ur** maskin-/fordonskapitlen (84/85/87) och **in i** kap. 73 — oavsett vad de sitter i. ESMA säljer till fordon/medicinteknik/verkstad och levererar ofta **kundspecifika detaljer**.

**Smärta:** En kundspecifik skruv till en fordonskund klassas lätt som "fordonsdel 8708" av en speditör som ser kundens tillämpning. Fel kapitel ⇒ fel tullsats, **fel CBAM-status**, fel AD-status. Både över- och underbetalning är möjlig.

**Bordics insats:** Klassificeringsgenomgång av de artiklar som ligger i 84/85/87 och testa dem mot anm. 2; identifiera kandidater för **bindande klassificeringsbesked (BKB)** via Tullverket; sök EBTI efter jämförbara beslut.

**Ekonomisk mekanism:** `tullvärde × Δsats` framåt + återbetalning 3 år bakåt vid överbetalning. BKB låser klassificeringen och tar bort risken.

**Exakt första fråga:**
> *"Hur många av era artiklar ligger klassade i kapitel 84, 85 eller 87 — och har ni testat dem mot regeln om delar av allmän användning?"*

**Data:** Artikelregister m. KN-nr per artikel; toppen efter tullvärde.

---

## H8 · Deklarantstatus — har beslutet faktiskt kommit?
**Confidence: 55** att det finns en lucka; **95** att frågan är legitim

**Bevis [K]:** Ansökningsfrist **2026-03-31**. Naturvårdsverket handlägger svenska ansökningar; handläggning uppges **120–180 dagar**. Den som ansökt före fristen får **provisoriskt fortsätta importera** i väntan på beslut. ESMA skrev i **okt 2024** att de *"kommer att ansöka"*.

**Smärta:** Om ansökan gick in sent kan beslutet fortfarande vänta i augusti 2026. Om den inte gick in alls och import över 50 ton skett — allvarligt.

**Bordics insats:** Ingen försäljning här — **detta är en omtankefråga som bygger förtroende**. Om det finns ett problem blir Bordic omedelbart relevant.

**Ekonomisk mekanism:** Skydd av importrätten. Värdet är hela importflödet.

**Exakt första fråga:**
> *"Har ni fått ert beslut om godkänd CBAM-deklarant från Naturvårdsverket, eller ligger ni fortfarande på provisorisk rätt?"*

**Data:** Beslut/diarienummer från Naturvårdsverket.

---

## H9 · Aluminium- och kopparfästelement glöms bort
**Confidence: 58**

**Bevis [K]:** CBAM bilaga I omfattar **kap. 76 inkl. 7616** (andra varor av aluminium — inkl. skruv, bult, mutter, nit av aluminium). ESMA anger *"alla … material"* i fästelement.

**Smärta:** CBAM-arbete i verkstadsbolag fokuserar nästan alltid på stål. Aluminiumartiklar (och 7616-undernummer) glöms i populationen. Aluminium har dessutom **högre utsläppsintensitet per ton** än stål — värdet per ton är större.

**Bordics insats:** Sök artikelregistret på kap. 76; verifiera 8-siffriga undernummer mot bilaga I.

**Ekonomisk mekanism:** Fyller ett hål i deklarationen (undviker sanktion) och identifierar högvärdiga actuals-kandidater.

**Exakt första fråga:**
> *"Finns aluminiumartiklar med i er CBAM-population, eller byggdes den på stålsidan?"*

**Data:** Artikelregister filtrerat på kapitel 76 och 74.

---

## H10 · Prekursorer och skrotandel — den stora actuals-hävstången
**Confidence: 75**

**Bevis [K]:** Benchmarks **EAF/skrot 0,072** vs **BF-BOF 1,370** tCO₂e/t. Påslag på default: **+10 % 2026, +20 % 2027, +30 % 2028+**.
⚠️ Det kinesiska standardvärdet **3,167** är ett **råstålsvärde** och gäller **inte** KN 7318 — färdigvarudefault krävs (se fil 07).

**Smärta:** Spridningen mellan rutterna är stor i *råstålsledet*, men för ett färdigt fästelement är realistiskt förhållande default/actual **~1,3×** — inte 4–40×. Skälet: **endast ~10 % av Kinas råstål är EAF-baserat**, så sannolikheten att en given leverantör sitter på en lågkoldioxidrutt är låg. **Vinsten finns, men den är koncentrerad till ett fåtal leverantörer — och det är just därför prioritering är hela poängen.**

**Bordics insats:** Identifiera vilka kinesiska/taiwanesiska/japanska leverantörer som har EAF-baserad prekursor; prioritera actuals-jakt dit **value-of-information är högst** (F2), och **avstå** där den är låg.

**Ekonomisk mekanism:** `ton × (EF_default − EF_actual) × €75 × faktor`. Verifiering kostar **per anläggning** ⇒ break-even styrs av **ton per fabrik**, och break-even-tonnaget faller **~40× till 2034**.
⚠️ **Och varningen som ingen konkurrent ger:** blir verifierade actuals *sämre* än schablonen **måste de användas**. Uppskatta rutten via **EN 10204 3.1-intyg** (som E&K sannolikt redan har) **innan** någon leverantör kontaktas.

**Exakt första fråga:**
> *"Vet ni i dag vilka av era asiatiska leverantörer som kör skrotbaserat stål och vilka som kör masugn?"*

**Data:** Leverantörslista m. tonnage; materialintyg; ev. befintliga svar från rapport 1 & 2.

---

## H11 · Japan och Taiwan — förbisedda CBAM-ursprung
**Confidence: 60**

**Bevis [K, PRIMÄR]:** esma.se: *"arbetar nära många tillverkare i **Japan, Taiwan och Kina**"*. CBAM gäller **allt tredjelandsursprung** utom bilaga III (Schweiz, Norge, Island, Liechtenstein).

**Smärta:** CBAM-arbete blir ofta "Kina-projekt". Japanska och taiwanesiska leverantörer är lika omfattade men hanteras inte — och de är ofta **mer** samarbetsvilliga och har bättre data. Att missa dem är både ett compliance-hål och ett missat värde.

**Bordics insats:** Utöka populationen till JP/TW; utnyttja att dessa leverantörer typiskt svarar bättre — snabba vinster i actuals.

**Exakt första fråga:**
> *"Ingick Japan och Taiwan i era CBAM-rapporter, eller låg fokus på Kina?"*

**Data:** Ursprungsfördelning per tonnage.

---

## H12 · Kundkrav vänder CBAM från kostnad till säljkrav
**Confidence: 68**

**Bevis:** ESMA har **>200 aktiva kunder** i **medicinteknik, fordon, verkstad, energi, flyg** — inkl. *"stora globala koncerner"* **[K, PRIMÄR]**. Bufab (noterad jämförelse) driver SBTi-mål och leverantörsutsläppsdata **[K]**. Stora svenska OEM:er kräver i ökande grad produktkoldioxidavtryck (PCF) och Scope 3-data av komponentleverantörer.

**Smärta:** Om ESMA:s kunder börjar kräva PCF per artikel blir utsläppsdata en **förutsättning för att behålla affären**, inte en myndighetskostnad. Då byter budgeten ficka — från compliance till försäljning, där den är mycket större.

**Bordics insats:** Samma dataunderlag som CBAM kräver kan levereras som **kundvänd PCF-tjänst**. ESMA säljer redan dokumenthantering — detta är nästa tjänstesteg och kan **prissättas mot kund**.

**Ekonomisk mekanism:** Förvandlar en kostnadspost till en **intäkts- och differentieringspost**. Detta är den enskilt största expansionsvägen för Bordic hos ESMA.

**Exakt första fråga:**
> *"Har någon av era större kunder börjat begära koldioxiddata per artikel av er?"*

**Data:** Kundförfrågningar, leverantörsuppförandekoder, ev. PCF-krav i avtal.

---

## Rankningsöversikt

| # | Hypotes | Värde | Brådska | Bevistid | Conf. | Prio |
|---|---|---|---|---|---|---|
| H1 | Återexport under tullförfarande | ●●●●● | ●●●●● | 2–4 v | 62 | **1** |
| H3 | Scope-städning | ●●● | ●●●● | 1–2 v | 80 | **2** |
| H2 | Antidumpning kinesiska fästelement | ●●●●● | ●●●● | 3–5 v | 70/45 | **3** |
| H8 | Deklarantstatus | ●●●● | ●●●●● | 1 dag | 55 | **4** |
| H10 | Prekursor/skrot, actuals-prioritering | ●●●● | ●●● | 4–8 v | 75 | **5** |
| H7 | Parts of general use / klassificering | ●●●● | ●●● | 3–6 v | 65 | **6** |
| H4 | Trader vs installation | ●●● | ●●●● | 3–6 v | 78 | **7** |
| H12 | Kundkrav → PCF som säljargument | ●●●●● | ●● | 8–12 v | 68 | **8** |
| H6 | Melt-and-pour / stålförordningen | ●●●●● | ●●● | 4–8 v | 50 | **9** |
| H5 | Ytbehandling PFAS/Cr(VI)/SCIP | ●●● | ●●● | 3–6 v | 72 | **10** |
| H9 | Aluminium glöms i populationen | ●● | ●●● | 1 v | 58 | **11** |
| H11 | Japan/Taiwan-ursprung | ●● | ●● | 1 v | 60 | **12** |
