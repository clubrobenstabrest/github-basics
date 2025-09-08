## Step 2: Commit a file

Now make a small change on your branch and commit it.

### 📖 Theory: What is a commit?

A commit records a snapshot of your changes with a message explaining **why** you made them.

### ⌨️ Activity: Edit `playground/README.md`

1. Create (if needed) and edit **`playground/README.md`** on **`my-first-branch`**.
2. Add 2–3 lines introducing yourself. Please include the word **Hello** so the check can confirm your edit.
3. Commit your change.

(Optional CLI)

```bash
mkdir -p playground
printf "Hello, I'm learning GitHub Basics!\n" >> playground/README.md
git add playground/README.md
git commit -m "docs: add a short introduction in playground"
git push origin my-first-branch
```

<details>
<summary>Having trouble? 🤷</summary><br/>

Ensure you’re on `my-first-branch` when editing.  
If committing via the web editor, use a clear message, for example “docs: add intro”.

</details>
