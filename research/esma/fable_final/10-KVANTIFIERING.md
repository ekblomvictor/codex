# Kvantifieringsmodell — formler, verifierade indata, försiktiga intervall
**Fable 2026-08-24 · [K] = källbelagd, [A] = antagande som ersätts med ESMA-data. 1 EUR ≈ 11 SEK [A].**

## Verifierade indata
| Parameter | Värde | Källa |
|---|---|---|
| CBAM-certifikatpris | **€75,36 (Q1-26) / €75,28 (Q2-26)**; kvartalsvis 2026, veckovis 2027 | Kommissionen [K] |
| CBAM-faktor | **2,5 / 5 / 10 / 22,5 / 48,5 / 61 / 73,5 / 86 / 100 %** (2026→2034) | [K] |
| ⚠️ Prognosförbehåll | ETS Phase 5-**förslag**: 15 % fri tilldelning åter från 2028, utfasning till 2038 | [K, ej lag] |
| Påslag på defaultvärden | **+10 % 2026 / +20 % 2027 / +30 % 2028+** (järn/stål, alu, cement) | IR 2025/2621 [K] |
| Defaultvärden | **13 566 land- och produktspecifika** i 2025/2621, **rättade av IR 2026/1740 (retroaktivt 1/1 2026)** — exakt 7318/Kina-värde hämtas ur bilagorna | [K] |
| Benchmarks stålrutt | BF-BOF 1,370 · DRI 0,481 · EAF 0,072 tCO₂e/t · kinesiskt slab-default 3,167 (**gäller EJ färdiga fästelement**) | [K] |
| Realistiskt default/actual för kinesiskt fästelement | **~1,3×** (endast ~10 % av Kinas stål EAF) | [K, härledd] |
| Kinas ETS | Stål/cement/alu sedan mars 2025, ~CNY 67 ≈ €8,5/t; art. 9-avdrag ej säkrat | [K] |
| Tull 7318 | ~3,7 % MFN; Kina utan preferens | [K] |
| AD Kina fästelement | 22,1–48,8 / 39,6 / **86,5 %** (2022/191; 2026/1788-ändring okontrollerad) | [K] |
| ESMA-volym | "flera tusen ton/år, ~50 % export"; oms. 354 MSEK; inköp ~250–265 MSEK | esma.se + register [K] |

## Formlerna
```
F1  CBAM-kostnad/år  = Σ ton_i × EF_i × P_cert × faktor_år − koldioxidpris_ursprung
F2  Värde av actuals = ton × (EF_default×påslag − EF_actual) × P_cert × faktor_år   [per fabrik!]
     Beslutsregel: jaga actuals om F2 (NPV 2026–34) > verifieringskostnad/fabrik — annars INTE
F3  Klassificeringsvärde = tullvärde × Δsats  (+ återbetalning ≤3 år; MINUS efterkravsrisk åt andra hållet)
F4  Förfarandevärde  = ton_ut_ur_EU × värde/ton × (tullsats + AD-sats) + ton × EF × P_cert × faktor
     ⚠️ Endast framåt — ingen drawback
F5  Tröskeln         = om Σ nettomassa CBAM-varor i fri omsättning < 50 t/år ⇒ skyldigheten faller
     (återexport under förfarande räknas inte in)
F6  Kassaflöde       = 2026 års kostnad betalas tidigast feb 2027; deklaration 30/9 2027
```

## Räkneexempel (mekanik-illustration, EJ prognos — antaganden [A] byts i steg 0/1)
Antag: 4 000 t genom Spånga [K-intervall], 1 360 t asiatiskt i CBAM-scope [A], 45 000 SEK/t [A], 400 t lämnar EU [A].

**CBAM (default, färdigvara ~3,6 tCO₂e/t [A]):** 1 360×3,6×€75 = €367k ofaktoriserat →
**2026: ~€9,2k ≈ 100 kSEK** · 2030 (48,5 %): ~€178k ≈ **2,0 MSEK** · 2034: ~€367k ≈ 4,0 MSEK.
*Säg 2026-siffran högt. Säg 2030 med förbehållet: "om utfasningen står sig — det ligger ett förslag om att mildra den".*

**Actuals-värde (1,3×):** Δ≈0,8 tCO₂e/t ⇒ 2026: ~22 kSEK (**irrationellt att jaga**) · 2030: ~435 kSEK/år · koncentrerat till få fabriker. Rutt-skattning gratis via EN 10204-intygen hos E&K **innan** någon kontaktas.

**Förfarande (F4):** 400 t × 45 kSEK = 18 MSEK tullvärde ⇒ **~0,67 MSEK/år** vid enbart 3,7 % — *citera "0,5–0,8"*. AD-scenarier nämns kvalitativt, aldrig som siffra.

**Klassificering (F3):** helt beroende av registrets kvalitet — UNKNOWN tills data. Ram: 1 %-enhet fel på 150 MSEK tredjelands-tullvärde [A] = 1,5 MSEK/år + retro.

## Var pengarna finns — sammanfattning
| Spår | 2026 | 2030 | Bevistid | Säkerhet |
|---|---|---|---|---|
| Förfarande/återexport | **0,5–0,8 MSEK** | + CBAM-delen | 2–4 v | Hypotes, testbar med 1 fråga |
| Massa + scope-städning | korrigerar allt | ackumulerar | **1–2 v** | **Garanterbar** |
| AD rätt sats/undantag | 0 → stort | samma | 3–5 v | Hypotes, mätbar |
| CBAM-certifikat | **~0,1 MSEK** | ~2 MSEK | — | Hög |
| Actuals | ~0 (**avstå**) | 0,4–0,9 MSEK/år | 2027+ | Prioriteringsfråga |
