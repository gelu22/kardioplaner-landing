# kardioplaner-landing

Publiczny landing KardioPlaner PRO. Służy jako strona pod weryfikację LemonSqueezy (KYC) oraz jako adres produktu dla klientów.

To repo zawiera **tylko** stronę statyczną. Kod aplikacji żyje w osobnym folderze projektu (ADR-006).

## Zawartość

- `index.html` — landing: opis produktu, plany i ceny, kontakt.
- `privacy.html` — polityka prywatności.
- `terms.html` — regulamin.
- `.nojekyll` — wyłącza przetwarzanie Jekyll na GitHub Pages.

## Deploy

GitHub Pages z gałęzi `main` i katalogu `/`. Każdy commit na `main` publikuje się automatycznie.

```bash
git add . && git commit -m "..." && git push
```

## Do podmiany przed wysłaniem KYC

- [ ] E-mail kontaktowy `kontakt@kardioplaner.example` (miejsca: stopka `index.html`, `privacy.html`, `terms.html`).
- [ ] Ceny i opis planów, jeśli różnią się od ustaleń.
- [ ] Nazwa administratora danych w `privacy.html`.

## A11y

Semantyczny HTML, kontrast tekstu AAA, skalowalny font, widoczny focus. Bez JavaScriptu i bez CDN.
