# Setup Guide

Steps to turn this template into your own `<your-github-username>-career-learnings` repo. For the *why* behind each convention below — and the full style guide (breadcrumbs, cross-linking, images, naming people in anecdotes, tables) — see [Building Your Own Career-Learnings Network](https://github.com/second-hand-tigers/career-learnings-directory/wiki/Building-Your-Own-Career-Learnings-Network-Repo-and-Wiki). Read that once; it covers everything here in more depth and this guide won't repeat it.

## 1. Create your repo

- Click **Use this template** on [career-learnings-template](https://github.com/second-hand-tigers/career-learnings-template) → **Create a new repository**.
- Name it `<your-github-username>-career-learnings` — anchored to your actual GitHub username, not your full name.
- Set visibility to **Public**. This is required: GitHub Free only allows Wikis on public repos.

## 2. Enable the Wiki

- Settings → Features → check **Wikis**.
- Create the Home page using `wiki-templates/Home.md` in this repo as your starting point — GitHub's "Use this template" button copies the file tree only, it does **not** copy the Wiki, Issues, or Project board, so this has to be pasted in by hand.
- Once you've copied it in, delete the `wiki-templates/` folder from your own repo — it's scaffolding, not part of your final repo.

## 3. Set up the Project board

- Create a new **Board** (not one of GitHub's curated Team/Sprint templates) with three columns: **Not Started → Drafted → Posted**.
- GitHub's built-in "issue closed → move to Done" automation targets a column literally named **Done**. If you rename that column, either keep a column named "Done" too, or repoint the workflow yourself (Project menu → Workflows → "Item closed").

## 4. Fill in README.md

- Replace every `<!-- TODO -->` block and bracketed placeholder: your name, your topics table, your About Me bio, your CTA links at the top.

## 5. Enable GitHub Pages

- Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder: **/docs**.
- Edit `docs/_config.yml` — set `title` and `description`.
- Edit `docs/index.md` and `docs/about.md` — replace placeholders, matching what you put in README.md. Wiki links in these files need to be full `github.com` URLs, not relative links — relative links resolve differently once served from the Pages site.
- Confirm it's live at `https://second-hand-tigers.github.io/<your-github-username>-career-learnings/`.

## 6. Add your source material

- Put your original decks, docs, or notes in `/slides`, organized by topic subfolder once you have more than a couple.

## 7. Get listed in the directory

- Ask whoever maintains [career-learnings-directory](https://github.com/second-hand-tigers/career-learnings-directory) to add your repo to its Contributors table.

## Before you write your first wiki page

Read [Building Your Own Career-Learnings Network](https://github.com/second-hand-tigers/career-learnings-directory/wiki/Building-Your-Own-Career-Learnings-Network-Repo-and-Wiki) — it covers the breadcrumb pattern, cross-linking style, image embedding, and naming conventions every repo in this network uses. Your **topics** are entirely your own; the **structure and style** are what this template and that page exist to standardize.
