# Portfolio — instructions projet

Site portfolio personnel. Langue principale : français (anglais en option).

## Brief
- **Qui** : Julie Ramier, Paris, 8 ans en cabinet de conseil. Designer généraliste : motion design, présentations (PPT), print, graphisme, communication interne, design SharePoint, UX/UI (à ne pas trop mettre en avant).
- **Positionnement** : designer graphique & motion — identités et communication (v1, voir `docs/positionnement.md`).
- **Objectif n°1 du site** : missions freelance ; ouvert à un CDI « coup de cœur ».
- **Cibles** : grands groupes en direct ; cabinets de conseil (qui la vendent sur leurs missions) ; PME (note interne, voir `docs/positionnement.md` — ne pas communiquer sur le site).
- **Projets** (visuels, rôle, année, chiffres : à compléter) :
  1. Programme interne d'un grand groupe aéronautique : DA puis déclinaisons, accompagnement d'événement interne, SharePoint
  2. Vidéo d'onboarding réalisée en IA générative
  3. Événement interne : communication, slide decks, photobooth
  4. Utah : logo d'un coffee shop dog-friendly
  5. Design SharePoint d'un programme interne
  6. Kaizo : atelier de branding, naming, logo, mascotte poulpe et identité d'une solution tech créée sans designer (2026)
  7. Orbit : marque FICTIVE créée pour tester les outils d'IA → toujours la présenter comme projet personnel / exploration IA, jamais comme projet client
  8. Invitations animées : projet perso (business de templates de mariage, pas encore lancé — rester discret) + déclinaison BtoB à concevoir ; GIF « opening-door » attendu
- **Confidentialité** : client aéronautique anonymisé (voir `docs/ux.md` §8).
- **Chiffre clé** : événement interne de 200 personnes.
- **Portrait** : photo avec un chien, à fournir. Placeholder en attendant.
- **Ton** : chaleureux, design, structuré. Pas d'écriture inclusive.
- **Choix UX validés** : accueil avec bibliothèque d'images des projets ; études de cas en 2 modes (Essentiel / En profondeur) ; section « Ce dont je suis le plus fière » dans chaque projet.
- **Moodboard** : `docs/img/moodboard-01.png`, analysé dans `docs/references.md`. Esprit d'accueil retenu : `docs/img/moodboard-02-home.png` (fond sombre pointillé, cartes d'interface flottantes, labels mono numérotés).
- **Méthode DA (choix de Julie)** : tester d'abord, définir les règles ensuite. On itère sur l'accueil (`docs/test-home.html`), puis on décline et on fige la DA dans `docs/da.md`. Les 3 pistes de `docs/da-pistes.html` ont été écartées.
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
