# Landingssider for uChange

Denne mappen inneholder alle kampanjelandinger under subdomenet `gh.uchange.no`.

## Struktur

Hver landingsside har sin egen mappe med sitt eget `index.html`:

```
landingssider/
├── kampanje-1/
│   └── index.html
├── kampanje-2/
│   └── index.html
└── kampanje-3/
    └── index.html
```

## Hvordan lage en ny landingsside

1. Kopier en eksisterende kampanjamappe eller malen
2. Lag ny mappe under `landingssider/` med navn som `kampanje-navn`
3. Kopier `../mal-template/index.html` og tilpass den
4. Oppdater bildereferanser til `../assets/`
5. Commit og push

## Assets (Delte ressurser)

Alle bilder, logoer og felles ressurser ligger i `../assets/`:

- Logoer
- Profilbilde
- Illustrasjoner
- Andre mediafiler

Referenser fra HTML-filer:
```html
<img src="../assets/logo_GH-signatur_RED.png" alt="..." />
```
Grafikk særskilt for den enkelte landingsside ligger i rot på mappen for kampanjen.

## Forsiden (`index.html`) – lenken i Bio

`landingssider/index.html` er forsiden på `gh.uchange.no` (Netlify publiserer mappen
`landingssider/`). Siden er en enkel «link i bio»-side for sosiale medier.

**Legge til en ny lenke:** åpne `index.html`, finn kommentarblokken «LENKER», kopier en
hel `<a class="link-card">`-blokk, lim den inn der du vil ha den (øverst = mest klikk)
og bytt ut adresse, tittel og undertekst. Rekkefølgen i koden er rekkefølgen på siden.

- `class="link-card featured"` gir gullknappen som løfter frem det viktigste – bruk den på én lenke om gangen.
- `<span class="lc-badge">` er merkelappen, f.eks. «Aktuelt nå». Slett linjen om den ikke skal vises.
- Ikonene for sosiale medier ligger nederst i filen, med adressene i `href`.
