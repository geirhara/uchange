# Landingssider for uChange

Denne mappen inneholder alle kampanjelandinger under subdomenet `kampanje.uchange.no`.

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
