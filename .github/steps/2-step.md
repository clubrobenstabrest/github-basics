## Étape 2, committer un fichier

Fais une petite modification sur ta branche et crée un commit.

### 📖 Théorie, c’est quoi un commit ?

Un commit enregistre un instantané de tes changements, avec un message qui explique **pourquoi**.

### ⌨️ Exercice, éditer `playground/README.md`

1. Crée si besoin et édite **`playground/README.md`** sur **`my-first-branch`**.
2. Ajoute 2–3 lignes pour te présenter, **incluant le mot Hello**.
3. Committe ta modification.

Option ligne de commande
```bash
mkdir -p playground
printf "Hello, j'apprends GitHub Basics !\n" >> playground/README.md
git add playground/README.md
git commit -m "docs: ajouter une courte présentation dans playground"
git push origin my-first-branch
```

<details>
<summary>Un souci ? 🤷</summary><br/>
Assure-toi d’être sur `my-first-branch` pour éditer.  
Dans l’éditeur web, mets un message clair, par exemple “docs: add intro”.
</details>