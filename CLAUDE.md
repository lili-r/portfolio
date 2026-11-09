# Portfolio — instructions projet

Site portfolio personnel. Langue principale : français (anglais en option).

## Brief
- **Qui** : Julie Ramier, Paris, 8 ans en cabinet de conseil. Designer généraliste : motion design, présentations (PPT), print, graphisme, communication interne, design SharePoint, UX/UI (à ne pas trop mettre en avant).
- **Positionnement** : en cours de définition — voir `docs/positionnement.md`.
- **Objectif n°1 du site** : missions freelance ; ouvert à un CDI « coup de cœur ».
- **Cible** : [à confirmer] grandes entreprises (communication interne, transformation), agences.
- **Projets** (visuels, rôle, année, chiffres : à compléter) :
  1. Programme interne d'un grand groupe aéronautique : DA puis déclinaisons, accompagnement d'événement interne, SharePoint
  2. Vidéo d'onboarding réalisée en IA générative
  3. Événement interne : communication, slide decks, photobooth
  4. Logo d'un restaurant
  5. Design SharePoint d'un programme interne
  6. Kaizo : logo et identité d'un programme de refonte des process
- **Confidentialité** : [à vérifier] peut-on citer le client aéronautique et montrer les visuels internes ?
- **Portrait** : photo avec un chien, à fournir. Placeholder en attendant.
- **Ton** : chaleureux, design, structuré.
- **Moodboard** : `docs/img/moodboard-01.png`, analysé dans `docs/references.md`.
- **Références aimées** (analyse détaillée : `docs/references.md`) :
  - https://www.product.inc/#resume — structure, ton, navigation simple, portrait avec le chien en home
  - https://jcubhow.com/colour — présentation des travaux, réflexion derrière chaque projet, typographie
- **Contraintes** : délai, hébergement, nom de domaine

## Workflow — utiliser les skills dans cet ordre
1. `ux-portfolio` → arborescence, parcours, wireframes
2. `redaction-contenu` → textes (accroche, à propos, études de cas)
3. `direction-artistique` → identité visuelle, design tokens
4. `dev-frontend` → implémentation
5. `qa-seo-accessibilite` → contrôle avant mise en ligne

Chaque étape produit un livrable dans `docs/` (ex. `docs/ux.md`, `docs/da.md`) qui sert d'entrée à l'étape suivante. Ne pas passer au code tant que `docs/ux.md` et `docs/da.md` n'existent pas.

## Stack par défaut
Astro + CSS natif (custom properties) — site statique, rapide, contenu en Markdown/MDX.
Déploiement : Netlify, Vercel ou GitHub Pages.
