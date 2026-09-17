# Nedtellingsklokke

En frittstående HTML-side med en digital nedtellingsklokke for visning på storskjerm.
Følger uCharges grafiske mal: Playfair Display (overskrift) + Montserrat (brødtekst),
og merkefargene dyp blå `#0F3D54`, gulbrun `#D4A06F`, dyp rød `#990000`.

## Bruk

1. Åpne `index.html` i en nettleser (Chrome/Edge anbefalt) på storskjermen.
2. Trykk **F** for fullskjerm.
3. Skriv inn spørsmålet/oppgaven i feltet, sett minutter og sekunder.
4. Trykk **Start** (eller mellomrom). Kontrollene skjules automatisk mens tiden går.

## Hurtigtaster

| Tast | Handling |
|------|----------|
| Mellomrom / Enter | Start / Pause |
| R | Nullstill |
| F | Fullskjerm av/på |
| H | Skjul/vis kontroller |
| Esc | Pause |

## Bygge oppgaver via URL

Man kan lenke direkte til en ferdig oppgave uten å skrive den inn:

```
index.html?q=Hva+tar+du+med+deg+videre?&sub=Snakk+to+og+to&m=2&s=0
```

- `q` – spørsmål/oppgave (venstre side)
- `sub` – undertekst (valgfri)
- `m` – minutter
- `s` – sekunder

## Bruk i PowerPoint

- Enklast: legg inn en **Web Viewer**-add-in (Office Store) og pek på URL-en,
  eller ta med skjermen i fullskjerm og Alt+Tab mellom lysbildene.
- Alternativ: sette inn som «Live Web Pages»-objekt i nyere PowerPoint.

## Lyd ved tiden er ute

Klokken bytter til rødt og pulserer når tiden er ute. For lyd, legg til en
`<audio>`-kilde og spill den i `stop()` (utelatt her for å holde filen selvstendig).
