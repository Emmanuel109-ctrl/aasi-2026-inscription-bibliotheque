# AASI 2026 — TP : amélioration du processus d'inscription à une bibliothèque

**Groupe 7** — ADOUNSI Emmanuel · HOUNNOU Déo-Gratias · MAHUGBE Obédine · NACHIROU Rayane · NOUHOEFLIN Franck

## Objet du TP

Appliquer la démarche d'analyse de processus à un processus réel, de la description
jusqu'à la proposition d'amélioration :

1. Décrire le processus (fiche processus)
2. Modéliser l'existant (AS-IS) en BPMN, avec couloirs et passerelles
3. Diagnostiquer : symptômes, goulot d'étranglement, indicateurs, causes
4. Choisir : amélioration continue ou réingénierie
5. Modéliser la version améliorée (TO-BE)
6. Comparer AS-IS et TO-BE dans un tableau

## Processus étudié

**Inscription d'un nouvel usager à une bibliothèque** : permettre à un usager
d'obtenir sa carte de lecteur afin d'emprunter des livres et des documents.

## Contenu du dépôt

| Fichier | Contenu |
|---|---|
| `Fiche-Processus-Inscription-Bibliotheque.docx` | Fiche processus, diagnostic, choix, plan d'action, comparaison AS-IS / TO-BE |
| `schemas/AS-IS.png` | Modèle BPMN de l'existant |
| `schemas/TO-BE.png` | Modèle BPMN de la cible |
| `schemas/AS-IS.drawio` | Source éditable du modèle AS-IS (diagrams.net) |
| `schemas/TO-BE.drawio` | Source éditable du modèle TO-BE (diagrams.net) |

Les fichiers `.drawio` s'ouvrent sur <https://app.diagrams.net> (Fichier → Ouvrir depuis → Appareil).
Ils contiennent exactement le même schéma que les PNG.

## Synthèse

| | AS-IS | TO-BE |
|---|---|---|
| Tâches | 9, séquentielles | 6, dont 2 en parallèle |
| Durée | 20 à 30 min | 5 à 10 min |
| Saisie | Manuelle par le bibliothécaire | Faite par l'usager, contrôlée automatiquement |
| Paiement | Guichet de caisse séparé | Mobile Money, en parallèle de la validation |
| Carte | Remise au guichet | Numérique, envoyée par mail / SMS |

**Goulot d'étranglement (AS-IS)** : la vérification des pièces et la saisie manuelle,
assurées par un seul bibliothécaire, en séquence.

**Choix retenu** : amélioration continue — le processus aboutit, les causes sont
localisées et corrigeables à faible coût, sans refonte complète.

## Points de conception du TO-BE

- **Contrôle automatique de complétude** placé dans le couloir *Système*, avant
  l'intervention du bibliothécaire : le dossier incomplet ne remonte plus au guichet.
- **Paiement Mobile Money en parallèle** de la validation des pièces : les deux
  branches se rejoignent sur une passerelle parallèle, puis le résultat du paiement
  est testé.
- **Deux boucles de retour** vers le formulaire (dossier incomplet, pièces non
  conformes) : l'usager corrige son dossier au lieu d'être refusé.
- **Chemin d'échec du paiement** : la passerelle « Paiement réussi ? » mène à
  « Inscription annulée (compte supprimé) ». Sans ce chemin, le processus resterait
  bloqué à la jonction parallèle.

## Équipe et répartition du travail

| Membre | Rôle | Tâches du sprint 1 |
|---|---|---|
| ADOUNSI Emmanuel | Coordination, back-end rôles | 3 |
| MAHUGBE Obédine | Base de données, cycle de vie du compte | 3 |
| NOUHOEFLIN Franck | Back-end utilisateurs et authentification | 3 |
| HOUNNOU Déo-Gratias | Front-end administration | 2 |
| NACHIROU Rayane | Front-end session usager | 2 |

Le détail est dans [`Taches-Emmanuel-ADOUNSI.md`](Taches-Emmanuel-ADOUNSI.md).
Chaque membre dépose sa propre fiche sur sa branche `sprint1/<prenom>`, puis ouvre une pull request.

## Gestion de projet

Tableau Trello (Scrum) : <https://trello.com/b/tm1lTD6a/backlog>

- **Product Backlog** : fonctionnalités du TO-BE à développer
- **Sprint Backlog** : module Utilisateurs et Rôles
- **Sprint in Progress** : découpage technique du sprint
- **In Progress** : tâches en cours
- **Done** : tâches codées, testées et validées
