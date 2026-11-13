# Tâches — Emmanuel ADOUNSI

**Rôle dans l'équipe** : coordination du sprint + back-end « rôles et droits »
**Sprint** : Sprint 1 — Module Utilisateurs et Rôles · **Fin** : dimanche 15 novembre 2026
**Dépôt** : <https://github.com/Emmanuel109-ctrl/test-aasi-> · **Branche** : `sprint1/emmanuel`

## 1. Tes trois tâches

| Carte Trello | Ce qu'il faut faire | Composant | Lien |
|---|---|---|---|
| **Créer un rôle** | Créer les rôles *usager* et *bibliothécaire* : table `role`, jeu de données initial, règles de nommage. | Back-end / Base de données | <https://trello.com/c/X7cEBRi9> |
| **Attribuer un rôle à un utilisateur** | Associer un rôle à un compte pour définir ses droits d'accès : table de liaison `utilisateur_role`, unicité, date d'attribution. | Back-end | <https://trello.com/c/WFUW821o> |
| **Développer l'API de gestion des rôles** | Endpoints de création d'un rôle, d'attribution et de retrait d'un rôle. Contrôle des doublons et des droits. | Back-end | <https://trello.com/c/WvmIjkUV> |

## 2. Definition of Done

Une carte est terminée quand :

- [ ] le besoin est couvert par du code, du SQL ou un document versionné dans le dépôt ;
- [ ] un cas nominal **et** un cas d'erreur sont décrits (ex. rôle déjà attribué) ;
- [ ] la description de la carte Trello est complétée avec ce qui a été livré ;
- [ ] la carte est passée en **Done** par toi, avec le lien du commit.

## 3. Ce que tu pousses

1. `contributions/emmanuel-adounsi.md` — rempli (obligatoire, c'est la trace individuelle).
2. Tes éventuels fichiers de code / scripts SQL dans `code/` ou `sql/`.
3. **Rien d'autre** : ne modifie pas les fichiers des autres membres.

## 4. Procédure Git

```bash
git config --global user.name "Emmanuel ADOUNSI"
git config --global user.email "emmanueladounsi2@gmail.com"

git clone https://github.com/Emmanuel109-ctrl/test-aasi-.git
cd test-aasi-
git checkout -b sprint1/emmanuel

# ... travail : tu remplis contributions/emmanuel-adounsi.md ...

git add .
git commit -m "API rôles : endpoints POST /roles et /users/{id}/roles"
git push -u origin sprint1/emmanuel
```

Puis sur GitHub : **Compare & pull request** → base `main` ← `sprint1/emmanuel` → **Create pull request**.

## 5. En plus (rôle de coordinateur)

- Relire et fusionner les 4 autres pull requests.
- Vérifier chaque vendredi que les 13 cartes sont à jour sur Trello.
- Remonter tout blocage : une carte bloquée reste en *In Progress* avec un commentaire, elle ne passe pas en *Done*.
