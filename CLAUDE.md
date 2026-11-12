# CLAUDE.md

## O projekcie

Statyczna strona portfolio hostowana na GitHub Pages (repozytorium
`beereq/beereq.github.io`, publikowane z gałęzi `main`, katalog główny).

- Czysty HTML i CSS – bez frameworków, bez JavaScriptu, bez kroku budowania.
- Treść strony jest po polsku (`<html lang="pl">`).

## Struktura

- `index.html` – cała strona (jeden plik), sekcje: O mnie (`#o-mnie`),
  Umiejętności (`#umiejetnosci`), Projekty (`#projekty`), Kontakt (`#kontakt`).
- `style.css` – wszystkie style.

## Konwencje

- Miejsca do uzupełnienia przez właściciela są oznaczone `[UZUPEŁNIJ]` lub
  `[UZUPEŁNIJ: wskazówka]`. Nie wymyślaj danych osobowych – zostaw placeholder,
  jeśli treść nie została podana.
- Design: jasny, minimalistyczny, jeden kolor akcentu. Kolory, promienie
  i szerokość kontenera są zmiennymi CSS w `:root` na górze `style.css`
  (akcent: `--accent`, `--accent-dark`, `--accent-soft`). Nie dodawaj drugiego
  koloru akcentu.
- Strona musi być responsywna: siatki przechodzą w jedną kolumnę poniżej
  860px, a poniżej 640px nagłówek układa się w dwóch wierszach.
- Czcionki systemowe, bez zewnętrznych zasobów (CDN, fonty, skrypty).
- Kotwice (`id`) bez polskich znaków; teksty widoczne dla użytkownika
  z polskimi znakami.
- Ścieżki do plików względne (`style.css`, nie `/style.css`).

## Podgląd lokalny

Wystarczy otworzyć `index.html` w przeglądarce albo uruchomić:

```bash
python3 -m http.server 8000
```

## Wdrożenie

Brak procesu budowania – GitHub Pages serwuje pliki bezpośrednio.
Zmiany są widoczne po scaleniu do `main`.
