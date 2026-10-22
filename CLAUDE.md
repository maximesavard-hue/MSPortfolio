# MSPortfolio

Site personnel de Maxime Savard, consulté surtout depuis un téléphone Android, créé à l'origine avec Claude.

## Structure

- **Techno :** HTML pur, sans framework ni générateur. Basé sur le modèle Dimension de HTML5 UP (licence CCA 3.0), avec jQuery, Font Awesome et du CSS compilé à partir de Sass.
- **Pages :** une seule page, `index.html`. Les sections (Disponibilités, Profile, Experience, Projects, Immobilier, Contact) sont des fenêtres qui s'ouvrent avec des ancres (`#disponibilites`, `#intro`, `#work`, `#about`, `#immobilier`, `#contact`). La section « Elements » est un reste du modèle, cachée du menu.
- **Dossiers :** `assets/css` (le CSS chargé est `main.css`), `assets/js`, `assets/sass` (sources du CSS), `assets/webfonts`, `images/`.
- **Publication :** GitHub Pages, branche `main`. Le fichier `CNAME` contient `immobilis.ca`.
- **Style :** fond sombre `#1b1f22` avec image de fond, texte blanc, police Source Sans Pro (Google Fonts). Bouton principal « Calendrier » rouge vin `#6d1a36` avec texte blanc.
- **Langues :** bouton EN / FR en haut à droite. Les textes bilingues utilisent `<span data-lang="en">…</span><span data-lang="fr">…</span>`. Le contenu existant (menu, Profile, Experience, Projects, Contact) est encore en anglais seulement.
- **Contact :** formulaire envoyé à Formspree.

## Règles de travail

- Français canadien pour le contenu visible.
- Mobile d'abord et accessible : contrastes suffisants, focus visible au clavier.
- Ne jamais committer ni publier sans l'accord explicite de Maxime.
- Travailler sur une branche, jamais directement sur `main`.
- Ne pas modifier le fichier `CNAME`.
- Modifier seulement ce qui est demandé.
- Vérifier qu'aucun lien interne n'est cassé après une modification.
- Poser la question quand une information manque plutôt que deviner.

## Lien de calendrier public

Ce lien ouvre un affichage Zoho Calendar en lecture seule (Libre/Occupé, sans détails). Il se copie sans modification. Dans le HTML, chaque `&` s'écrit `&amp;`.

```
https://calendar.zoho.com/zc/ui/embed/#calendar=0801124867d0fd3fef6b1919295a4d940000711647b4b33d89401f69a787db6c54fb795a58734c40903729f3d88d76e070e1e5faaa7d5e9f9b571ae1b6dbbeac3a90b1906c991c43b74d2629&title=Dispo%3A%20Maxime%20Savard&type=1&language=fr-CA&timezone=America%2FToronto&showTitle=1&showTimezone=1&startingDayOfWeek=0&timeFormat=1&view=week&showDetail=0&theme=5&showAttendee=0&showSwitchingViews=1&expandAllday=1&eventColorType=bold&showLogo=0&multical=08011248a41fccf5de36f581b79c597b0000636b3ba6e8a61b557bf780d2344ebbd52b8a1f8999bde24335488995e9645c8fda43a1458076563734c9720d91214dd960db003ddf1a26a88da7
```
