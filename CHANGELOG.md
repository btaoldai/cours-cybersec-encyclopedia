# Changelog

Toutes les modifications notables de ce projet sont consignées dans ce fichier.

Le format est basé sur [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/), et ce projet suit le [Semantic Versioning](https://semver.org/lang/fr/).

## [Unreleased]

### Ajouté
- `CHANGELOG.md` — historique structuré des évolutions du contenu pédagogique.
- Référence explicite à **MITRE ATLAS** dans le bloc de licences/sources de la carte des menaces, en complément de MITRE ATT&CK.
- Mention dans la fiche XSS de la fusion des injections (SQLi, XSS, LDAP) dans la catégorie `A03:2021` d'OWASP depuis la révision 2021.
- Précisions historiques pour le cas CCleaner 2017 (rachat de Piriform par Avast en juillet 2017).
- Lien explicite RFC 9293 (TCP, août 2022) avec mention de l'obsolescence de la RFC 793.

### Modifié
- **OWASP Top 10 — XSS** : reclassée de `A07:2021` (incorrect) vers `A03:2021 — Injection` (catégorie réelle depuis 2021). La fiche cible était dans `pages/encyclopedie-iot-rgpd.html`.
- **MITRE ATLAS pour les attaques IA** : 8 fiches (Adversarial Examples, Data Poisoning, Model Inversion, Prompt Injection, Model Stealing, Backdoor IA, Jailbreaking, RAG Poisoning, Agent Hijacking) ne pointent plus vers MITRE ATT&CK mais vers MITRE ATLAS (`AML.Txxxx`), framework dédié aux attaques adversariales sur les systèmes d'IA. Les URL de référence pointent désormais vers `atlas.mitre.org`.
- **Watering Hole** : exemple NotPetya remplacé par Holy Water (2020) et VOHO (2012). NotPetya est un cas supply chain (compromission MAJ MEDoc), pas un watering hole — note explicative ajoutée.
- **DDoS Mirai** : chiffres alignés sur les sources officielles (CISA, Cloudflare, F5) — ~600 000 devices au pic global, ~145 000 mobilisés sur l'attaque OVH (1,1 Tbps), Krebs ~620 Gbps, Dyn cluster distinct (octobre 2016). Cohérence rétablie entre la fiche DDoS et la fiche Recrutement Botnet IoT.
- **HTTP/2 Rapid Reset (CVE-2023-44487)** : unité corrigée de `Mpps` (millions de paquets/s) vers `M req/s` (millions de requêtes/s) — Google a rapporté 398 M req/s en pic applicatif.
- **Adresse IP / CJUE Breyer** : exemple corrigé de `192.168.1.42` (IP privée RFC 1918, hors champ Breyer) vers `82.123.45.6` (IP publique dynamique, vrai cas couvert par l'arrêt CJUE C-582/14 du 19 oct. 2016).
- **AES-128 / Diffusion Restreinte** : description nuancée pour clarifier que le RGS B1 admet AES-128 comme taille minimale, mais que pour le marquage DR (IGI 1300), la qualification produit prime et la plupart des produits qualifiés utilisent AES-256.
- **rsyslog** : reformulation pour lever l'ambiguïté entre rsyslog (le daemon) et la stack de surveillance à 4 niveaux (kernel/auditd → système/rsyslog → applicatif → intégrité/AIDE).
- **mTLS Kubernetes** : précision que le mTLS inter-services dans Kubernetes nécessite un service mesh (Istio, Linkerd) ou Cilium, et n'est pas natif au cluster.
- **Fiche Data Poisoning** : ajout de la référence académique BadNets (Gu et al., 2017) aux côtés du cas grand public Tay (Microsoft, 2016).
- `README.md` : mise à jour complète — chiffres alignés (84 concepts, 51 recommandations ANSSI, 190 abréviations), ajout des deux pages IoT/RGPD et carte des menaces dans la structure et le contenu.
- `index.html` : compteur d'abréviations passé de 198 à 190.

### Corrigé
- **HPKP retirée des recommandations** : la fiche MITM citait HPKP comme contre-mesure ; ce protocole est obsolète depuis 2018 (retiré de Chrome 67-72, Firefox 72, jamais implémenté par Safari/Edge). Remplacé par Certificate Transparency monitoring + CAA records.
- **Acronyme `TFP`** : typo corrigée vers `TFTP` (Trivial File Transfer Protocol, port 69/UDP).
- **RFC TCP** : mise à jour de RFC 793 (1981) vers RFC 9293 (2022), qui obsolète officiellement la 793.

### Supprimé
- 8 abréviations fabriquées ou hors-scope retirées de la liste pour préserver la rigueur du glossaire :
  - `DSOS` (Duty to Secure Our Systems) — acronyme inexistant dans NIS2/RGPD.
  - `ITK` (Insight Segmentation and Registration Toolkit) — librairie d'imagerie médicale, sans lien avec la cybersécurité.
  - `SACT` (Security Assessment and Configuration Tool) — non standard, absent des référentiels reconnus.
  - `SAP` (Systems, Applications, and Products) — ERP, hors-scope cybersécurité d'infrastructure.
  - `TANDBERG` — nom propre d'entreprise (visioconférence), pas un acronyme.
  - `TFSM` (Threat Focused Security Model) — non standard, absent des référentiels reconnus.
  - `VLANF` (VLAN Filtering) — acronyme non standard, le terme courant est juste « VLAN filtering » sans abréviation.
  - `ZEN` (Zen IDS/IPS Ruleset) — ruleset Suricata inexistant ; les rulesets standards sont ET Open, ET Pro et Snort VRT.
- Définitions corrigées (gardées avec sens correct) :
  - `ICP` : « Internet Content Provider » (sens marginal) → « Infrastructure de Clés Publiques » (équivalent français de PKI, sens cyber attendu).
  - `WARP` : « WebAssembly Runtime for Python » (faux) → « Cloudflare WARP » (sens cyber attendu, service VPN/proxy DNS basé sur WireGuard).
  - `SPDY` : précision que ce n'est pas un acronyme strict (prononcé « speedy »), protocole expérimental Google précurseur de HTTP/2.

---

[Unreleased]: https://github.com/btaoldai/cours-cybersec-encyclopedia/compare/HEAD
