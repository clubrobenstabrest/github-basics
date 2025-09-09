## Étape 4, résoudre les conflits et fusionner

{{ status_line }}

### 📖 Qu’est-ce qu’un conflit de fusion ?
Un conflit arrive quand la même portion de code a été modifiée différemment sur `main` et sur ta branche. Git ne sait pas quelle version garder, il te demande de trancher.

### ✅ Cas simple, pas de conflit
- Le message GitHub « **This branch has no conflicts with the base branch** » (ou équivalent en FR) signifie que tu peux **fusionner** directement.
- Clique **Merge pull request** puis **Confirm merge**.

### ⚠️ S’il y a des conflits
Choisis **une** des deux méthodes :

**A. Bouton GitHub (UI)**
1. Clique **Update branch** dans la PR (s’il est proposé).
2. Si des conflits persistent, clique **Resolve conflicts**, édite les fichiers, puis **Mark as resolved** → **Commit merge**.

**B. En ligne de commande (rebase recommandé)**
```bash
# Mets à jour ton dépôt local
git fetch origin

# Va sur ta branche de la PR
git checkout my-first-branch

# Rebase sur main
git rebase origin/main

# Ouvre les fichiers en conflit, supprime les marqueurs <<<<<<< ======= >>>>>>>
# puis valide les résolutions :
git add .

# Continue le rebase
git rebase --continue

# Pousse le résultat (forcé sécurisé)
git push --force-with-lease
