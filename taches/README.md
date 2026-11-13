# Répartition des tâches — Sprint 1 « Module Utilisateurs et Rôles »

**Groupe 7** — AASI 2026 · TP « Améliorer un processus existant »
**Dépôt** : <https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque>
**Tableau Trello** : <https://trello.com/b/tm1lTD6a/backlog>
**Fin de sprint** : dimanche 15 novembre 2026

## Qui fait quoi

| Membre | GitHub | Tâches | Nombre |
|---|---|---|---|
| Emmanuel ADOUNSI | `emmanueladounsi` | Créer un rôle · Attribuer un rôle à un utilisateur · API de gestion des rôles | 3 |
| Obédine MAHUGBE | `obedinemahugbe` | Concevoir le modèle de données · Créer un utilisateur · Modifier un utilisateur | 3 |
| Franck NOUHOEFLIN | `francknouhoeflin743` | API de création des utilisateurs · Désactiver un utilisateur · API d'authentification | 3 |
| Déo-Gratias HOUNNOU | `deogratiashounnou1` | Interface de création des utilisateurs · Interface de connexion | 2 |
| Rayane NACHIROU | `rayannenachirou` | Connexion · Déconnexion | 2 |

Total : **13 cartes** réparties, soit l'intégralité du Sprint Backlog et du « In Progress ».

Les **16 cartes du Product Backlog** (paiement Mobile Money, carte de lecteur numérique, notifications,
tableau de bord, etc.) ne sont volontairement assignées à personne : elles concernent les sprints suivants.

## Fiches individuelles

Seule la fiche du coordinateur est versionnée ici : [emmanuel-adounsi.md](emmanuel-adounsi.md).

Chaque membre rédige et dépose **lui-même** sa fiche (`taches/<prenom>.md`) et sa contribution
(`contributions/<prenom>.md`) sur sa propre branche. C'est ce qui rend la répartition vérifiable
dans l'historique Git : personne n'écrit à la place d'un autre.

## Règles communes

1. **Une branche par personne** : `sprint1/<prenom>`. Personne ne pousse directement sur `main`.
2. **Un fichier par personne** : chacun crée ses propres `taches/<prenom>.md` et
   `contributions/<prenom>.md` (et ses éventuels fichiers de code). Pas de risque de conflit Git.
3. **Pas de `git push --force`**, pas de suppression des fichiers des autres.
4. **Message de commit** : `US — action` (ex. `API rôles : endpoint POST /roles`).
5. En fin de sprint, une **pull request** par personne, relue et fusionnée par Emmanuel.
6. Une carte n'est déplacée en **Done** que si elle est réellement terminée ; sinon elle reste
   en *In Progress* et on note ce qui bloque.

## Mise en route (une seule fois)

1. Accepter l'invitation GitHub reçue par mail (*View invitation* → *Accept invitation*).
2. `git config --global user.name "Prénom NOM"` puis `git config --global user.email "email-du-compte-github"`.
3. `git clone https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque.git`
4. Créer `taches/<prenom>.md` (sa fiche) et remplir `contributions/<prenom>.md`, puis committer les deux.
