# Idée : page « curseurs de personnalité de marque »

> Brainstorm v1. Prototype : `docs/nuancier.html`.
>
> **Choix de Julie** : tester les 3 noms ; double point de départ (marque / programme interne), la niche « programme interne » mise en avant ; offre d'atelier affichée sans prix ; aperçu spectaculaire ; accès depuis le menu + recommandation : depuis la section Contact.

## L'idée en une phrase
Une page interactive où un client règle des curseurs (Classique ↔ Contemporain, Sérieux ↔ Ludique…) pour poser la personnalité de sa marque ou de son programme. Il repart avec un brief clair, et il a une raison concrète d'écrire à Julie.

## Pourquoi c'est une bonne idée
- **Ça qualifie les demandes** : Julie reçoit un brief déjà structuré au lieu d'un « on aurait besoin d'un logo ».
- **Ça démontre sa méthode** : le réflexe du conseil, « comprendre avant de dessiner », devient visible et utilisable.
- **Ça prolonge une offre existante** : Julie anime déjà des ateliers de branding (Kaizo). L'outil en est la version en libre-service, et l'atelier en est la suite naturelle.
- **Ça attire du trafic** : les recherches du type « définir la personnalité de sa marque » ou « brief identité visuelle » peuvent mener à la page.

## Noms possibles
1. **Le Nuancier**, nuancier de marque. Vocabulaire de designer, chaleureux. *(préféré)*
2. **Curseurs**, simple et direct.
3. **Réglages de marque**, dans l'esprit d'une table de mixage.

## Parcours
1. **Choisir son point de départ** : « Une marque » ou « Un programme interne ». Le second correspond à la niche de Julie.
2. **Régler 8 à 10 curseurs**, un écran ou une ligne à la fois.
3. **Voir l'aperçu évoluer en direct** : une mini-identité (typo, couleurs, formes, rythme) change à chaque réglage. C'est l'effet « waouh » qui démontre le savoir-faire. L'aperçu est présenté comme indicatif.
4. **Obtenir son portrait de marque** : un texte généré à partir des réglages (« Une marque contemporaine, chaleureuse et accessible… »), avec ses 3 traits dominants.
5. **Compléter le brief** en 4 ou 5 questions courtes : cible, objectif, supports, échéance, budget sous forme de fourchette (facultatif).
6. **Choisir comment repartir** :
   - « Envoyer mon brief à Julie » → formulaire, c'est l'objectif principal ;
   - « Copier le lien » → les réglages sont dans l'URL, pour les partager avec son équipe ;
   - « Télécharger le brief » (V2).

## Les curseurs
**Tronc commun**
- Classique ↔ Contemporain
- Sérieux ↔ Ludique
- Institutionnel ↔ Proche
- Discret ↔ Expressif
- Rationnel ↔ Émotionnel
- Accessible ↔ Exclusif
- Calme ↔ Énergique
- Minimal ↔ Généreux

**Spécifiques « programme interne »**
- Descendant ↔ Participatif
- Rassurant ↔ Disruptif
- Ponctuel ↔ Au long cours

## Ce que l'aperçu fait varier
| Curseur | Effet visuel |
|---|---|
| Classique ↔ Contemporain | police à empattements → grotesque |
| Sérieux ↔ Ludique | angles droits → formes arrondies, légère rotation |
| Calme ↔ Énergique | vitesse et amplitude des animations |
| Discret ↔ Expressif | saturation et contraste des couleurs |
| Minimal ↔ Généreux | densité, taille des éléments, espaces |
| Rationnel ↔ Émotionnel | palette froide → chaude |

## L'idée « équipe » (V2)
Plusieurs personnes d'une même entreprise règlent leurs curseurs. L'outil montre où elles sont d'accord et où elles divergent. Ces écarts deviennent le point de départ d'un **atelier de positionnement** animé par Julie. C'est très parlant pour les grands groupes et les comités de pilotage.

## De l'outil à la mission
Outil gratuit → brief reçu → **atelier de positionnement** (à définir : durée, format, prix) → direction artistique → déclinaisons.

## Technique (site statique)
- Tout se calcule dans le navigateur, sans serveur.
- Le brief est envoyé par un service de formulaire (Formspree, Tally ou Netlify Forms), sans clé secrète dans le code.
- RGPD : consentement explicite, finalité indiquée (« pour vous recontacter au sujet de votre projet »), pas de données sensibles demandées.
- Partage : les réglages sont encodés dans l'URL.

## Versions
- **MVP** : 8 curseurs, aperçu simple (typo + couleurs), portrait de marque, formulaire.
- **V2** : volet « programme interne », téléchargement du brief, comparaison en équipe.

## Questions ouvertes
- Le nom ?
- Un ou deux points de départ (marque / programme interne) dès le MVP ?
- Afficher l'offre « atelier de positionnement » (avec ou sans prix) ?
- Quel niveau d'aperçu : simple ou spectaculaire ?
- Où la page vit-elle : entrée dans le menu, lien depuis le contact, depuis les études de cas ?
