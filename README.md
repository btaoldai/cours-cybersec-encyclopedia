# Encyclopedie Cybersecurite

Ressources interactives pour le module **Securite des Infrastructures et Reseaux**.

Chaque page est un outil de revision autonome (HTML standalone) utilisable hors ligne ou heberge via GitHub Pages.


## Pages disponibles

| Page | Description | Seances couvertes |
|---|---|---|
| [Encyclopedie](pages/encyclopedie.html) | 84 concepts, 51 recommandations ANSSI, 198 abreviations — format cartes interactives avec recherche et filtres | S1, S2, S3 |
| RGPD *(a venir)* | Referentiel RGPD applique a la cybersecurite | - |


## Utilisation

**En ligne (GitHub Pages) :**
Acceder directement via `https://<username>.github.io/cours-cybersec-encyclopedia/pages/encyclopedie.html`

**Hors ligne :**
Telecharger le fichier HTML et l'ouvrir dans un navigateur. Aucune dependance externe requise (polices Google Fonts chargees en ligne, mais le contenu reste lisible sans).


## Deploiement GitHub Pages

1. Aller dans **Settings** > **Pages** du depot
2. Source : **Deploy from a branch**
3. Branche : `main`, dossier : `/ (root)`
4. Sauvegarder — le site sera accessible sous quelques minutes

> Ce depot est public. GitHub Pages est actif par defaut pour les depots publics.


## Structure du depot

```
cours-cybersec-encyclopedia/
  pages/
    encyclopedie.html      # Encyclopedie interactive (S1-S3)
  assets/                   # Ressources partagees (images, CSS) — a venir
  README.md
  LICENSE
  .gitignore
```


## Licence

Ce projet est distribue sous licence **Creative Commons Attribution — Partage dans les Memes Conditions 4.0 International (CC BY-SA 4.0)**.

Voir le fichier [LICENSE](LICENSE) pour les details complets.


## Auteur

**Baptiste Ochlafen** — TheRustLab
