# 🎓 Portail Interactif PMP — PMBOK 8 & ECO 2026

Plateforme web interactive de préparation à la certification **PMI-PMP**, développée en SPA (Single-Page Application) 100% front-end.

## 🚀 Fonctionnalités

| Module | Description |
|---|---|
| 📖 **Fiches de Révision** | 12 diapositives interactives (Leçons PMI 1–12), double page Cours + PMBOK 8/ECO 2026, infobulles, glossaire 681 termes |
| 🎯 **Entraînement Examen** | Quiz par domaine (Gens / Processus / Affaires), Examen Blanc 180 Q / 4h, grille de navigation, multi-sélection stricte, historique |
| 🏗️ **Atelier Projet** | Project Builder guidé — 5 phases PMBOK, checklists Prédictif / Agile / Hybride, Builders (Charte, WBS, Risques, Leçons) |

## 📁 Structure du Projet

`
Project Management/
├── index.html                  — Application principale (SPA)
├── exam-questions-data.js      — Base de données Examen (130 questions)
├── glossary-data.js            — Base de données Glossaire (681 termes)
├── vercel.json                 — Configuration Vercel (headers sécurité, rewrites)
└── .gitignore                  — Exclusions Git (PDFs propriétaires, scripts build)
`

## 🖥️ Développement Local

`ash
# Lancer le serveur local
python -m http.server 8000

# Ouvrir dans le navigateur
http://localhost:8000
`

## ☁️ Déploiement Vercel

Ce projet est configuré pour un déploiement automatique via Vercel.

1. Connecter le repository GitHub à Vercel
2. Framework Preset : **Other**
3. Root Directory : . (racine du dépôt)
4. Build Command : *(vide — pas de build requis)*
5. Output Directory : . (racine)

## 📊 Contenu Pédagogique

- **130 questions officielles PMI** réparties en 3 domaines ECO 2026
  - Domaine I — Gens (People) : 40 questions · 33%
  - Domaine II — Processus : 50 questions · 41%
  - Domaine III — Environnement des Affaires : 40 questions · 26%
- **681 termes** du Glossaire officiel PMI (français)
- **12 leçons** couvrant l'intégralité du programme de formation intensive 35h

## ⚖️ Avertissement

> Les ressources documentaires PMI (PDFs des leçons, livres et examens officiels) sont sous copyright PMI et ne sont **pas incluses** dans ce dépôt. Ils sont exclus via .gitignore.

## 🛠️ Stack Technique

- HTML5 / CSS3 / Vanilla JavaScript ES6+
- Tailwind CSS (CDN)
- Font Awesome 6.4 (CDN)
- Google Fonts — Inter
- Persistance : localStorage
