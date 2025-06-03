
# Contributing Guide

Hi! This guide helps us collaborate smoothly on this project. Please read and follow these steps when working in this repository.

## 📁 Repository Structure

- `data/` — Raw and cleaned datasets
- `code/` — Analysis and preprocessing scripts
- `output/` — Figures and tables
- `products/` — Drafts, notes, and paper sections
- `README.md` — Project description and setup instructions

## 👥 Workflow

### 1. Clone the repo (first time only)
```bash
git clone https://github.com/silviateliz/jeon_teliz.git
cd jeon_teliz
```

### 2. Always start by pulling from the `main` branch

```bash
git checkout main
git pull origin main
```

### 3. Create a branch for the task you're working on

Use a clear name that describes the task for which you are using the branch. For example:

```bash
git checkout -b feature/summary-stats
```

Other examples:

* `analysis/text-analysis`
* `fix/typo-in-readme`
* `doc/paper-draft`

### 4. Commit regularly with clear messages

Use present tense and describe what you did:

```bash
git commit -m "feat: Add descriptive plots"
```

Use the following format for the commit message: 
> type: description in present tense

The most common commit types are:
* feat: for adding new features (code, files, etc.)
* docs: for adding files or modifying file paths
* fix: for quick fixes 


### 5. Push your branch

```bash
git push origin feature/summary-stats
```

### 6. Open a Pull Request (PR)

A **Pull Request** (PR) is how we propose and review changes to the project before merging them into the `main` branch. Think of it as saying:

> “Hey, I’ve made some changes on a separate branch — can you review and approve them before they go into the main project?”

Here’s how to open one:

1. Push your branch to GitHub:
   ```bash
   git push origin feature/your-branch-name
    ```

2. Go to the GitHub page for the repo. GitHub will usually prompt you with a green button that says
   **"Compare & pull request"** — click that.

3. In the PR page:

   * **Title**: Describe what the branch does (e.g., *"Add regression plots by skin tone"*).
   * **Description**: Give a brief explanation of the work you’ve done.

     * What was the goal?
     * Any specific decisions or issues you encountered?
     * Anything the reviewer should test?

4. If you're ready for review, **assign your collaborator** or tag them with `@username`.

5. Once reviewed and approved (or if you're working solo and just double-checking), click:

   * **"Squash and merge"**: Combines all your commits into one for a cleaner history (recommended).
   * **"Rebase and merge"**: Keeps the linear history of the project.
   * Avoid **"Create a merge commit"** unless there’s a specific reason.

6. After merging, **delete your branch** to keep the repo clean. GitHub will offer a button to do this.



### 7. Review and Merge

* Check for conflicts (GitHub will alert you)
* Merge using **"Squash and merge"** or **"Rebase and merge"** for a clean history

## 🛑 Avoid Committing These

* Large raw data files, like images
* `.Rhistory`, `.ipynb_checkpoints/`, `.DS_Store`
* Sensitive or personal information

These files are listed in `.gitignore`, so they are ignored by default.

## ✅ Tips for Smooth Collaboration

* Pull frequently: `git pull origin main`
* Communicate via GitHub Issues or directly (Slack, WhatsApp, etc.)
* Use Issues to track ideas, bugs, or to-dos
* Tag your coauthor on GitHub PRs if you want feedback
