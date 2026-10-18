# eremita.si

Mirna, informativna osebna stran: kdo sem in seznam mojih spletnih projektov. Čist HTML in CSS, brez ogrodij, brez gradnje, brez piškotkov in sledilnikov. JavaScripta ni.

## Datoteke

- `index.html` – domača stran
- `igre/index.html` – podstran Igre
- `style.css` – skupen slog
- `fonts/` – self-hostane pisave (woff2): Newsreader, Figtree, IBM Plex Mono (vse SIL Open Font License 1.1, vir: Fontsource)
- `favicon.svg`, `robots.txt`, `sitemap.xml`
- `CNAME` – vsebuje `eremita.si` (GitHub Pages)

## Še odprto

Vse, kar je v oglatih zadevah, je vidni placeholder. Poiščeš jih z `grep -rn "\[DOMENA\]\|\[DOPOLNI\]\|\[E-NASLOV\]" --include=*.html .`. Pri `[DOMENA]` zamenjaj tako besedilo kot `href="[DOMENA]"`.

## Objava na GitHub Pages

1. V repozitoriju: Settings → Pages → Source: *Deploy from a branch*, veja `main`, mapa `/ (root)`.
2. Datoteka `CNAME` je že v korenu. V Pages nastavitvah naj se izpiše `eremita.si`.
3. Pri registrarju nastavi DNS:
   - štirje `A` zapisi za `@` (eremita.si): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` za `www` → `<github-uporabnik>.github.io`
   - po želji še `AAAA` za `@`: `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
4. Počakaj na propagacijo DNS (minute do nekaj ur), nato v Settings → Pages vklopi *Enforce HTTPS*. Potrdilo se izda samodejno.
