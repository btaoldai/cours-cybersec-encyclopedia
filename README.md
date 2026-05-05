# Encyclopédie Cybersécurité — Cartes de révision interactives

Outil de révision open-source pour apprendre et réviser les fondamentaux de la cybersécurité : concepts clés, recommandations ANSSI, acronymes du domaine, RGPD/IoT, cartographie des menaces, et quiz interactif.

**Accès direct (GitHub Pages) :** [btaoldai.github.io/cours-cybersec-encyclopedia](https://btaoldai.github.io/cours-cybersec-encyclopedia)

---

## Contenu

Trois supports complémentaires :

- **Encyclopédie principale** — 84 concepts répartis en 11 familles, 51 recommandations ANSSI issues de 7 guides officiels, 190 abréviations en deux niveaux de difficulté.
- **IoT & RGPD** — 84 concepts dédiés aux objets connectés et à la conformité RGPD, organisés en 10 familles (architecture IoT, sécurité LoRaWAN, données personnelles/sensibles, principes RGPD, droits des personnes, anonymisation/pseudonymisation, etc.).
- **Carte des menaces cyber** — 68 vecteurs d'attaque cartographiés sur 10 catégories (réseau, web, social, cloud, IoT, IA, malware, supply chain, IAM, physique), mappés à MITRE ATT&CK et MITRE ATLAS (pour les techniques IA).

Thèmes couverts : hardening Linux, authentification et gestion des accès, audit et journalisation, architecture réseau et segmentation, sécurité périmétrique, attaques TCP/IP, SIEM et détection d'intrusion, référentiels (ANSSI, CIS, MITRE ATT&CK, MITRE ATLAS, OWASP), RGPD appliqué à l'IoT.

---

## Quiz — 5 modes d'entraînement

- **QCM** — définitions à choix multiples sur les 84 concepts
- **Vrai / Faux** — associations concept ↔ terme anglais à valider
- **Texte libre** — retrouver le terme complet d'un acronyme (190 abréviations)
- **Association** — relier chaque concept à son équivalent anglais par lot de 4
- **Mix** — combinaison aléatoire de tous les types

Options configurables : nombre de questions (5 / 10 / 20 / 30), filtre par session (S1, S2, S3 ou tout), chronomètre activable (30s par question).

Raccourcis clavier : **A / B / C / D** pour les QCM, **V / F** pour Vrai/Faux, **Entrée** pour passer à la question suivante.

---

## Utilisation

**En ligne :** ouvrir l'URL GitHub Pages ci-dessus, aucune installation requise.

**Hors ligne :** télécharger n'importe quelle page de [`pages/`](pages/) et l'ouvrir directement dans un navigateur. Aucune dépendance, aucun serveur, aucun build — tout le contenu est embarqué dans un seul fichier HTML par page.

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
├── index.html                          # Page d'accueil (liens vers les 3 outils)
├── pages/
│   ├── encyclopedie.html               # Encyclopédie principale + Quiz
│   ├── encyclopedie-iot-rgpd.html      # IoT & RGPD + Quiz
│   └── carte-menaces-cyber.html        # Carte interactive des menaces (D3.js)
├── README.md
└── LICENSE                             # CC BY-SA 4.0
```

---

## Licence

**CC BY-SA 4.0** — utilisation libre, y compris commerciale, sous réserve de mentionner l'auteur et de redistribuer sous la même licence.

Référentiels et ressources cités (domaine public ou licences compatibles) :
- ANSSI — guides PG-040 (cloisonnement), PA-066 (DMZ), PA-105 (DNS), BP-033/BP-094 (commutateurs), DAT-NT-007 (OpenSSH), Guide d'hygiène informatique, Guide Authentification & MdP
- MITRE ATT&CK (CC BY 4.0) — techniques d'attaque traditionnelles
- MITRE ATLAS (CC BY 4.0) — techniques adversariales propres à l'IA/ML
- OWASP (CC BY-SA 3.0) — Top 10 et Cheat Sheets

---

## Auteur

**Baptiste Ochlafen** — [TheRustLab](https://github.com/btaoldai)
