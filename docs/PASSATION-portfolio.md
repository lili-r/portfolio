# Passation : portfolio (design et contenu)

> Session dédiée au site portfolio. L'outil « Nuancier » est traité dans une autre session : voir `docs/PASSATION-nuancier.md`. Ne pas y toucher ici.

## À lire en premier
- `CLAUDE.md` : brief complet, choix validés, workflow.
- `docs/positionnement.md`, `docs/ux.md`, `docs/contenu.md`, `docs/references.md`.
- `docs/projets/` : études de cas (01 programme interne et 02 Kaizo rédigées ; 07 Orbit en ébauche).

## Prototype de l'accueil
- Fichier : `docs/test-home.html`, publié en artifact : https://claude.ai/artifact/Naq3qahzBrwBjV6Rv8cUrT. Republier sur le même fichier pour garder le lien.
- Images web dans `docs/assets/` (webp allégés, publiés avec `files: {"assets/xxx.webp": "docs/assets/xxx.webp"}`). Originaux dans `visuels/`, avec des noms anonymisés.
- **Validé** : univers sombre ; header = composition Figma de Julie (portrait avec le chien, kaléidoscope, tampon, poulpe, étoile, pictos dans des ronds translucides, étiquette « Conforme »), sans rotation du tampon ; mots qui changent en rose dans la phrase du header ; CTA « Écrivez-moi » en pilule légèrement magnétique (surtout pas de rond) ; section Projets en grille 2 colonnes, titre « Des univers pensés pour prendre vie. » ; Savoir-faire « De l'idée à l'univers, du concept au mouvement. » ; contact = variante « Lueur » ; numéros de section « 01 » en style fin (police des titres) ; carte de vœux sous embargo en **carte à gratter**.
- **Refusé** : les 3 pistes de `docs/da-pistes.html`, le « bazar organisé », le header rond, les étiquettes de type « Sous embargo », le style mono/code pour les numéros, la numérotation serif « N°1 » ou glyphe.
- La barre de test en bas ne propose plus que : Header « Ta compo » / « Mosaïque ».

## Projets (miniatures actuelles)
01 Programme interne (visuel C-NUM + galerie de 3) · 02 Kaizo (poulpe) · 03 Onboarding IA (homme au téléphone jaune) · 04 Événement interne (kaléidoscope) · 05 Intranet SharePoint (emplacement provisoire) · 06 Utah, coffee shop dog-friendly (logo) · 07 Orbit (marque fictive, à présenter comme exploration IA) · 08 Carte de vœux (sous embargo, carte à gratter).

## Règles importantes
- Confidentialité : ne jamais afficher le nom du client aéronautique (logo effacé sur la blouse, fichiers renommés). Prévenir Julie si un nouveau visuel le montre.
- Orbit = projet fictif : ne jamais le présenter comme un projet client.
- Business de templates de mariage (GIF « opening-door » attendu, jamais reçu) : rester discret.
- Pas d'écriture inclusive. Ton chaleureux, design, structuré.
- Méthode de Julie : tester d'abord, figer les règles ensuite (`docs/da.md` reste à écrire).
- Commits au nom de Julie Ramier, poussés sur `main` à chaque étape.

## Prochaines étapes possibles
1. Harmoniser les derniers éléments en style « code » (petit texte au-dessus du nom, années, pied de page).
2. Écrire `docs/da.md` (système figé à partir des choix validés).
3. Compléter les études de cas 03 à 08 (questions déjà posées à Julie : année, rôle, contexte, livrables, fierté).
4. Ajouter l'accès au Nuancier dans le menu et dans la section Contact (« Pas encore de brief ? Posez-le en 3 minutes »).
5. Ensuite : passage au code Astro (skill `dev-frontend`).
