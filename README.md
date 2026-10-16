# Rétro-PC Dépannage — refonte d'un site vitrine

Site vitrine de trois pages pour une entreprise de réparation d'ordinateurs
vintage, refait entièrement à partir d'une unique page HTML dépassée.  
Résultats mesurés : **100/100 en Performance, Accessibilité et SEO** sur toutes les pages.

**Auteur :** Rafaël HOCQUE
**Version :** 1.0 - janvier 2026

## L'objectif

Transformer un site désuet en un site **responsive**, **accessible** (utilisable
par les personnes qui naviguent à l'aide d'un lecteur d'écran) et **« SEO friendly »**
(mieux classé dans les moteurs de recherche).

| # | Problème de départ | Conséquence |
|---|--------------------|-------------|
| 1 | Design dépassé | L'image donnée à l'entreprise ne donnait pas confiance |
| 2 | Manque d'accessibilité | Site non responsive, non adapté aux lecteurs d'écran |
| 3 | Code confus | Tout le contenu dans un seul fichier HTML, impossible à maintenir |

## Ce qui a changé

| Ce qui change | Avant | Après |
|---------------|-------|-------|
| Design | Palette et typographie dépassées | Couleurs, titres et espacements modernes, centralisés en variables |
| Structure | Une seule page HTML | Un fichier par page : Accueil, Services, Contact |
| Responsive | Absent | Mobile-first, deux colonnes à partir de 768 px |
| Thème sombre | Absent | Automatique selon les préférences du système, sans JavaScript |
| Accessibilité | Images sans texte alternatif, champs sans label | Tout est décrit et relié, structure sémantique complète |
| Contraste | Insuffisant sur les zones colorées | Fond plus sombre sous les textes, corrigé après l'audit Lighthouse |
| Images | JPEG et PNG lourds | WebP avec repli JPEG : 196 ko → 98 ko sur l'image d'accueil |

## Les pages

| Page | Contenu |
|------|---------|
| **Accueil** | Bannière avec photo et accroche, trois cartes de savoir-faire, encart « À propos » et contact rapide |
| **Services** | Diagnostic complet, réparation matérielle, installation d'un système, puis grille de tarifs |
| **Contact** | Formulaire de demande de devis : nom, prénom, téléphone, email, message |


## Le résultat

| Catégorie | Score |
|-----------|-------|
| Performance | **100 / 100** |
| Accessibilité | **100 / 100** |
| Bonnes pratiques | 96 / 100 |
| SEO | **100 / 100** |

Mesuré avec Lighthouse sur les trois pages, en mode clair comme en mode sombre :
le score d'accessibilité reste à 100 dans les deux thèmes.
