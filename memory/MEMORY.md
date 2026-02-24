# CEVPU – Mémoire projet

## Structure du site
- Site statique HTML/CSS, déployé via GitHub Pages sur cevpu.org
- Pages : index.html, fonctionnement.html, histoire.html, travaux.html, contact.html, mentions-legales.html
- Dossier `travaux/` : PDFs + acronymes.html

## Design (refonte 2025)
- Toutes les pages utilisent **`css/index.css`** (remplace l'ancien style.css)
- Typographie : **Inter** (Google Fonts)
- Couleur principale : `#11aacc` (teal CEVPU), variables CSS dans `:root`
- Header : sticky 68px, glassmorphism, nav avec drawer mobile JS (pas de checkbox hack)
- index.html : hero plein écran (88vh) avec photo cevpu_photo_index.jpg
- Pages internes : bannière `.page-banner` (dégradé navy), puis sections alternées blanc/gris
- Footer : fond sombre `#0a1628`

## Composants CSS clés
- `.page-banner` : bannière pages internes
- `.person-card` / `.people-grid` : organisation (fonctionnement)
- `.doc-card` / `.docs-grid` : documents travaux
- `.cdp-link` : communiqués de presse
- `.contact-wrapper` / `.contact-email` : page contact
- `.legal-content` : mentions légales

## Images disponibles
- CEVPU_Communication_Logo_Court.webp (carré)
- CEVPU_Communication_Logo_Long_FondTransparent.webp (bandeau footer)
- cevpu_photo_index.jpg (photo hero)
- instagram-ico.webp, linkedin-ico.webp, twitter-ico.webp

## Navigation mobile
- Script inline dans chaque page (pas de script.js externe pour la nav)
- Toggle id="nav-toggle", liste id="nav-list", classe .is-open
- Fermeture ESC + clic extérieur
