## VAPE Autoclick — Site vitrine (FR)

Site vitrine statique (HTML/CSS/JS vanilla) présentant l’outil « VAPE Autoclick ». Ce dépôt ne contient que l’interface web (aucun binaire, aucune installation côté serveur).

## Aperçu

- **Stack**: HTML unique (`index.html`) avec styles et scripts embarqués
- **Fonctionnalités UI**: navigation par onglets via hash, interface responsive, fond animé `<canvas>`, bouton « retour en haut », barre d’action mobile
- **Accessibilité**: lien d’évitement (« Aller au contenu »), focus visible, préférence « reduce motion » respectée
- **Sections**: Accueil, Guide, Téléchargement, FAQ, À venir

## Démarrage rapide en local

Option 1 — Ouvrir le fichier:
- Double-cliquez `index.html` pour l’ouvrir dans votre navigateur.

Option 2 — Servir en HTTP (recommandé):
- Python 3:
  - `python3 -m http.server 8080`
  - Ouvrez `http://localhost:8080/`
- Node (serve):
  - `npx --yes serve -l 8080 .`
  - Ouvrez `http://localhost:8080/`

Note: Le code tente d’afficher un checksum à titre informatif. Servir le site via HTTP évite certains comportements liés à `file://` et au CORS.

## Structure du projet

```
.
└── index.html   # Page unique avec styles et scripts inline
```

## Personnalisation

- **Méta & SEO**: modifiez les balises `<meta>` (titre, description, Open Graph) dans l’en-tête du document
- **Couleurs & thèmes**: ajustez les variables de couleurs et styles dans le bloc `<style>`
- **Contenus**: mettez à jour les listes de fonctionnalités, la FAQ et la roadmap dans les sections correspondantes
- **Scripts**: la navigation par onglets, le fond animé et les petits comportements UI se trouvent en bas de `index.html` (bloc `<script>`) 

## Déploiement

Ce site est 100% statique — hébergez-le sur n’importe quel service de pages statiques:
- GitHub Pages: branche `main` → Settings → Pages → déployer le dossier racine
- Netlify / Vercel / Cloudflare Pages: importer le repo, framework = « static », build = none
- Serveur/Nginx: servir le dossier contenant `index.html`

## Accessibilité (récap)

- Lien d’évitement du menu vers le contenu principal
- Styles `:focus-visible` renforcés
- Prise en compte de `prefers-reduced-motion`
- Navigation fonctionnelle au clavier

## Avertissement légal & éthique

Ce dépôt présente une page d’information pour un outil d’automatisation de clics. L’utilisation d’outils d’automatisation peut être limitée ou interdite par certaines applications/plateformes. Vous êtes entièrement responsable du respect des lois et des conditions d’utilisation des services tiers. Ce projet n’encourage ni n’approuve l’usage abusif (p. ex. triche, contournement de protections, atteinte à l’équité de jeu). Utilisez-le uniquement dans des contextes légitimes (tests, accessibilité, automatisation permise).

## Licence

Aucune licence explicite n’est fournie dans ce dépôt. Par défaut, tous droits réservés. Ajoutez une licence (MIT, Apache-2.0, etc.) si vous souhaitez autoriser la réutilisation.

## Crédits

UI/UX et code HTML/CSS/JS: ce dépôt.

