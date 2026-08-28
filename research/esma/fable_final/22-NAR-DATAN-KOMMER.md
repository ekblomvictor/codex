# NÄR DATAN KOMMER — operativ körlista
**Utlösare:** John Nyman (ESMA Försäljnings AB) svarar på uppföljningsmejlet med de sex fälten för EN artikel: artikelnummer · KN/TARIC-nummer · ursprungsland · årsvolym · tullvärde · tullförfarande/destination.
**Löfte som ska hållas:** gratis ensidig exponeringsanalys inom en vecka från mötet (fre 2026-08-28), dvs. **senast fre 2026-09-04**. Sidan vidarebefordras till ESMA:s tullombud — den ska överleva expertgranskning.
**Alla tider nedan räknas från att mejlet landar (T+0).**

---

## T+0h — Bekräfta mottagandet (inom en timme, max samma dag)

- [ ] Skicka kvittensen. Inga siffror, ingen analys, inget nytt löfte utöver det redan givna.

**Utkast, 2 rader:**
> Hej John, tack — jag har allt jag behöver. Du får ensidan senast [veckodag, datum — sätt en dag FÖRE fredagens deadline].
> /Victor

- [ ] Om något fält saknas eller ser konstigt ut: skicka ÄNDÅ kvittensen först — rimlighetskontrollen (nästa steg) avgör om en kontrollfråga behövs, och den bakas då in i ETT separat mejl, inte i kvittensen.

---

## T+0h — Rimlighetskontroll INNAN någon räkning börjar (grind, 15 min)

**Regel: ser något konstigt ut — FRÅGA, gissa aldrig. En (1) samlad kontrollfråga, inte fem separata mejl.**

| Kontroll | Rött ljus om | Konsekvens om fel |
|---|---|---|
| **KN-nr vs benämning** | Koden börjar inte på 7318 (eller 7616 vid aluminium); rostfritt i benämningen men koden är en icke-rostfri undernummerrad (eller tvärtom); "mutter" men koden är inte 7318 16; "bricka" men inte 7318 21/22 | Fel AD-scope, fel CBAM-schablon — hela sidan fel |
| **Huvudlös skruv?** | Benämning tyder på pinnskruv/stoppskruv/gängstång-typ men koden är inte 7318 15 42/48 — eller tvärtom | Fel AD-regim: huvudlösa har EGEN ny AD 54,7–72,3 % (IR 2025/2153), inte spannet 22,1/39,6/86,5 % |
| **Ursprungsland vs AD** | Ursprung ≠ Kina men John förväntar sig AD-rader; Taiwan/Japan har ingen AD på fästelement | AD-scenarierna ska då UT ur sidan, inte visas med 0 |
| **Tullvärde vs volym** | Implicit pris = tullvärde/årsvolym hamnar utanför ca 0,5–20 EUR/kg för fästelement (typiskt Kina-spann ~1–3 EUR/kg) | Sannolikt ton/kg-fel eller SEK/EUR-fel — alla kostnadsrader skalar fel |
| **Tullförfarande/destination** | Otydligt om artikeln övergår till fri omsättning (4000) eller går i transit/tullager för återexport | CBAM och tull utgår bara vid övergång till fri omsättning — återexportandelen ändrar hela exponeringen |
| **Årsvolym enhet** | Volym angiven i styck utan styckvikt, eller i "pall/kartong" | CBAM räknas per ton — utan ton ingen CBAM-rad |

**Utkast kontrollfråga (anpassa hakparenteserna, EN fråga per mejl-princip — men samla alla avvikelser i samma mejl):**
> Hej John, en snabb kontroll innan jag räknar: [KN-numret 7318 xx xx avser normalt (beskrivning), men benämningen "(Johns benämning)" låter som (annan varutyp) — vilket stämmer?] / [tullvärdet delat med volymen ger ca X kr/kg, vilket ligger utanför det normala — är volymen i ton eller styck?]. Jag frågar hellre än gissar i ett underlag som er speditör ska granska.
> /Victor

- [ ] Väntar vi på svar: klockan pausar för kalkylen, men INTE för deadline — påminn dig själv T+24h om svar uteblir.
- [ ] Saknas bara **tullvärde**: räkna hela sidan i **kr/ton respektive EUR/ton** i stället för årstotal och skriv det uttryckligen — fråga inte om det är enda luckan.

---

## T+0–2h — De fem uppslagen (kör mot kalkylbladet/ensides-mallen i denna serie, fil 20/21)

Fasta värden som redan är verifierade (tre granskningsrundor — omvärdera inte): CBAM-faktor 2,5 % (2026) → 48,5 % (2030) → 100 % (2034); certifikatpris Q1 2026 = 75,36 EUR, Q2 = 75,28 EUR; schablonpåslag +10 % 2026 / +20 % 2027 / +30 % 2028 (IR 2025/2621, rättad genom IR 2026/1740 med retroaktiv verkan från 1 jan 2026 — påslaget ligger REDAN INNE i de publicerade 2026-tabellerna, lägg inte på det två gånger).

1. **[ ] Konventionell tullsats (TARIC)** för Johns exakta 8/10-siffriga kod.
   Förväntat: **3,7 %** — bekräftat för hela rubrik 7318 (inkl. 7318 15 42/48, 7318 16, 7318 22 00). Källrad: "EU TARIC / KN 2026, bilaga I till förordning (EEG) 2658/87".
   Aluminium (7616 10 00): ~6 % är EJ omverifierat — slå upp i TARIC eller skriv `[KONTROLLERA I TARIC]`, aldrig en gissad siffra.

2. **[ ] AD-scope + sats** mot art. 1.1 i IR (EU) 2022/191 (konsoliderad 02022R0191, 29.7.2025, ändrad genom IR 2026/1785 och 2026/1788 av 23 juli 2026).
   - I scope: skruv/bult med huvud, träskruv, självgängande, brickor — ursprung Kina, ej rostfritt.
   - UTANFÖR: rostfritt · franska träskruvar (coach screws) · räls-/järnvägsskruv · **fristående muttrar (7318 16)** — muttrar bara när de kommer MED sina skruvar.
   - **OBS, ändrat läge sedan 05-DONT-SAY skrevs: det finns INGET ≤6 mm-undantag för svarvad skruv i 2022/191** — den formuleringen hör till gamla 91/2009 (och UK AD2108). Små diametrar ligger fullt inne i spannet. Skriv aldrig in det undantaget; uppdatera 05-DONT-SAY p. "svarvad skruv" till LÖST.
   - Scenariospann: **22,1 % (Jiangsu Yongyi) / 39,6 % (samarbetande) / 86,5 % (övriga)**. Har John TARIC-tilläggskod ur egna deklarationer: använd den exakta satsen i stället för spann (22,1/46,1/48,8/39,6/86,5).
   - Huvudlös skruv 7318 15 42/48: byt regim till **IR (EU) 2025/2153, 54,7–72,3 %**.

3. **[ ] CBAM-schablonvärde** för exakt 8-siffrigt KN-nr + ursprungsland — ur Kommissionens Excel på CBAM-sidan (bilaga I, IR 2025/2621 i lydelse enligt IR 2026/1740).
   Detta är rundans enda kvarstående lucka: exakt Kina-värde för 7318 15 kunde inte hämtas (källor blockerade). Går Excel/EUT-bilagan inte att nå före utskick: ange **intervall 3,9 (centralt) – 6,6 (konservativt tak) tCO2e/ton inkl. påslag**, märkt *"sekundärkälla — exakt värde per 8-siffrigt KN-nr hämtas ur bilaga I till IR 2025/2621, rättad genom IR 2026/1740"* — eller `[KONTROLLERA I KOMMISSIONENS EXCEL]`. **Aldrig 3,167 — det är råstål/slab, inte färdiga fästelement.**
   Rimlighetsankare om ombudet trycker: Vietnam 7318 15 88 = 3,025; hela 7318 15-spannet 1,37–8,23 över 33 länder.

4. **[ ] Certifikatpris för innevarande kvartal.** Q1/Q2 ovan är låsta; Q3 2026-siffran var inte publicerad/verifierad per 2026-08-28 — slå upp eller räkna på Q2 (75,28 EUR) med fotnot *"senast publicerade kvartalspris"*. `[KONTROLLERA aktuellt kvartalspris]` om osäkert.

5. **[ ] Färskhetskoll AD-status (5 min sökning).** Per 2026-08-28: utgångsdatum **18 feb 2027** bekräftat (tillkännagivande i EUT C-serien 29 maj 2026 — **skriv INTE ett specifikt C/2026/xxxx-nummer**, det är overifierat); ingen översynsbegäran (EIFI) rapporterad; frist ~18 nov 2026. Kolla om något hänt sedan dess innan sidan låses.

**Sanity-ankare för kalkylen (2026 är liten, 2030 är poängen):**
2026: schablon × 2,5 % × certpris ≈ 3,9 × 0,025 × 75,36 ≈ **~7 EUR/ton** (tak ~12). 2030: × 48,5 % ≈ **~143–241 EUR/ton** vid konstant certpris. Hamnar kalkylbladet långt från detta per ton — leta fel innan något skickas.

---

## T+2–4h — Fyll mallen + självgranskning

- [ ] Fyll ensides-mallen: tull + CBAM **2026 och 2030**, AD-spannets tre scenarier som egna rader, källa på VARJE rad (förordning + artikel + åtkomstdatum), och märkningen **"Samtalshypotes — ej klassificeringsbesked"** synlig på sidan.
- [ ] Fotnot på 2030-AD-kolumnen: *"Åtgärderna löper ut 18 feb 2027 om ingen översynsbegäran inkommer (frist ~18 nov 2026); historiskt har unionsindustrin begärt och fått förlängning, och tullarna gäller under pågående översyn. Per 2026-08-28 är ingen begäran offentligt rapporterad."*
- [ ] AD-källraden: *"IR (EU) 2022/191, art. 1.1 (konsoliderad 29.7.2025), ändrad genom IR 2026/1785 och 2026/1788 (23 juli 2026)"*.

**Självgranskning mot DONT-SAY — sidspecifik dödslista (varje punkt bockas av):**
- [ ] Inget ≤6 mm-undantag nämnt (finns inte i 2022/191 — att citera det fäller sidan hos ombudet).
- [ ] Inte 3,167 tCO2e/t för fästelement (slab-värde).
- [ ] Inget påhittat C/2026-nummer, inget påhittat schablonvärde, ingen gissad tullsats — luckor = `[KONTROLLERA ...]`-platshållare, aldrig siffra.
- [ ] Påslaget +10 % inte dubbelräknat (ligger redan i publicerade 2026-schabloner).
- [ ] Konservativa intervall, sekundärkällor märkta som sekundärkällor.
- [ ] Ingen referenskund vid namn, inga "vi har sparat X", inga juridiska garantier ("håller i revision").
- [ ] Rostfritt/muttrar/coach screws/järnväg korrekt hanterade om Johns artikel tangerar dem.
- [ ] Om ursprung ≠ Kina: inga AD-rader alls.

**Ribban:** läs sidan som ESMA:s tullombud: *varje siffra ska gå att spåra till förordning eller TARIC, varje osäkerhet ska vara skyltad.* Ett enda ospårbart tal och Bordics trovärdighet — hela affären — åker ut med det. Hellre en ärlig platshållare än en snygg gissning.

---

## T+4h — Skicka (samma dag som kalkylen blir klar, aldrig efter deadlinedagen)

- [ ] PDF:a ensidan (filnamn: `ESMA_exponeringsanalys_[artikelnr]_[datum].pdf`), bifoga, skicka till John. **Cc Magnus endast om John sa ja till det i mötet — annars föreslå honom i mejlet i stället.**

**Utkast följebrev, 3 rader:**
> Hej John, här är ensidan för [artikelnr]: tull + CBAM för 2026 och 2030, inklusive spannet för antidumpningsscenarierna, med källa per rad. Den är märkt samtalshypotes — skicka den gärna till er speditör, den är byggd för att granskas. Ska vi ta 30 minuter nästa vecka och gå igenom vad den betyder för fler artiklar — ta gärna med Magnus? Föreslå två tider som passar.
> /Victor

---

## T+4h — Efterlogg (10 min, direkt efter skickat)

- [ ] Logga i 06-VERIFIERINGSLOGG.md: datum skickat · artikel/KN/ursprung · vilka värden som användes (tullsats, schablonvärde + källstatus, certpris + kvartal, AD-scenario/tilläggskod) · kvarvarande `[KONTROLLERA]`-platshållare · exakt vad som utlovades i följebrevet.
- [ ] Uppdatera 05-DONT-SAY: ≤6 mm-raden → LÖST (undantaget finns ej i 2022/191).
- [ ] Sätt påminnelse **T+3 arbetsdagar**: inget svar → kort nudge med de två mötestiderna igen.
- [ ] Om ombudet återkommer med invändningar: svara med källa, aldrig med försvar — en korrigerad v2 av sidan inom 24h slår varje bortförklaring.
