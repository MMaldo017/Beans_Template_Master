# The Beans Place: Student Template

Starter project for The Beans Place code-along, built with React, Vite, and Tailwind CSS.

## Prerequisites

- [Node.js](https://nodejs.org/) 20.19+ or 22.12+
- [Git](https://git-scm.com/)

## Getting started

Follow these steps to copy the template into your own GitHub repo. Replace `YOUR-USERNAME` and `YOUR-REPO` with your own details.

### 1. Create an empty repo on GitHub

Click **New repository** and give it a name. **Leave the README, .gitignore, and license options off**, because the repo has to be empty.

### 2. Clone the template

In a terminal, go to the folder where you keep your projects and run:

```bash
git clone https://github.com/MMaldo017/Beans_Template_Master.git beans-place
cd beans-place
```

### 3. Connect it to your own repo

```bash
git remote rename origin upstream
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git remote -v
```

`origin` should now show your repo, and `upstream` should show the class template.

### 4. Push the code to your repo

```bash
git push -u origin main
```

The first time, Git may ask you to sign in to GitHub. Once it finishes, refresh your repo page and the files should be there.

### 5. Install and run the app

```bash
npm install
npm run dev
```

Then open the local URL shown in your terminal (usually http://localhost:5173).

## Saving your work

```bash
git add .
git commit -m "Describe what you changed"
git push
```

## Getting updates from the instructor

Commit your own work first, then run:

```bash
git pull --no-rebase upstream main
git push
```

If you and the instructor changed the same lines, Git will ask you to resolve a merge conflict.

## Common problems

| Problem | Fix |
| --- | --- |
| `Please tell me who you are` when committing | Run `git config --global user.name "Your Name"` and `git config --global user.email "you@example.com"`, then commit again. |
| `failed to push some refs` on step 4 | The GitHub repo probably isn't empty. The easiest fix is to delete it, create it again with the options off, and rerun step 4. |
| `remote origin already exists` | Run `git remote set-url origin https://github.com/YOUR-USERNAME/YOUR-REPO.git` instead of the `git remote add` command. |
| `Permission denied` or `403` when pushing | Run `git remote -v` to check that `origin` is your repo, and that you're signed in to your own GitHub account. |

## Scripts

| Command           | What it does                             |
| ----------------- | ---------------------------------------- |
| `npm run dev`     | Starts the development server            |
| `npm run build`   | Builds the production site into `dist/`  |
| `npm run preview` | Previews the production build            |
| `npm run lint`    | Checks the code with ESLint              |
