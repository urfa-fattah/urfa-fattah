# GitHub Profile Workflow (step by step)

Goal: turn your GitHub account into a clean mirror of your portfolio at
https://urfa-hasan-fattah.netlify.app/ — CSE student, software development,
cybersecurity, AI/ML, astrophysics.

Time needed: about 90 minutes the first time.

---

## Phase 1 — Profile settings (10 min)

Go to github.com → your avatar → **Settings → Public profile**.

1. **Name:** Urfa Hasan Fattah
2. **Bio (160 chars):** `CSE student @ Netrokona University · Software dev · Cybersecurity · AI/ML · Astrophysics`
3. **Company:** Netrokona University
4. **Location:** Netrokona, Bangladesh
5. **Website:** https://urfa-hasan-fattah.netlify.app/
6. **Social accounts:** add LinkedIn / Facebook / others.
7. **Profile picture:** same photo or avatar as the portfolio, so people recognize you.
8. **Status (smiley on profile):** "Learning DSA & building in public".
9. Settings → **Emails:** tick "Keep my email private" if you do not want it shown.

## Phase 2 — Create the profile README repo (10 min)

1. github.com → **New repository**.
2. Name it **exactly your username** (GitHub shows a "special repository" hint).
3. Set it **Public**, tick **Add a README**.
4. Clone it, then copy this folder's files into it:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.git
cd YOUR_USERNAME
# copy README.md, LICENSE, .github/ from this package into here
git add .
git commit -m "feat: profile README"
git push origin main
```

5. In `README.md`, search for **YOUR_USERNAME** and **TODO** and replace all of them.

## Phase 3 — Enable the snake animation (5 min)

1. In the profile repo: **Settings → Actions → General → Workflow permissions →
   Read and write permissions → Save.**
2. Go to **Actions → Generate Snake Animation → Run workflow.**
3. After it finishes, an `output` branch appears with the SVG files.
   The README already points to them.

## Phase 4 — Clean up your repositories (30 min)

Do this for every existing repo.

1. **Rename** to lowercase-hyphen names (`cse-7-directory`, not `CSE7_Final_v2`).
2. **Add a README** using `templates/PROJECT_README_TEMPLATE.md`.
3. Fill in **About** (description, website, topics) using `templates/REPO_METADATA.md`.
4. Add a **screenshot** to `assets/screenshot.png`.
5. Add a **LICENSE** (MIT is fine for study projects).
6. Archive or delete junk repos (tests, duplicates, empty). Settings → Danger Zone → Archive.
7. Make unfinished projects **private** until they are presentable.

## Phase 5 — Pin and organize (5 min)

1. Profile → **Customize your pins** → choose 6 repos in the order from `templates/REPO_METADATA.md`.
2. Put your strongest, best-documented work first.

## Phase 6 — Build real content for the stats (ongoing)

Your portfolio mentions code, cybersecurity and AI/ML, so the repos should show it.

| New repo | What to put in it |
|---|---|
| `competitive-programming` | C++ solutions grouped by platform (Codeforces, AtCoder, BdMO), with a short note per problem |
| `cybersecurity-notes` | Notes and write-ups from legal practice labs and CTFs (TryHackMe, picoCTF). Never post real targets or live exploit code |
| `ai-ml-learning` | Notebooks following a course; keep each one short and readable |
| `portfolio` | The source of the Netlify site |

Commit small and often. A green graph with real work beats one giant commit.

## Phase 7 — Polish (15 min)

- **Achievements and profile badges** appear automatically as you collect them. Do not chase them.
- **Pull requests:** contribute one small fix or doc improvement to an open-source repo. Use the label `good first issue`.
- **GitHub Pages:** for projects without Netlify, enable Settings → Pages.
- **Security:** enable 2FA (Settings → Password and authentication). Add an SSH key.
- **Contribution settings:** Profile → Contribution settings → tick "Include private contributions".

## Phase 8 — Maintenance routine

- **Weekly:** commit something, however small.
- **Monthly:** update the README project table and remove stale badges.
- **Per semester:** archive old repos, pin your newest best work.

---

## Checklist

- [ ] Name, bio, website, location filled
- [ ] Profile repo `YOUR_USERNAME/YOUR_USERNAME` created and pushed
- [ ] All `YOUR_USERNAME` and `TODO` replaced in README
- [ ] Snake workflow ran once and `output` branch exists
- [ ] Every public repo has README, description, topics, screenshot
- [ ] 6 repos pinned
- [ ] 2FA on
- [ ] Contact links work

## Troubleshooting

| Problem | Fix |
|---|---|
| README not showing on profile | Repo name must equal username exactly, and be public |
| Snake image broken | Run the workflow once; check the `output` branch exists |
| Stats card shows an error | Check username spelling; stats need at least one public repo |
| Profile views badge stuck at 0 | It counts only after the README is live |
