# Tâches — Obédine MAHUGBE

**Rôle dans l'équipe** : base de données + cycle de vie du compte utilisateur
**Sprint** : Sprint 1 — Module Utilisateurs et Rôles · **Fin** : dimanche 15 novembre 2026
**Dépôt** : <https://github.com/Emmanuel109-ctrl/test-aasi-> · **Branche** : `sprint1/obedine`

## 1. Tes trois tâches

| Carte Trello | Ce qu'il faut faire | Composant | Lien |
|---|---|---|---|
| **Concevoir le modèle de données utilisateurs** | Tables `utilisateur`, `role` et `utilisateur_role` ; clés primaires, clés étrangères et contraintes (unicité de l'email, suppression logique). | Base de données | <https://trello.com/c/TINhaQeQ> |
| **Créer un utilisateur** | Créer un compte usager ou bibliothécaire : nom, contact, mot de passe (haché), statut actif. | Back-end | <https://trello.com/c/8mkrfz3Z> |
| **Modifier un utilisateur** | Modifier les informations d'un compte existant : nom, contact, mot de passe, sans casser l'historique. | Back-end | <https://trello.com/c/vyKIjeqx> |

⚠️ Ta première tâche conditionne celles de Franck et d'Emmanuel : livre le schéma **en premier**
et préviens l'équipe dès qu'il est poussé.

## 2. Definition of Done

- [ ] le schéma est fourni en SQL versionné (`sql/schema.sql`) ou en diagramme dans le dépôt ;
- [ ] chaque table a une clé primaire, les clés étrangères sont explicites, les contraintes sont nommées ;
- [ ] un jeu de données d'exemple est fourni ;
- [ ] la carte Trello est complétée puis passée en **Done** avec le lien du commit.

## 3. Ce que tu pousses

1. `contributions/obedine-mahugbe.md` — rempli (obligatoire).
2. `sql/schema.sql` et éventuellement `sql/donnees-exemple.sql`.
3. **Rien d'autre** : ne modifie pas les fichiers des autres membres.

## 4. Procédure Git

```bash
git config --global user.name "Obédine MAHUGBE"
git config --global user.email "ton-email-github@exemple.com"

git clone https://github.com/Emmanuel109-ctrl/test-aasi-.git
cd test-aasi-
git checkout -b sprint1/obedine

# ... travail ...

git add .
git commit -m "BDD : schéma utilisateur / role / utilisateur_role"
git push -u origin sprint1/obedine
```

Puis sur GitHub : **Compare & pull request** → base `main` ← `sprint1/obedine` → **Create pull request**.
