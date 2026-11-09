---
name: qa-seo-accessibilite
description: Contrôle qualité avant mise en ligne du portfolio — accessibilité (WCAG AA), performance (Core Web Vitals), SEO, partage social et responsive. À utiliser après une modification importante du site et avant chaque déploiement.
---

# QA — Accessibilité, performance, SEO

Tu agis comme un·e testeur·se exigeant·e. Tu **mesures** avant d'affirmer : chaque point est vérifié par un outil ou une capture, pas supposé.

## Outils (Chromium + Playwright préinstallés)
- Build : `npm run build && npm run preview`
- Lighthouse : `npx lighthouse <url> --chrome-flags="--headless --no-sandbox" --output=json`
- Accessibilité : `@axe-core/playwright` sur chaque page
- Captures Playwright à 360, 768, 1280 px, thèmes clair et sombre

## Checklist
**Accessibilité**
- [ ] 0 violation axe ; contrastes ≥ AA
- [ ] Navigation complète au clavier, focus visible, ordre logique
- [ ] Un `h1` par page, hiérarchie de titres sans saut
- [ ] `alt` pertinents (vides pour les images décoratives)
- [ ] `lang="fr"`, liens explicites, `prefers-reduced-motion` respecté

**Performance** (objectif Lighthouse ≥ 95 mobile)
- [ ] LCP < 2,5 s, CLS < 0,1, INP < 200 ms
- [ ] Images optimisées et dimensionnées, polices préchargées
- [ ] JS client minimal

**SEO & partage**
- [ ] `title` + `meta description` uniques par page, URL canonique
- [ ] Open Graph + Twitter Card avec image 1200×630
- [ ] `sitemap.xml`, `robots.txt`, favicon, page 404
- [ ] Données structurées `Person` (JSON-LD) sur l'accueil

**Responsive & contenu**
- [ ] Aucun débordement horizontal, textes lisibles sur mobile
- [ ] Aucun `[À COMPLÉTER]`, lorem ipsum ou lien mort restant
- [ ] Liens externes, `mailto:`, CV téléchargeable fonctionnels

## Livrable
`docs/rapport-qa.md` : scores, problèmes classés (bloquant / important / mineur) avec fichier concerné et correctif proposé. Corriger les bloquants avant de déclarer le site prêt.
