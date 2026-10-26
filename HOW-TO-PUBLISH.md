# Publishing scn-freelance.com (GitHub Pages + Namecheap)

Folder contents: index.html (company page), mathly/ (app page, privacy.html, support.html, img/), style.css, favicon.png, CNAME, robots.txt, sitemap.xml.

## 1. Put the files online
1. Free account at github.com → New repository → name `scn-freelance` → Public.
2. "uploading an existing file" → drag in EVERYTHING from this folder (including the `mathly` folder and the hidden files `CNAME` and `.nojekyll`; if the hidden ones don't show, they are optional – you can set the domain in step 3) → Commit.
3. Repository Settings → Pages → Source: Deploy from a branch → main, `/ (root)` → Save. Under "Custom domain" type `scn-freelance.com` → Save.

## 2. Connect the domain at Namecheap
Domain List → Manage `scn-freelance.com` → Advanced DNS → delete the default parking records, then add:
| Type | Host | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOURGITHUBUSERNAME.github.io |
(These are GitHub's published Pages addresses – check that they match what GitHub's docs list under "Managing a custom domain", they rarely change.)

Wait 10 min – a few hours. Then in GitHub Pages tick **Enforce HTTPS**.

## 3. Email
The site uses suciu.cristian.nicolae@gmail.com as the contact address, so no mailbox setup is needed.

## 4. Check
Open https://scn-freelance.com , /mathly/ , /mathly/privacy.html , /mathly/support.html – all four should load. Then use the addresses in `PLAY-CONSOLE-ANSWERS.md`.
