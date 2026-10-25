# MSPortfolio

Site personnel de Maxime Savard, consulté surtout depuis un téléphone Android, créé à l'origine avec Claude.

## Structure

- **Techno :** HTML pur, sans framework ni générateur. Basé sur le modèle Dimension de HTML5 UP (licence CCA 3.0), avec jQuery, Font Awesome et du CSS compilé à partir de Sass.
- **Pages :** une seule page, `index.html`. Les sections (Disponibilités, Profile, Experience, Projects, Immobilier, Contact) sont des fenêtres qui s'ouvrent avec des ancres (`#disponibilites`, `#intro`, `#work`, `#about`, `#immobilier`, `#contact`). La section « Elements » est un reste du modèle, cachée du menu.
- **Dossiers :** `assets/css` (le CSS chargé est `main.css`), `assets/js`, `assets/sass` (sources du CSS), `assets/webfonts`, `images/`.
- **Publication :** GitHub Pages, branche `main`. Le fichier `CNAME` contient `immobilis.ca`.
- **Style :** fond sombre `#1b1f22` avec image de fond, texte blanc, police Source Sans Pro (Google Fonts). Bouton principal « Calendrier » rouge `#A72020` avec texte blanc (tout le rouge du site utilise cette couleur).
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

## État et à faire

Dernière mise à jour : 24 octobre 2026. Tout ce qui est décrit ici est publié sur `main`.

**Fait :**
- Gros bouton « Calendrier » (rouge #A72020) sur l'accueil, qui ouvre la section Disponibilités (calendrier Google intégré + bouton « Ouvrir en plein écran », rouge #A72020 aussi). Le rouge de survol est `#C42B2B`.
- Section Immobilier (provisoire : « Nouveau volet à venir » et un bouton vers le contact).
- Bouton EN / FR en haut à droite, avec choix mémorisé.
- Séparateurs du menu corrigés (la ligne centrale du modèle est désactivée).
- Le calendrier Zoho a été remplacé par le calendrier Google (2 agendas, liste des agendas masquée). Le bouton « Ouvrir en plein écran » pointe vers le même lien Google.

**À faire :**
- Traduire en français le menu (Profile, Experience, Projects, Contact), le contenu de ces sections et le formulaire de contact. Aujourd'hui, seuls l'accueil, Disponibilités et Immobilier sont bilingues, et le reste reste en anglais quand on choisit FR.
- Remplacer la section Immobilier provisoire quand le volet immobilier sera défini (contenu à fournir par Maxime). Une vraie page pourra être ajoutée à ce moment-là.
- Corriger le titre de l'onglet, qui affiche encore « Dimension by HTML5 UP ».
- Supprimer la section « Elements » (démo du modèle, cachée du menu), seulement si Maxime le demande.
- Vérifier que les 2 agendas Google sont publics en « libre/occupé » (détails masqués), sinon le cadre est vide pour les visiteurs. Tester en navigation privée.
- Le calendrier du site est en vue Mois et dans la langue par défaut de Google, car le lien n'a ni `hl=fr` ni `mode=WEEK`. À ajouter si Maxime préfère la vue Semaine en français.
- CRM (hors site) : nettoyer les événements en doublon créés le 24 octobre à 22 h 14, à partir du 25 octobre (FOIRE VR et MOTONEIGE), puis refaire les événements proprement. Voir la mémoire « crm-doublons-calendrier ».

**Décisions déjà prises (ne pas rediscuter) :**
- On a gardé la page actuelle et sa structure au lieu de créer une nouvelle accueil à boutons ou de déplacer le portfolio vers une autre page. Les liens existants (`immobilis.ca/`, `#contact`) restent donc valides.
- Le menu ne contient pas de bouton « Disponibilités » : le gros bouton de l'accueil suffit.
- Tout le rouge du site utilise `#A72020`.
- Le calendrier du site est un calendrier Google (plus Zoho). Le lien est dans `index.html` (le cadre et le bouton plein écran), chaque `&` s'écrit `&amp;`.

## Lien de calendrier public

Le calendrier Google intégré (agendas `maxime.savard@immobilis.ca` et un agenda de groupe). Il doit rester public en lecture seule, « libre/occupé » sans détails. Pour le modifier, on le change dans les deux endroits d'`index.html` (cadre et bouton « Ouvrir en plein écran »).

```
https://calendar.google.com/calendar/embed?wkst=1&ctz=America%2FToronto&showPrint=0&showTitle=0&showTz=0&showCalendars=0&src=bWF4aW1lLnNhdmFyZEBpbW1vYmlsaXMuY2E&src=NWY1NThkNWUxMzgxYmY0YWI3OGU2M2RkNTc1YjU1YmMxNGQzZjFkZWFhYmZjYjM5YmVjYzI1YzU2NjBlYzgyZEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23039be5&color=%237986cb
```
