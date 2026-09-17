


# ⚡ Énergie Hydraulique Renouvelable · 7 Simulations Interactives

> Un simulateur éducatif 100 % web de systèmes hydrauliques de production et de transfert d'énergie — sans aucune dépendance, dans un seul fichier HTML.

🌐 **Démo en ligne** : [gunout.github.io/energie-hydraulique-renouvelable](https://gunout.github.io/energie-hydraulique-renouvelable/)

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-déployé-0055A4?logo=github&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-EF4135?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-4d9fff?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?logo=javascript&logoColor=black)
![Licence](https://img.shields.io/badge/licence-MIT-white)

---

## 📖 Présentation

Cette application propose **7 simulations animées et interactives** de circuits hydrauliques : turbines, pompes, béliers hydrauliques, STEP (stations de transfert d'énergie par pompage) et circuits fermés.

Chaque simulation affiche en temps réel :

- 💧 les **niveaux des réservoirs**
- 🔄 les **débits de circulation** (L/s)
- ⚡ les **puissances produites / consommées** (kW ou MW)
- 📊 le **bilan énergétique net** et l'énergie cumulée

Le tout dans une interface sombre avec schémas SVG animés, curseurs de réglage, pause/reset, et navigation par onglets.

---

## 🗂️ Les 7 simulations

| # | Simulation | Description |
|---|------------|-------------|
| 1 | **STEP réversible** | Deux réservoirs à altitudes différentes, turbine/pompe réversible, mode automatique turbine ⇄ pompe |
| 2 | **Bélier hydraulique** | Remontée d'eau sans électricité grâce au coup de bélier — cycle en 4 phases animé (accélération, martèlement, refoulement, détente) |
| 3 | **Double réseau + pompe** | Deux réservoirs de même hauteur, réseau gravitaire A→B et refoulement B→A par pompe — *bilan physique honnête (négatif)* |
| 4 | **Double réseau + bélier** | Même architecture, refoulement assuré par un bélier hydraulique (~20 % du débit) |
| 5 | **Circuit fermé gravitaire** | Boucle fermée turbine + pompe, niveaux constants, aucun apport d'eau |
| 6 | **Croix "X" optimisée** | Réseaux croisés perpendiculaires (±45°), turbine T1 en haut, pompe T2 au point bas |
| 7 | **Circuit fermé · Tricolore 🇫🇷** | Réseaux parallèles bleu (turbine A→B) / rouge (pompe B→A), énergie en blanc — édition bleu-blanc-rouge |

---

## ✨ Fonctionnalités

- 🎛️ **Réglages en direct** : charge des turbines, ouverture des vannes, débits
- 🎬 **Animations SVG** : écoulements, rotors, vagues, vannes, manomètres
- 📐 **Physique simplifiée mais cohérente** : P = ρ·g·Q·H·η, rendements en cloche
- 🧩 **Isolation par iframes** : chaque simulation tourne indépendamment, sans conflit d'identifiants
- 📱 **Responsive** : layout adaptatif desktop / mobile
- 🚫 **Zéro dépendance** : pas de framework, pas de build, pas de requête réseau

---

## 🛠️ Technologies

| Élément | Choix |
|---------|-------|
| Structure | HTML5 sémantique + `<template>` |
| Style | CSS3 pur (variables, gradients, animations) |
| Logique | JavaScript vanilla (ES6+, `requestAnimationFrame`) |
| Schémas | SVG inline animés |
| Isolation | iframes `srcdoc` générées dynamiquement |

---

## 🚀 Lancer localement

Aucune installation nécessaire :

    git clone https://github.com/gunout/energie-hydraulique-renouvelable.git
    cd energie-hydraulique-renouvelable
    # ouvrez index.html dans votre navigateur

Ou avec un serveur local :

    python -m http.server 8000
    # puis http://localhost:8000

---

## 🌍 Déploiement GitHub Pages

Le site est déployé automatiquement depuis la branche `main` :

1. `Settings` → `Pages`
2. Source : `Deploy from a branch` → `main` / `(root)`
3. L'application est disponible sur <https://gunout.github.io/energie-hydraulique-renouvelable/>

---

## ⚠️ Note physique importante

Certaines simulations (notamment les **circuits fermés « auto-entretenus »**, onglets 5, 6 et 7) présentent un bilan énergétique **positif à des fins de démonstration visuelle**.

> 🔬 **Dans la réalité**, une pompe consomme toujours *plus* d'énergie qu'une turbine n'en produit sur le même circuit (rendements cumulés < 100 %, second principe de la thermodynamique). La simulation 3 affiche honnêtement ce bilan négatif. Ce projet est **pédagogique et visuel**, pas un plan de machine à énergie infinie. 😉

---

## 📁 Structure

    energie-hydraulique-renouvelable/
    ├── index.html          # Application complète (7 simulations + moteur)
    └── README.md

---

## 🤝 Contribuer

Les idées d'amélioration sont bienvenues :

- ➕ nouvelles simulations (pompe à chaleur, vannes marémotrices…)
- 🎨 mode clair / thèmes
- 🔊 sons et effets
- 📈 graphiques temporels des bilans

Ouvrez une *issue* ou soumettez une *pull request* !

---

## 📄 Licence

Distribué sous licence **MIT**. Voir [LICENSE](LICENSE) pour plus de détails.

---


## SCREENSHOTS 

<img width="1800" height="1024" alt="Screenshot 2026-09-17 at 22-44-53 7 Simulations · Énergie Hydraulique Renouvelable" src="https://github.com/user-attachments/assets/046c6126-61dd-490b-a80a-565990b37520" />

---

<div align="center">

### 🇫🇷 Gunout · 2026

![Made in France](https://img.shields.io/badge/Made_in-France-002395?style=flat-square&labelColor=FFFFFF&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5MDAgNjAwIj48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjYwMCIgZmlsbD0iIzAwMjM5NSIvPjxyZWN0IHdpZHRoPSI5MDAiIGhlaWdodD0iNDAwIiB5PSIxMDAiIGZpbGw9IiNmZmYiLz48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjIwMCIgeT0iNDAwIiBmaWxsPSIjZWQyOTM5Ii8+PC9zdmc+)
![GitHub](https://img.shields.io/badge/GitHub-gunout-181717?style=flat-square&logo=github&logoColor=white)
![Year](https://img.shields.io/badge/2026-ED2939?style=flat-square&labelColor=FFFFFF)

<sub>© 2026 <strong>gunout</strong> — Tous droits réservés.</sub>

</div>
