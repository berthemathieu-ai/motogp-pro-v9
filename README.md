# MotoGP Pro Racing V9 — prototype PWA public

## Contenu
- `index.html` : interface et navigation
- `style.css` : design V9
- `app.js` : appels aux API, calendrier, classement, pilotes, circuits et météo
- `manifest.webmanifest` et `icon.svg` : installation sur écran d'accueil
- `sw.js` : mise en cache des fichiers de l'application

## Publication
1. Créer un dépôt GitHub public et y déposer les fichiers à la racine.
2. Activer GitHub Pages dans **Settings > Pages**, avec la branche principale et le dossier racine.
3. Ouvrir l'adresse HTTPS générée dans Safari sur iPhone.
4. Utiliser **Partager > Sur l'écran d'accueil > Ajouter**.

## Limites importantes
Ceci est un **prototype fonctionnel à tester**, pas une migration intégrale de la V8.
- L'API MotoGP peut refuser les requêtes provenant d'un navigateur (CORS). Dans ce cas, utiliser un backend/proxy autorisé ; GitHub Pages seul ne suffit pas.
- L'onglet Live est un emplacement réservé, pas un chronométrage actif.
- Les fiches pilotes sont simplifiées ; les records de circuits de V8 ne sont pas encore importés.
- Le cache hors ligne couvre les fichiers de l'application ; les données API sont mises en cache via localStorage après un premier chargement.
- Les dates et horaires doivent être vérifiés par rapport au calendrier officiel, notamment lors des reports.
- Pour un usage public, vérifier les conditions d'utilisation des données, des noms et des images MotoGP.
- Une icône SVG peut ne pas être acceptée comme icône d'installation par tous les navigateurs ; prévoir des PNG 192x192 et 512x512 avant une diffusion large.
