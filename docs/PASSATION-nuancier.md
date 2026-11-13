# Passation : outil « Le Nuancier » (curseurs de personnalité)

> Session dédiée à l'outil. Le portfolio est traité dans une autre session : voir `docs/PASSATION-portfolio.md`. Ne pas toucher à `docs/test-home.html` ici.

## À lire en premier
- `CLAUDE.md` (ton, règles générales), puis `docs/idee-curseurs-de-marque.md` (brainstorm et historique v1 → v3).
- Données de Julie : `docs/nuancier-32-profils.xlsx` (onglets « 32 profils » et « Guide des axes »).
- Références visuelles : `docs/img/nuancier-refs/` (UNNA, nuage rose, « W », pictos modulaires).

## Prototype
- Fichier : `docs/nuancier.html`, publié en artifact : https://claude.ai/artifact/H2PSPizcPv9z7Dwu2yjmDZ. Republier sur le même fichier pour garder le lien.
- Parcours : 01 point de départ (À vos équipes / À vos clients) → 02 cinq curseurs + planche d'identité en direct → 03 portrait → 04 brief (envoi simulé) → 05 mode équipe + atelier de positionnement (sans prix).
- Barre de test en haut : nom (Le Nuancier / Curseurs / Réglages de marque), formulation des entrées et **transition entre profils** (Fondu / Éclosion / Vague).
- Transition : l'ancienne planche est figée dans un calque « fantôme » posé par-dessus, le nouveau profil s'installe dessous, puis le fantôme s'efface (fonctions `ghost()` et `morph()`). Désactivée si l'utilisateur a demandé moins d'animations.

## Décisions de Julie
- Outil **simple, grand public, ludique**.
- **5 curseurs** : Classique ↔ Contemporain (ex. Hermès / Nothing), Discret ↔ Affirmé (Aesop / Diesel), Rationnel ↔ Émotionnel (IBM / Disney), Accessible ↔ Exclusif (IKEA / Rolex), Conventionnel ↔ Audacieux (LinkedIn / Balenciaga).
- **32 profils** = 2⁵ combinaisons (chaque curseur à gauche si < 50, à droite si ≥ 50). Numéro = 1 + style×16 + expression×8 + communication×4 + positionnement×2 + créativité.
- **Sur la planche, jamais de nom de marque** : seulement une ambiance (nom et description du profil).
- **« Peu importe le design, il faut que ce soit beau »** : rien n'est calculé au hasard. Chaque profil a une ambiance composée à la main (palette de 8 couleurs, typo de titre + texte, famille de formes, casse) dans le tableau `PROFILS` du script.
- Niche prioritaire : la communication interne, mais l'externe reste proposé.
- Atelier affiché sans prix. Accès prévu : menu + section Contact du portfolio.

## Questions en attente (posées à Julie)
1. Quelles ambiances ne correspondent pas à son idée du profil ?
2. Garder ou non les marques en exemple sous les curseurs ?
3. Garder ou retirer le choix interne / externe (il ne change plus que les textes) ?
4. Quelle transition entre profils garder : Fondu, Éclosion ou Vague ?

## Règles
- Pas d'écriture inclusive. Commits au nom de Julie Ramier, poussés sur `main`.
- Vérifier le rendu des 32 profils (captures Playwright) après toute modification des ambiances.
