# Encyclopédie Cybersécurité — Cartes de révision interactives

Outil de révision open-source pour apprendre et réviser les fondamentaux de la cybersécurité : concepts clés, recommandations ANSSI, acronymes du domaine, et quiz interactif.

**Accès direct (GitHub Pages) :** [btaoldai.github.io/cours-cybersec-encyclopedia](https://btaoldai.github.io/cours-cybersec-encyclopedia)

---

## Contenu

**110 concepts** organisés en 11 familles thématiques, **57 recommandations ANSSI** issues de 7 guides officiels, **156 abréviations** en deux niveaux de difficulté (débutant / intermédiaire).

Thèmes couverts : hardening Linux, authentification et gestion des accès, audit et journalisation, architecture réseau et segmentation, sécurité périmétrique, attaques TCP/IP, SIEM et détection d'intrusion, référentiels (ANSSI, CIS, MITRE ATT&CK, OWASP).

---

## Quiz — 5 modes d'entraînement

- **QCM** — définitions à choix multiples sur les 110 concepts
- **Vrai / Faux** — associations concept ↔ terme anglais à valider
- **Texte libre** — retrouver le terme complet d'un acronyme (156 abréviations)
- **Association** — relier chaque concept à son équivalent anglais par lot de 4
- **Mix** — combinaison aléatoire de tous les types

Options configurables : nombre de questions (5 / 10 / 20 / 30), filtre par session (S1, S2, S3 ou tout), chronomètre activable (30s par question).

Raccourcis clavier : **A / B / C / D** pour les QCM, **V / F** pour Vrai/Faux, **Entrée** pour passer à la question suivante.

---

## Utilisation

**En ligne :** ouvrir l'URL GitHub Pages ci-dessus, aucune installation requise.

**Hors ligne :** télécharger [`pages/encyclopedie.html`](pages/encyclopedie.html) et l'ouvrir directement dans un navigateur. Aucune dépendance, aucun serveur, aucun build — tout le contenu est embarqué dans un seul fichier HTML.

---

## Déploiement GitHub Pages (fork)

1. Forker ce dépôt
2. Aller dans **Settings > Pages**
3. Source : **Deploy from a branch** — branche `main`, dossier `/ (root)`
4. Sauvegarder — le site sera en ligne sous quelques minutes

---

## Structure

```
cours-cybersec-encyclopedia/
├── index.html              # Page d'accueil (liens vers les outils)
├── pages/
│   └── encyclopedie.html   # Application principale (standalone)
├── README.md
└── LICENSE                 # CC BY-SA 4.0
```

---

## Licence

**CC BY-SA 4.0** — utilisation libre, y compris commerciale, sous réserve de mentionner l'auteur et de redistribuer sous la même licence.

Références ANSSI utilisées : PA-022, PG-040, PA-066, BP-033, BP-094, DAT-NT-028 (domaine public).

---

## Auteur

**Baptiste Ochlafen** — [TheRustLab](https://github.com/btaoldai)
