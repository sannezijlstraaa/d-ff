# D/ff Sports Management — Landingspagina

E�n bestand, klaar om te deployen.

## Bestanden

```
dff-landing/
├── index.html      ← de volledige pagina (HTML + CSS in één bestand)
└── README.md
```

## Foto's toevoegen

Maak een map `images/` aan en voeg persfoto's toe. Vervang daarna in `index.html` de SVG-placeholders door:

```html
<!-- Jill Roord -->
<img src="images/jill-roord.jpg" alt="Jill Roord">

<!-- Pien Sanders -->
<img src="images/pien-sanders.jpg" alt="Pien Sanders">

<!-- Boyd Rood -->
<img src="images/boyd-rood.jpg" alt="Boyd Rood">
```

De `.fc-img` container is al gestyled met `object-fit: cover` — de foto past zich automatisch aan.

## Deployen via GitHub Pages

1. Maak een nieuwe repository aan op GitHub (bijv. `dff-landing`)
2. Upload `index.html` (en eventueel de `images/` map)
3. Ga naar **Settings → Pages**
4. Kies bij Source: `main` branch, `/ (root)`
5. De pagina is live op `https://jouwusername.github.io/dff-landing`

## Contactformulier activeren

Het e-mailinputveld werkt nog niet. Koppel het eenvoudig via [Formspree](https://formspree.io):

```html
<!-- Vervang de <div class="cta-row"> door: -->
<form class="cta-row" action="https://formspree.io/f/JOUW_ID" method="POST">
  <input class="cta-inp" type="email" name="email" placeholder="jouw@email.nl" required />
  <button class="cta-sub" type="submit">Stuur bericht ↗</button>
</form>
```
