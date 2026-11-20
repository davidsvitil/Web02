# penShop – koncept nového e-shopu

Statický frontend (HTML + CSS + vanilla JS, bez buildu) pro penshop.cz, vizuálně inspirovaný patike.ch – stejný designový jazyk jako předchozí koncepty (tmavý rám, zaoblené plochy, plovoucí pill menu, obří „ghost“ nápisy, carousel s výřezy produktů, pozadí se přebarvuje podle barvy pera).

**Jde o neoficiální návrh** – stránka má trvalý pruh „KONCEPT“, vodoznak a `noindex`.

## Co umí
- **Katalog** – 642 produktů: pera (Kaweco, Cross…), inkousty a náplně (Iroshizuku, Sailor, Diamine), kreslení, zápisníky Leuchtturm1917 a Rhodia. Z papíru a doplňků je v náhledu jen výběr.

## Spuštění lokálně
```bash
cd penshop && python3 -m http.server 8000   # http://localhost:8000
```

## Nasazení
Settings → Pages → Source: **GitHub Actions**, pak Actions → Run workflow. Kořenový `index.html` přesměruje do `penshop/`.

## Co ještě chybí do ostrého provozu
- Platby, sklad a objednávky v reálném čase – ceny jsou snímek z 20. 11. 2026, objednávka zatím odchází e-mailem (mailto).
- Objednávka gravírování (text rytiny) – v ostré verzi jako pole v detailu produktu.
