# uChange - Kampanjelandinger

Repository for kampanjelandinger og landingssider under uchange.no subdomenet `kampanje.uchange.no`.

## 📁 Mappestruktur

```
uchange/
├── mal-template/              # Mal for nye landingssider
│   └── index.html
├── landingssider/             # Alle aktive kampanjelandinger
│   ├── README.md
│   ├── kampanje-1/
│   ├── kampanje-2/
│   └── ...
├── assets/                    # Delte ressurser (logoer, bilder, etc)
│   ├── favicon.ico
│   ├── logo_*.png
│   ├── logo_*.gif
│   ├── portrett_*.webp
│   ├── image_*.webp
│   └── ...
└── README.md                  # Dette filen
```

## 🚀 Hvordan bruke malen

1. **Opprett ny kampanjemappe:**
   ```bash
   mkdir landingssider/kampanje-ny-navn
   cp mal-template/index.html landingssider/kampanje-ny-navn/
   ```

2. **Rediger HTML-filen:**
   - Oppdater tittel, beskrivelse og innhold
   - Referanser til assets bruker `../assets/filnavn`

3. **Commit og push:**
   ```bash
   git add .
   git commit -m "Ny kampanjeside: kampanje-ny-navn"
   git push
   ```

4. **Netlify deployer automatisk!**

## 🎨 Branding

### Farger
- **Primær blå:** `#0F3D54`
- **Sekundær rød:** `#990000`
- **Aksent gull:** `#D4A06F`
- **Bakgrunn:** `#F5F5F5` (mint)

### Typografi
- **Overskrifter:** Playfair Display
- **Brødtekst:** Montserrat

## 📱 Responsive Design

Malen er fullt responsiv med breakpoint på 820px.

## 🔄 Arbeidsflyt

1. Lag kampanjeside med AI agent i Netlify
2. Netlify lager automatisk PR på GitHub
3. Du godkjenner/merger PR
4. GitHub oppdaterer main-branchen
5. Netlify deployer automatisk ✅

## 📝 Lisens

uChange AS
