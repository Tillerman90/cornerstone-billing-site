# Cornerstone Billing Solutions website

A simple static site: plain HTML and CSS. No build step, no frameworks, no accounts needed beyond GitHub and a domain registrar.

## Files
- `index.html` : all page content. Text is easy to find and edit.
- `styles.css` : colors and fonts are at the top (`:root`).
- `favicon.svg` : browser tab icon.
- `assets/` : `logo.png` (header logo) and `allie.jpg` (headshot). Swap in higher-resolution versions with the same file names any time.

## Edit the site
On GitHub, open a file, click the pencil icon, edit, and click **Commit changes**. The site updates in about a minute.

## Publish with GitHub Pages
1. Repo **Settings > Pages**.
2. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Under **Custom domain**, enter the domain (for example `cornerstonebilling.com`) and save.
4. Tick **Enforce HTTPS** once it becomes available.

## Connect the custom domain
At the domain registrar, add these DNS records:
- Four `A` records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- One `CNAME` record for `www` pointing to `<github-username>.github.io`

Verify these against GitHub's current docs before setting up. DNS can take a few hours to update.

## Handoff checklist
- [ ] Allie owns the GitHub account (or the repo has her as owner)
- [ ] Allie owns the domain registration, in her name
- [ ] Allie has the logins stored in a password manager
- [ ] Contact form (optional): sign up at formspree.io and swap the email button for a form
- [ ] Business email on the domain (optional): Google Workspace or Zoho
