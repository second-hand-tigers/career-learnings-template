# Setup Guide

Steps to turn this template into your own `<your-github-username>-career-learnings` repo. For the *why* behind each convention below — and the full style guide (breadcrumbs, cross-linking, images, naming people in anecdotes, tables) — see [Building Your Own Career-Learnings Network](https://github.com/second-hand-tigers/career-learnings-directory/wiki/Building-Your-Own-Career-Learnings-Network-Repo-and-Wiki). Read that once; it covers everything here in more depth and this guide won't repeat it.

**Placeholders used throughout this template:** `REPLACE-WITH-YOUR-USERNAME` (your GitHub username) and `[Your Name]`. A find-and-replace for both in every file you copy catches them all.

## 1. Create your repo

- Click **Use this template** on [career-learnings-template](https://github.com/second-hand-tigers/career-learnings-template) → **Create a new repository**.
- Name it `<your-github-username>-career-learnings` — anchored to your actual GitHub username, not your full name.
- Set visibility to **Public**. This is required: GitHub Free only allows Wikis on public repos.

## 2. Enable the Wiki

- Settings → Features → check **Wikis**.
- GitHub's "Use this template" button copies the file tree only — it does **not** copy the Wiki, Issues, or Project board — so the wiki pages have to be pasted in by hand from `wiki-templates/`:
  - **Home** — from `wiki-templates/Home.md`. Keep its structure: **Where to Start** (your entry-point pages, bottom line up front), **Other Topics**, **About the Author**, and an empty **Job Aids** table.
  - **_Sidebar** — from `wiki-templates/_Sidebar.md`. Create it from any wiki page via "Add a custom sidebar." It holds the breadcrumb trail plus your Where to Start and Other Topics links.
  - **_Footer** — from `wiki-templates/_Footer.md`. Create it via "Add a custom footer." It repeats the breadcrumb trail so mobile readers, who see the sidebar at the bottom of the page, still have navigation.
- Replace `REPLACE-WITH-YOUR-USERNAME` and `[Your Name]` in all three.
- Once everything is copied in, delete the `wiki-templates/` folder from your own repo — it's scaffolding, not part of your final repo.

## 3. Set up the Project board

- Create a new **Board** (not one of GitHub's curated Team/Sprint templates) with three columns: **Not Started → Drafted → Posted**.
- GitHub's built-in "issue closed → move to Done" automation targets a column literally named **Done**. If you rename that column, either keep a column named "Done" too, or repoint the workflow yourself (Project menu → Workflows → "Item closed").

## 4. Fill in README.md

- Replace `REPLACE-WITH-YOUR-USERNAME`, `[Your Name]`, and every `<!-- TODO -->` block: your topic tables, your About Me bio.
- Keep the order: breadcrumb trail and **Toggle to Page View** link at the top, then **Where to Start**, **Other Topics**, Why This Exists, How This Repo Is Organized, About Me. Readers should reach your content before your mission statement.
- Links in the README go to the repo view (`github.com/...`) for repos, and to `github.com/.../wiki/...` for wiki pages.

## 5. Enable GitHub Pages

- Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder: **/docs**.
- Edit `docs/_config.yml` — set `title` and `description`.
- Edit `docs/index.md` and `docs/about.md` — replace `REPLACE-WITH-YOUR-USERNAME`, `[Your Name]`, and other placeholders, matching what you put in README.md. Leave out any link back to the repo view; the Pages site is for readers, and keeping them on it is deliberate.
- Link rules for the Pages files:
  - Links to the Learning Hub, the directory, or any repo that has Pages turned on use the **Pages URL** (`https://second-hand-tigers.github.io/<repo>/`), so readers stay on the site.
  - Wiki links stay as full `github.com/.../wiki/...` URLs — wikis aren't served by Pages, and relative links resolve differently once served from the Pages site.
- **Leave a blank line before every table, list, or blockquote.** GitHub's renderer tolerates a missing one; Pages doesn't, and it will fold your table into the paragraph above it.
- Confirm it's live at `https://second-hand-tigers.github.io/<your-github-username>-career-learnings/`, and check it on a phone as well as a desktop.

## 6. Add your source material

- Put your original decks, docs, or notes in `/slides`, organized by topic subfolder once you have more than a couple.

## 7. Get listed in the directory

- Ask whoever maintains [career-learnings-directory](https://github.com/second-hand-tigers/career-learnings-directory) to add your repo to its Contributors table, and your entry-point pages to the directory's Where to Start listing.

## Before you write your first wiki page

Read [Building Your Own Career-Learnings Network](https://github.com/second-hand-tigers/career-learnings-directory/wiki/Building-Your-Own-Career-Learnings-Network-Repo-and-Wiki) — it covers the breadcrumb trail, sidebar and footer, cross-linking style, image embedding, and naming conventions every repo in this network uses. Your **topics** are entirely your own; the **structure and style** are what this template and that page exist to standardize.
