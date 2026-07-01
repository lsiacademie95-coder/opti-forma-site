# AUDIT COMPLET — OPTIFORMA SITE
**Date :** 1er juillet 2026  
**Dépôt :** https://github.com/optiforma95-cyber/opti-forma-site  
**Production :** https://opti-forma.fr (Cloudflare Pages, déploiement automatique sur push `main`)  
**Total commits :** 64

---

## 1. IDENTITÉ LÉGALE

| Champ | Valeur |
|---|---|
| Raison sociale | OPTIFORMA |
| Forme juridique | SASU à capital variable |
| SIRET | 98840369700010 |
| NDA (déclaration d'activité) | 11950956995 |
| Mention légale obligatoire | « Enregistré sous le numéro 11950956995. Cet enregistrement ne vaut pas agrément de l'État. » |
| Certification Qualiopi | CAP2061 (délivré par CAPCERT, accréditation COFRAC n°5-0638, valide du 11/09/2025 au 10/09/2028) |
| Adresse | 9 Chaussée Jules César, 95520 Osny |
| Email | contact@opti-forma.fr |
| Téléphone | 06 35 46 84 92 |
| Calendly | calendly.com/optiforma95/30min |
| Formulaire de contact | Formspree — endpoint : `https://formspree.io/f/mdabpngk` |
| Formatrice principale | Nadia BELBOUAB |

---

## 2. STACK TECHNIQUE

| Composant | Choix |
|---|---|
| HTML/CSS/JS | Vanilla (pas de framework) — CSS inline dans `index.html`, fichier externe `css/style.css` pour les autres pages |
| Polices | Plus Jakarta Sans (titres, poids 400/500/700/800) + Inter (corps, poids 400/500/600) via Google Fonts |
| Hébergement | Cloudflare Pages (déploiement auto depuis GitHub `main`) |
| Formulaires | Formspree (`mdabpngk`) |
| Réservation | Calendly (`optiforma95/30min`) — bouton flottant sur toutes les pages |
| Sitemap | `sitemap.xml` à la racine |
| Icône | `favicon.svg` |

---

## 3. CHARTE GRAPHIQUE v2.0

```css
--teal:       #30998D   /* couleur principale */
--teal-dark:  #216e65
--teal-light: #e8f5f3
--teal-mid:   #c2e8e3
--orange:     #F97316   /* accent / CTA primaire */
--orange-dark:#ea6a0a
--orange-light:#fff7f0
--dark:       #1a2e2c   /* hero, footer */
--text:       #2d3f3d
--muted:      #6b8a87
--border:     #e0eeec
--bg:         #fff
--bg-light:   #f7fafa
```

**Typographie :**
- Titres h1/h2/h3 : Plus Jakarta Sans, font-weight 800
- Corps : Inter
- Taille base : Inter 1rem / `.hero-sub` 1.05rem

---

## 4. ARCHITECTURE DES PAGES

### Pages principales
| Fichier | Rôle | Statut |
|---|---|---|
| `index.html` | Page d'accueil — hero, grille formations, stats, à propos, pédagogie, qualiopi band, financement, CTA | ✅ Actif |
| `formations.html` | Catalogue complet — 4 cards (RNCP, RS6490, SSCT, SST) | ✅ Actif |
| `financement.html` | Dispositifs de financement CPF/OPCO | ✅ Actif |
| `qualiopi.html` | Certification Qualiopi CAP2061 | ✅ Actif |
| `a-propos.html` | Présentation OPTIFORMA & Nadia BELBOUAB | ✅ Actif |
| `contact.html` | Formulaire Formspree + coordonnées | ✅ Actif |
| `blog.html` | Index articles de blog | ✅ Actif |
| `mentions-legales.html` | Mentions légales | ✅ Actif |
| `politique-confidentialite.html` | RGPD | ✅ Actif |
| `cgv.html` | Conditions Générales de Vente | ✅ Actif |
| `404.html` | Page d'erreur custom | ✅ Actif |

### Pages de formation (fiche détaillée)
| Fichier | Formation | Statut commercial |
|---|---|---|
| `formation-rncp37275.html` | Formateur Professionnel d'Adultes — RNCP37275 Niv.5 | ✅ Vente active |
| `formation-rs6490.html` | Animer une Formation en Situation Pro — RS6490 Manitude | ✅ Vente active |
| `formation-ssct.html` | Santé, Sécurité et Conditions de Travail (SSCT) — Élus CSE | ✅ Vente active |
| `formation-sst.html` | Sauveteur Secouriste du Travail (SST) | ⏳ Pré-inscription (habilitation INRS en cours) |

### Articles de blog
| Fichier | Titre |
|---|---|
| `blog/devenir-formateur-independant.html` | Devenir formateur indépendant |
| `blog/cpf-devenir-formateur.html` | CPF et formation de formateur |
| `blog/opco-financement-formation.html` | OPCO et financement |
| `blog/qualiopi-certification.html` | La certification Qualiopi |
| `blog/rncp-vs-rs.html` | RNCP vs RS |

### Fichiers legacy (non liés dans la nav)
- `formation-evaluer-ameliorer.html`
- `formation-formateur-interne.html`
- `opti-forma-preview.html`

---

## 5. CATALOGUE FORMATIONS — DÉTAIL

### Formation 01 — RNCP37275
- **Titre :** Formateur Professionnel d'Adultes
- **Niveau :** 5 (Bac+2) — RNCP37275
- **Certificateur :** Ministère du Travail
- **Durée :** 3 à 6 mois
- **Format :** Présentiel + Distanciel
- **Financement :** OPCO, France Travail, AIF, Transitions Pro, CPF
- **VAE :** Possible
- **Valide jusqu'au :** 29 avril 2028
- **Fiche France Compétences :** francecompetences.fr/recherche/rncp/37275/

### Formation 02 — RS6490
- **Titre :** Animer une Formation en Situation Professionnelle
- **Répertoire :** RS6490 — Répertoire Spécifique
- **Certificateur :** Manitude
- **Durée :** 4 à 5 jours (24h–40h)
- **Format :** Présentiel + Distanciel
- **Financement :** OPCO, Plan de développement des compétences
- **Enregistré le :** 21/12/2023 — Valide jusqu'au 21/12/2028
- **Fiche France Compétences :** francecompetences.fr/recherche/rs/6490/

### Formation 03 — SSCT (ACTIVE)
- **Titre :** Santé, Sécurité et Conditions de Travail
- **Public :** Membres élus du CSE (titulaires, suppléants, membres CSSCT)
- **Base légale :** Art. L.2315-18 du Code du travail
- **Durées légales :**
  - 1er mandat (toute taille entreprise) : 5 jours / 35h
  - Renouvellement de mandat : 3 jours / 21h
  - Membres CSSCT (≥ 300 salariés) : 5 jours / 35h
- **Financement :** Employeur intégral (art. L.2315-18) — ne s'impute pas sur heures de délégation
- **Délai d'accès :** 11 jours ouvrés minimum
- **Délai congé formation :** L'élu prévient l'employeur 30 jours avant (art. L.2315-16)
- **Sanction :** Attestation de fin de formation (non certifiante — hors RNCP/RS)
- **Loi 2026-403 :** Depuis le 28/05/2026, plus soumise à agrément préfectoral — OPTIFORMA intervient sur base NDA + Qualiopi CAP2061
- **Groupe :** 4 à 12 participants

### Formation 04 — SST (PRÉ-INSCRIPTION)
- **Titre :** Sauveteur Secouriste du Travail
- **Statut :** Habilitation INRS / réseau Assurance Maladie en cours (plateforme FORPREV)
- **Formatrice SST :** Nadia BELBOUAB — certificat SST délivré le 02/06/2026
- **Durées prévues :**
  - Formation initiale : 2 jours / 14h
  - MAC SST (renouvellement) : 1 jour / 7h
- **Financement prévu :** OPCO / Plan de développement des compétences
- **Important :** La page formation-sst.html est une page de pré-inscription UNIQUEMENT. Aucune promesse de délivrance de certificat SST tant que l'habilitation INRS n'est pas obtenue. Mention explicite : « Aucune inscription ferme ni paiement à ce stade. »

---

## 6. STRUCTURE CSS (css/style.css + inline index.html)

### Variables CSS globales (`:root`)
```css
--py: clamp(2rem,4.5vw,4rem)   /* padding vertical sections — réduit le 01/07/2026 */
--px: clamp(1.25rem,5vw,5rem)  /* padding horizontal */
--max-w: 1280px
--r-card: 14px
--r-btn: 6px
```

### Classes principales réutilisées sur toutes les pages formation
| Classe | Rôle |
|---|---|
| `.page-header` / `.page-header-inner` | En-tête de page (fond teal dégradé) |
| `.breadcrumb` / `.breadcrumb-sep` / `.breadcrumb-current` | Fil d'Ariane |
| `.fd-intro-ref` | Badge lien France Compétences |
| `.fd-section-wrap` / `.fd-section-inner` | Wrapper deux colonnes contenu + sidebar |
| `.fd-content` | Colonne principale |
| `.fd-sidebar` | Colonne latérale |
| `.fd-block` / `.fd-block-title` | Bloc de contenu avec titre |
| `.fd-objectives` | Liste à puces objectifs |
| `.fd-program` / `.fd-day` / `.fd-day-header` / `.fd-day-num` / `.fd-day-title` / `.fd-day-items` / `.fd-day-item` | Programme jour par jour |
| `.fd-audience-grid` / `.fd-audience-card` | Grille public + prérequis |
| `.fd-infocard` / `.fd-infocard-header` / `.fd-infocard-body` | Carte infos pratiques sidebar |
| `.fd-info-row` / `.fd-info-label` / `.fd-info-value` | Lignes d'info sidebar |
| `.fd-funding-card` / `.fd-funding-title` / `.fd-funding-tags` / `.fd-funding-note` | Carte financement sidebar |
| `.fd-access-card` / `.fd-access-icon` / `.fd-access-text` | Bloc accessibilité |
| `.fd-actions` / `.btn-primary` / `.btn-outline` / `.btn-back` | Boutons d'action sidebar |
| `.cta-section` / `.cta-inner` / `.btn-teal` | Section CTA bas de page |
| `.tag` / `.tag.teal` / `.tag-orange` | Badges colorés |
| `.badge-soon` / `.soon-badge` | Badges "Bientôt disponible" (ambré) |

### Grille homepage formations
```css
.formations-grid { display:grid; grid-template-columns:repeat(2,1fr); gap:1.5rem }
/* Mobile ≤768px → 1 colonne */
```

### Hauteurs réduites (01/07/2026)
| Élément | Avant | Après |
|---|---|---|
| `--py` (sections) | `clamp(3.5rem,7vw,6rem)` | `clamp(2rem,4.5vw,4rem)` |
| Hero padding-top | `clamp(4rem,8vw,7rem)` | `clamp(2rem,4vw,4rem)` |
| Hero img height | `480px` | `360px` |
| Hero h1 font-size | `clamp(2.4rem,4.5vw,3.8rem)` | `clamp(2rem,3.5vw,3.2rem)` |
| Portrait circle | `340px` | `240px` |
| img-pedagogy height | `400px` | `260px` |
| Qualiopi band padding | `3rem 0` | `2rem 0` |
| Footer padding | `3.5rem 0 2rem` | `2.5rem 0 1.5rem` |

---

## 7. NAVBAR & FOOTER — STRUCTURE COMMUNE

### Navbar (identique sur toutes les pages)
```html
<nav id="nav">
  <div class="nav-inner">
    <a href="index.html" class="nav-logo">Opti<span>Forma</span><div class="nav-logo-dot"></div></a>
    <ul class="nav-links">
      <li><a href="formations.html">Formations</a></li>
      <li><a href="financement.html">Financement</a></li>
      <li><a href="qualiopi.html">Qualiopi</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
    <button class="nav-burger" aria-label="Ouvrir le menu" aria-expanded="false">
      <span></span><span></span><span></span>
    </button>
    <a href="contact.html" class="btn btn-teal nav-cta" style="font-size:.82rem;padding:.55rem 1.1rem">
      Demander un devis
    </a>
  </div>
</nav>
```

### Footer — mentions légales complètes
```
© 2025 OPTIFORMA — SASU à capital variable · SIRET 98840369700010
NDA 11950956995 · Enregistré sous le numéro 11950956995.
Cet enregistrement ne vaut pas agrément de l'État. · Qualiopi CAP2061
```

### Bouton Calendly flottant (toutes les pages)
```html
<a href="https://calendly.com/optiforma95/30min" target="_blank" rel="noopener" class="calendly-float">
  📅 Réserver un appel
</a>
```

---

## 8. SITEMAP.XML — ÉTAT ACTUEL

| URL | Priority | Changefreq |
|---|---|---|
| / | 1.0 | weekly |
| /formations.html | 0.9 | weekly |
| /formation-rncp37275.html | 0.9 | monthly |
| /formation-rs6490.html | 0.9 | monthly |
| /formation-ssct.html | 0.9 | monthly |
| /formation-sst.html | 0.7 | monthly |
| /financement.html | 0.8 | monthly |
| /qualiopi.html | 0.8 | monthly |
| /a-propos.html | 0.7 | monthly |
| /blog.html | 0.8 | weekly |
| /contact.html | 0.6 | yearly |
| /blog/* (5 articles) | 0.7 | monthly |
| /cgv.html | 0.3 | yearly |
| /mentions-legales.html | 0.3 | yearly |
| /politique-confidentialite.html | 0.3 | yearly |

---

## 9. HISTORIQUE DES SESSIONS DE TRAVAIL (cette conversation)

### Session du 01/07/2026

| Commit | Description |
|---|---|
| `43626a9` | Création `formation-ssct.html` — page vente active SSCT conforme loi 2026-403 |
| `b36227a` | Création `formation-sst.html` — page pré-inscription SST (habilitation INRS en cours) |
| `51c3cc8` | Mise à jour grille formations `index.html` — SSCT actif + carte SST bientôt disponible |
| `55b2e94` | Réduction hauteur hero et toutes les sections de la page d'accueil |
| `97c99b5` | 01/07/2026 — 4 corrections : harmonisation footers `formation-rncp37275.html`/`formation-rs6490.html` (liens SSCT/SST + mentions légales complètes) · vérification `robots.txt` (déjà conforme, aucun changement) · audit des 3 fichiers legacy non liés (tailles relevées, conservés en l'état) · vérification cohérence grille formations `index.html` (déjà à jour, aucun changement) |

### Détail formation-ssct.html
- Fiche conforme Qualiopi Critère 1 / Indicateur 1
- 5 objectifs pédagogiques
- Programme 5 jours détaillé (J1→J5) + programme renouvellement 3 jours
- Bloc réassurance loi n°2026-403 du 26/05/2026 (fin agrément préfectoral)
- Sidebar : durées légales, délai 11 jours ouvrés, financement employeur intégral
- CTA orange "Demander un devis" + teal "Réserver un créneau"

### Détail formation-sst.html
- Page pré-inscription UNIQUEMENT (pas de vente ferme)
- Contenu au conditionnel/futur
- Encart confiance : Nadia BELBOUAB, certificat SST 02/06/2026, parcours FORPREV
- Formulaire Formspree avec champ caché `formation = "SST - pré-inscription"`
- Mention légale : « Aucune inscription ferme ni paiement à ce stade »

### Modifications index.html
- Grille formations passée de 3 colonnes → 2×2 (responsive)
- Card 3 SSCT : active (suppression classe `soon`)
- Card 4 SST ajoutée : badge ambré, lien "M'alerter →" couleur `#92400e`
- Réduction globale des hauteurs (voir tableau section 7)

---

## 10. POINTS D'ATTENTION & PROCHAINES ÉTAPES

### Urgent / À surveiller
- [ ] **Habilitation SST INRS** : dès obtention → activer la vente sur `formation-sst.html` (retirer le formulaire pré-inscription, ajouter le programme complet et le CTA devis)
- [x] Footers `formation-rncp37275.html` et `formation-rs6490.html` harmonisés avec SSCT/SST — corrigé le 01/07/2026

### SEO & technique
- [ ] Ajouter `og:url` spécifiques par page (actuellement toutes pointent vers `https://opti-forma.fr`)
- [ ] Vérifier la Search Console après les nouveaux ajouts
- [x] `robots.txt` vérifié le 01/07/2026 — déjà présent et conforme (`User-agent: *` / `Allow: /` / `Sitemap: https://opti-forma.fr/sitemap.xml`)

### Contenu
- [ ] Photos de Nadia BELBOUAB : vérifier que les vraies photos sont bien en place sur `a-propos.html`
- [ ] Articles de blog : 5 articles existants — envisager un 6e sur la loi 2026-403 / fin agrément SSCT
- [ ] `formation-evaluer-ameliorer.html` et `formation-formateur-interne.html` : décider si ces pages restent ou sont supprimées

### Légal
- [ ] Vérifier que les CGV (`cgv.html`) mentionnent bien la formation SSCT
- [ ] S'assurer que `mentions-legales.html` est à jour avec NDA + Qualiopi + SASU à capital variable

---

## 11. COMMANDES GIT UTILES

```bash
# Voir l'état
git status
git log --oneline -10

# Déployer (Cloudflare Pages se déclenche automatiquement)
git push

# Revenir à un commit précédent (sans perdre les fichiers)
git checkout <hash> -- <fichier>
```

---

*Audit généré le 01/07/2026 — Opti Forma / OPTIFORMA*
