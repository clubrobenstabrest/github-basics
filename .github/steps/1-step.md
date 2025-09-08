## Étape 1, créer une branche

Les branches te permettent de travailler en sécurité, sans toucher à `main`.

### 📖 Théorie, c’est quoi une branche ?

Une branche est un pointeur mobile vers une séquence de commits. Tu peux expérimenter librement, puis fusionner ton travail dans `main` via une pull request.

### ⌨️ Exercice, créer `my-first-branch`

1. Depuis l’onglet **Code**, ouvre le menu des branches, il affiche probablement `main`.
2. Saisis **`my-first-branch`**, clique **Create branch**.
3. Option ligne de commande
   ```bash
   git checkout -b my-first-branch
   ```

<details>
<summary>Un souci ? 🤷</summary><br/>
Assure-toi d’être bien sur la page du dépôt, pas la liste de tes forks.  
En CLI, vérifie que Git est installé, `git --version`.
</details>
