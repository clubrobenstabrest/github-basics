## Étape 4, résoudre les conflits et fusionner

{{ status_line }}

### 📖 Qu’est-ce qu’un conflit de fusion ?
Un conflit arrive quand la même portion de code a été modifiée différemment sur `main` et sur ta branche. Git ne sait pas quelle version garder, il te demande de trancher.

### ✅ Cas simple, pas de conflit
- Le message GitHub « **This branch has no conflicts with the base branch** » signifie que tu peux **fusionner** directement.
- Clique **Merge pull request** puis **Confirm merge**.

### ⚠️ S’il y a des conflits
Choisis **une** des deux méthodes :

**A. Bouton GitHub, UI**
1. Clique **Update branch** dans la PR, si proposé.
2. Si des conflits persistent, clique **Resolve conflicts**, édite, **Mark as resolved**, puis **Commit merge**.

**B. Ligne de commande, rebase recommandé**
```bash
git fetch origin
git checkout my-first-branch
git rebase origin/main

# Résous les conflits, supprime les marqueurs <<<<<<< ======= >>>>>>>
git add .
git rebase --continue

git push --force-with-lease
