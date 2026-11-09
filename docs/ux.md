# UX — Portfolio Julie Ramier

## 1. Objectifs
- **Objectif n°1** : obtenir des prises de contact pour des missions freelance.
- **Objectif n°2** : être référencée par des cabinets de conseil qui la placeront sur leurs missions.
- **En 5 secondes**, le visiteur doit savoir : *Julie Ramier, designer graphique & motion à Paris : identités et communication, avec une culture du conseil et des grands groupes.*
- **CTA principal unique** : « Parlons de votre projet » → section contact (mail + LinkedIn). CTA secondaire : « Télécharger mon CV ».

## 2. Cibles
1. Grands groupes en direct (communication interne, RH, transformation)
2. Cabinets de conseil qui la vendent sur leurs missions
3. PME (logos, identités). *Note interne : sert aussi de terrain d'expérimentation. À ne jamais mentionner sur le site.* Les projets logo (restaurant, Kaizo) suffisent à les rassurer, sans section dédiée.

## 3. Personas

### P1 — Claire, responsable communication interne d'un grand groupe
- **Contexte** : lance un programme de transformation et a besoin d'une identité, de supports et d'un événement. Lit les études de cas en entier.
- **Sa question** : « A-t-elle déjà fait ça, à notre échelle, avec nos contraintes (validation, confidentialité, délais) ? »
- **Ce qui la convainc** : le projet aéronautique de bout en bout, des chiffres (200 participants), une méthode claire, un ton rassurant.
- **Action attendue** : écrire pour un premier échange.

### P2 — Thomas, manager dans un cabinet de conseil
- **Contexte** : doit staffer un·e designer sur une mission client, souvent en urgence. Reste 30 à 60 secondes sur le site.
- **Sa question** : « Est-ce que je peux la proposer à mon client demain ? Que sait-elle faire, et est-elle à l'aise dans un environnement conseil ? »
- **Ce qui le convainc** : « 8 ans en cabinet de conseil » visible dès le hero, la liste des savoir-faire, un CV téléchargeable en 1 clic, une section qui s'adresse explicitement aux cabinets.
- **Action attendue** : télécharger le CV et envoyer un mail.

## 4. Arborescence
Comme sur product.inc : **une page d'accueil longue avec des ancres**, plus une page par projet.

```
/                       Accueil (one-page)
  #projets              Index des projets
  #savoir-faire         Ce que je fais
  #a-propos             Parcours + façon de travailler + CV
  #contact              Contact
/projets/[slug]         6 études de cas
/mentions-legales
/404
```
**Navigation (4 entrées)** : Projets · Savoir-faire · À propos · Contact
+ logo/monogramme « JR » à gauche (retour en haut) et lien mail à droite.
Mobile : barre fixe compacte, menu plein écran.

## 5. Parcours
- **P1 Claire** : Accueil → hero → Index projets → clic « Programme aéronautique » → lit l'étude de cas → CTA de fin « Parlons de votre projet » → mail. **2 clics.**
- **P2 Thomas** : Accueil → hero (lit « 8 ans en cabinet de conseil ») → bouton « Télécharger mon CV » (**1 clic**) → descend jusqu'à « Pour les cabinets de conseil » → mail (**2 clics**).

## 6. Wireframes (mobile d'abord, puis adaptation desktop)

### Accueil
```
┌──────────────────────────────┐
│ JR            ☰    (mail)    │  Header fixe, discret
├──────────────────────────────┤
│ [ PORTRAIT avec le chien ]   │  HERO — desktop : 2 colonnes
│                              │  portrait à gauche / texte à droite
│ DESIGNER GRAPHIQUE & MOTION  │  label majuscules, couleur accent
│ Julie Ramier                 │  H1 très grand
│ Je crée des identités et je  │  accroche (2–3 lignes)
│ les fais vivre partout…      │
│ 8 ans en cabinet de conseil. │  preuve de crédibilité
│ Basée à Paris.               │
│ [Parlons de votre projet]    │  CTA principal
│ [Télécharger mon CV]  [in]   │  CTA secondaires
├──────────────────────────────┤
│ 8 ans · 6 projets · 200 pers │  Bandeau de chiffres (optionnel)
├──────────────────────────────┤
│ PROJETS                      │  INDEX (moodboard image 2)
│ Programme aéronautique  2024 │  liste : titre en grand, année,
│ Kaizo                   2024 │  disciplines en petit
│ Événement interne       2023 │  desktop : survol = ligne en noir,
│ Onboarding en IA        2024 │  autres en gris, aperçu image
│ Intranet SharePoint     2023 │  à droite
│ Restaurant —            2022 │  mobile : vignette + titre
├──────────────────────────────┤
│ SAVOIR-FAIRE                 │  5 blocs = un système, pas une liste
│ 01 Identité                  │  logo, univers, charte
│ 02 Déclinaisons              │  print, présentations PowerPoint
│ 03 Motion                    │  motion design, vidéo IA générative
│ 04 Expérience                │  événements, photobooth
│ 05 Digital interne           │  SharePoint, intranet
│ chaque bloc → lien vers 1–2  │
│ projets qui le prouvent      │
├──────────────────────────────┤
│ POUR QUI                     │  2 colonnes desktop
│ Entreprises : j'accompagne   │
│ vos programmes de A à Z      │
│ Cabinets de conseil : je     │  ← spécifique P2
│ rejoins vos missions en      │
│ renfort design               │
├──────────────────────────────┤
│ À PROPOS                     │  court, chaleureux, 1re personne
│ 8 ans en conseil, ma façon   │  + détail perso (le chien !)
│ de travailler (3 principes)  │
│ [Télécharger mon CV]         │
├──────────────────────────────┤
│ CONTACT                      │  grand titre-phrase
│ Un projet, une mission ?     │
│ [Parlons de votre projet]    │  mailto + LinkedIn
├──────────────────────────────┤
│ © Julie Ramier · Paris ·     │  footer + mentions légales
│ mail · LinkedIn              │
└──────────────────────────────┘
```

### Étude de cas `/projets/[slug]` (structure inspirée de jcubhow)
```
┌──────────────────────────────┐
│ ← Projets                    │
│ IDENTITÉ / PRINT / MOTION    │  label disciplines
│ Titre du projet              │  H1 géant
│ [ VISUEL / VIDÉO HERO ]      │  pleine largeur
│ Résumé en 2 phrases          │
│ Client  · Groupe aéro (anon.)│  FICHE technique
│ Rôle    · DA, design, motion │
│ Livrables · …                │
│ Année   · …  Outils · …      │
├──────────────────────────────┤
│ CONTEXTE                     │  label
│ Titre-phrase qui énonce      │  ex. « Un programme interne
│ l'idée                       │  qui devait donner envie »
│ paragraphe                   │
├──────────────────────────────┤
│ LE DÉFI  + 3–4 objectifs     │
├──────────────────────────────┤
│ DÉMARCHE  01 02 03 04        │  étapes numérotées
├──────────────────────────────┤
│ LE SYSTÈME                   │  logo, palette, typo, règles
├──────────────────────────────┤
│ RÉALISATIONS                 │  galerie : slides, print, motion,
│ [img] [img]                  │  événement, SharePoint
│ [   vidéo   ]                │
├──────────────────────────────┤
│ RÉSULTATS  200 participants… │  chiffres en grand + puces
├──────────────────────────────┤
│ CE QUE J'EN RETIENS          │  réflexion, 1 paragraphe
├──────────────────────────────┤
│ [Parlons de votre projet]    │
│ PROJET SUIVANT → Kaizo       │
└──────────────────────────────┘
```
Les projets plus petits (logo du restaurant) utilisent une **version courte** : hero, fiche, contexte, système, réalisations, projet suivant.

## 7. Ordre des projets (du plus fort au plus léger)
1. Programme interne aéronautique : projet phare, il prouve « l'identité puis les déclinaisons partout »
2. Kaizo : identité d'un programme de transformation
3. Vidéo d'onboarding en IA générative : motion + IA
4. Événement interne : 200 personnes, slides, photobooth
5. Intranet SharePoint d'un programme interne
6. Logo d'un restaurant : ouverture hors corporate

## 8. Confidentialité
- Client anonymisé : « Groupe aéronautique international ». Aucun logo ni nom de client, de collaborateur ou de projet interne sensible.
- Visuels : masquer ou flouter les textes internes, ou recréer des maquettes de présentation (mockups) avec des contenus neutres.
- Un discret « Certains éléments ont été modifiés pour des raisons de confidentialité » en bas des études de cas concernées. Cela rassure aussi les grands groupes.

## 9. Notes pour la DA
- Hero : portrait + chien. **Placeholder** en attendant la photo, même ratio que la future photo (4:5 ou carré).
- Index projets : liste typographique avec survol (moodboard image 2). C'est l'élément signature.
- Les titres de section sont des **titres-phrases** (jcubhow) avec petits labels en majuscules.
- Ton : chaleureux, design, structuré → palette chaude, grain, grille nette.

## 10. Notes pour le dev
- Les projets sont des fichiers Markdown (`src/content/projets/`) avec champs : titre, slug, année, disciplines[], client, rôle, livrables[], outils[], résumé, couverture, ordre, confidentiel (bool), format (`complet` | `court`).
- Les ancres doivent rester utilisables quand le header est fixe (`scroll-margin-top`).
- Le survol de l'index doit aussi marcher au clavier (focus). Sur mobile, pas de survol : afficher des vignettes.
- CV : `public/julie-ramier-cv.pdf`.

## Questions ouvertes
- Les sujets 1, 3 et 5 (programme aéro, événement, SharePoint) portent-ils sur **le même programme** ? Si oui, on peut en faire **un grand projet phare** + 2 études courtes, ou garder 3 études séparées reliées entre elles.
- Années de chaque projet ?
- Visuels disponibles par projet (formats, vidéos) ?
