# Aktualizace dat
```bash
python3 tools/penshop/fetch_pages.py urls.txt raw/pages                 # šetrné stažení (4 paralelně, cache)
python3 tools/penshop/parse_shop.py shoptet raw/pages raw/parsed.json     # parsování
python3 tools/penshop/build_catalog.py raw/parsed.json penshop tools/penshop/config.json
HERO_ROTATE=1 python3 tools/penshop/make_hero.py penshop <id produktu> ... # výřezy per (otočené na výšku)
```
Potřeba: Python 3, Pillow, BeautifulSoup4, lxml, curl.
