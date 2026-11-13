# Tâches — Rayane NACHIROU

**Rôle dans l'équipe** : front-end « parcours usager » (session)
**Sprint** : Sprint 1 — Module Utilisateurs et Rôles · **Fin** : dimanche 15 novembre 2026
**Dépôt** : <https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque> · **Branche** : `sprint1/rayane`

## 1. Tes deux tâches

| Carte Trello | Ce qu'il faut faire | Composant | Lien |
|---|---|---|---|
| **Connexion** | Connexion par email et mot de passe : appel de l'API, stockage du jeton, redirection vers l'espace selon le rôle. | Front-end / Usager | <https://trello.com/c/1FbGy4ZU> |
| **Déconnexion** | Fermer la session en cours : suppression du jeton, retour à l'écran de connexion, blocage du retour arrière. | Front-end / Usager | <https://trello.com/c/YJS8ns6Y> |

Tu travailles avec Déo-Gratias sur le même écran : mettez-vous d'accord sur les identifiants
des champs (`#email`, `#mot-de-passe`) avant de coder, pour éviter deux versions incompatibles.

## 2. Definition of Done

- [ ] la connexion appelle réellement l'API et gère le cas « mauvais mot de passe » ;
- [ ] la déconnexion vide le jeton et empêche l'accès aux pages protégées ;
- [ ] une capture d'écran est ajoutée dans `contributions/preuves/` ;
- [ ] la carte Trello est complétée puis passée en **Done** avec le lien du commit.

## 3. Ce que tu pousses

1. `contributions/rayane-nachirou.md` — rempli (obligatoire).
2. Ton code de session (JS) et tes captures.
3. **Rien d'autre** : ne modifie pas les fichiers des autres membres.

## 4. Procédure Git

```bash
git config --global user.name "Rayane NACHIROU"
git config --global user.email "ton-email-github@exemple.com"

git clone https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque.git
cd aasi-2026-inscription-bibliotheque
git checkout -b sprint1/rayane

# ... travail ...

git add .
git commit -m "Front : session utilisateur (connexion / déconnexion)"
git push -u origin sprint1/rayane
```

Puis sur GitHub : **Compare & pull request** → base `main` ← `sprint1/rayane` → **Create pull request**.
