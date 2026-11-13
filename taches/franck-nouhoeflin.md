# Tâches — Franck NOUHOEFLIN

**Rôle dans l'équipe** : back-end utilisateurs et authentification
**Sprint** : Sprint 1 — Module Utilisateurs et Rôles · **Fin** : dimanche 15 novembre 2026
**Dépôt** : <https://github.com/Emmanuel109-ctrl/test-aasi-> · **Branche** : `sprint1/franck`

## 1. Tes trois tâches

| Carte Trello | Ce qu'il faut faire | Composant | Lien |
|---|---|---|---|
| **Développer l'API de création des utilisateurs** | Endpoint `POST /users` : validation des données, email unique, mot de passe haché, gestion des doublons. | Back-end | <https://trello.com/c/b4xQ0XJo> |
| **Désactiver un utilisateur** | Désactivation logique du compte (drapeau `actif`), sans supprimer l'historique ni les emprunts. | Back-end | <https://trello.com/c/3ogSj5NP> |
| **Développer l'API d'authentification** | Endpoint `POST /login` : vérification du mot de passe, jeton JWT, expiration et gestion des sessions. | Back-end | <https://trello.com/c/WBFjofDt> |

## 2. Definition of Done

- [ ] chaque endpoint répond en JSON, avec les codes HTTP attendus (200/201/400/401/404/409) ;
- [ ] les entrées sont validées et les erreurs renvoyées de façon lisible ;
- [ ] une collection de tests (Postman ou `curl`) est versionnée dans `api/` ;
- [ ] la carte Trello est complétée puis passée en **Done** avec le lien du commit.

## 3. Ce que tu pousses

1. `contributions/franck-nouhoeflin.md` — rempli (obligatoire).
2. Ton code d'API et ta collection de tests.
3. **Rien d'autre** : ne modifie pas les fichiers des autres membres.

## 4. Procédure Git

```bash
git config --global user.name "Franck NOUHOEFLIN"
git config --global user.email "ton-email-github@exemple.com"

git clone https://github.com/Emmanuel109-ctrl/test-aasi-.git
cd test-aasi-
git checkout -b sprint1/franck

# ... travail ...

git add .
git commit -m "API : POST /users et POST /login (JWT)"
git push -u origin sprint1/franck
```

Puis sur GitHub : **Compare & pull request** → base `main` ← `sprint1/franck` → **Create pull request**.
