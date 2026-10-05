# Trackr   <!--utilisateur/new dev-->
Suivre tous ses colis au même endroit : recherche par numéro de suivi,
statut et date de livraison estimée. Application fictive réalisée par
l'équipe 5 (Ynov Val d'Europe, Bachelor 2, 2026-2027). 

## Installation   <!--utilisateur/new dev-->
Prérequis : Node.js 22 ou plus (`node -v`), Git.
```bash
git clone https://github.com/Alexanger300/trackr-equipe-5.git
cd trackr-equipe-5
npm install
npm run dev
```
L'application s'ouvre sur http://localhost:5173 avec 6 colis.

## Utilisation  <!--utilisateur/new dev-->
| Commande | Effet |
|-------------------|-------------------------------------------------|
| `npm run dev` | Serveur de développement avec rechargement |
| `npm run build` | Vérifie les types, construit la version dans dist/ |
| `npm run preview` | Sert la version construite |
| `npm run lint` | Analyse le code (oxlint) |
Les données sont fictives : `src/data/colis.ts` (6 colis de démonstration).

## Architecture <!--new dev/ equipe-->
```
src/
├── App.tsx état de la page (recherche, filtre) et assemblage
├── components/ composants d'affichage (CarteColis, ListeColis…)
├── data/colis.ts colis de démonstration
├── utils/ fonctions sans effet de bord (recherche, dates, tri)
└── types.ts types Colis et Statut
├── main.tsx donne autorisations sur l application( lance app.tsx)
```
Les décisions techniques sont expliquées dans [docs/adr/](docs/adr/).

## Contribuer  <!--new dev-->
Une issue, une branche `type/numéro-sujet`, une Pull Request relue  <!--utilisateur-->
(1 Approve obligatoire). Détails : [CONTRIBUTING.md](CONTRIBUTING.md).
