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

- [ ] E-mail kontaktowy `kontakt@kardioplaner.example`. Miejsca: stopka i CTA `index.html`, `privacy.html`, `terms.html`. TLD `.example` jest zarezerwowany i nie dostarcza poczty.
- [ ] Tożsamość wydawcy `[imię i nazwisko lub nazwa]` oraz `[adres]`. Miejsca: `privacy.html` sekcja 1, `terms.html` sekcja 1.
- [ ] Ceny i opis planów, jeśli różnią się od ustaleń.

## A11y

Semantyczny HTML, kontrast tekstu AAA, skalowalny font, widoczny focus. Bez JavaScriptu i bez CDN.
