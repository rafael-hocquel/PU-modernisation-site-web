# Rétro-PC Dépannage — Refonte de site vitrine
*Note : Projet réalisé avant ma prise en main de Git et importé a posteriori sur ce dépôt pour archivage (d'où l'absence d'historique de commits).*

Refonte complète du site vitrine d'une boutique de réparation d'ordinateurs vintage. Le projet partait d'une unique page HTML vieillissante et non maintenable pour aboutir à un site statique de trois pages, pensé pour l'accessibilité, le responsive et la performance.

Le site obtient **100/100 en Performance, Accessibilité et SEO** sur Lighthouse (en thème clair comme en thème sombre).

## Pourquoi cette refonte ?

Le site d'origine cumulait plusieurs dettes techniques et visuelles :
- **Code monolithique :** Tout le contenu était entassé dans un seul fichier HTML sans structure sémantique claire.
- **Aucune adaptation mobile :** Mise en page figée, inutilisable sur petit écran.
- **Accessibilité absente :** Contrastes insuffisants, images sans attributs `alt`, champs de formulaire non reliés à leurs labels.

## Ce qui a changé

| Axe | Avant | Après |
| :--- | :--- | :--- |
| **Architecture** | Une seule page fourre-tout | Découpage en 3 pages distinctes (`Accueil`, `Services`, `Contact`) |
| **Design & Thème** | Styles en dur, couleurs datées | Variables CSS centralisées + thème sombre automatique |
| **Responsive** | Absent | Approche *mobile-first*, passage sur deux colonnes à partir de `768px` |
| **Accessibilité** | Balisage générique, aucun label | HTML sémantique complet, labels explicites, navigation au lecteur d'écran |
| **Contraste** | Texte illisible sur les fonds colorés | Assombrissement des zones d'arrière-plan suite à l'audit Lighthouse |
| **Médias** | JPEG et PNG bruts | Conversion en WebP avec fallback JPEG (ex. `196 Ko` → `98 Ko` sur la bannière d'accueil) |

## Structure du site

- **Accueil (`index.html`) :** Bannière principale, présentation des trois grands pôles d'expertise, encart « À propos » et accès rapide au contact.
- **Services :** Détail des prestations (diagnostic, réparation matérielle, installation d'OS) accompagné d'une grille tarifaire claire.
- **Contact :** Formulaire de demande de devis accessible (nom, prénom, téléphone, email, message).

## Audit Lighthouse

Tests effectués sur les trois pages du site, avec validation des contrastes sur les deux thèmes (clair et sombre) :

- **Performance :** 100 / 100
- **Accessibilité :** 100 / 100
- **Bonnes pratiques :** 96 / 100
- **SEO :** 100 / 100

## Aperçu en local

Le projet étant en HTML/CSS pur sans étape de build, il suffit d'ouvrir `index.html` dans un navigateur ou de lancer un serveur local :

```bash
git clone https://github.com/rafael-hocquel/PU-modernisation-site-web.git
cd PU-modernisation-site-web
