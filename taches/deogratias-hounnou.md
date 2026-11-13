# Tâches — Déo-Gratias HOUNNOU

**Rôle dans l'équipe** : front-end « administration » (écrans du bibliothécaire)
**Sprint** : Sprint 1 — Module Utilisateurs et Rôles · **Fin** : dimanche 15 novembre 2026
**Dépôt** : <https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque> · **Branche** : `sprint1/deogratias`

## 1. Tes deux tâches

| Carte Trello | Ce qu'il faut faire | Composant | Lien |
|---|---|---|---|
| **Développer l'interface de création des utilisateurs** | Formulaire de création de compte côté bibliothécaire : champs, contrôles de saisie, messages d'erreur, confirmation. | Front-end / Usager | <https://trello.com/c/tuZnpJHG> |
| **Développer l'interface de connexion** | Écran de connexion usager / bibliothécaire : champs email + mot de passe, état de chargement, message d'échec. | Front-end / Usager | <https://trello.com/c/oxJVGDyi> |

Tu as deux cartes mais ce sont les plus visibles : ce sont les écrans que le professeur verra en démonstration.

## 2. Definition of Done

- [ ] les deux écrans sont navigables (même avec des données simulées) ;
- [ ] les champs obligatoires sont contrôlés côté client, avec un message clair ;
- [ ] une capture d'écran est ajoutée dans `contributions/preuves/` ;
- [ ] la carte Trello est complétée puis passée en **Done** avec le lien du commit.

## 3. Ce que tu pousses

1. `contributions/deogratias-hounnou.md` — rempli (obligatoire).
2. Tes écrans (HTML/CSS/JS ou maquettes) et tes captures.
3. **Rien d'autre** : ne modifie pas les fichiers des autres membres.

## 4. Procédure Git

```bash
git config --global user.name "Déo-Gratias HOUNNOU"
git config --global user.email "ton-email-github@exemple.com"

git clone https://github.com/Emmanuel109-ctrl/aasi-2026-inscription-bibliotheque.git
cd aasi-2026-inscription-bibliotheque
git checkout -b sprint1/deogratias

# ... travail ...

git add .
git commit -m "Front : formulaire de création de compte + écran de connexion"
git push -u origin sprint1/deogratias
```

Puis sur GitHub : **Compare & pull request** → base `main` ← `sprint1/deogratias` → **Create pull request**.
