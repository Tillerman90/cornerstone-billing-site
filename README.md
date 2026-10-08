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

## Connect the custom domain (cornerstoneaiabilling.com, registered at Namecheap)
GitHub recommends verifying the domain first, then adding it to the repo, then changing DNS.

1. **Verify the domain:** GitHub profile picture > **Settings > Pages > Add a domain**. Enter `cornerstoneaiabilling.com`. GitHub shows a TXT record.
2. In Namecheap: **Domain List > Manage > Advanced DNS**. Add that TXT record, then click **Verify** in GitHub.
3. **Add it to the repo:** repo **Settings > Pages > Custom domain**, enter `cornerstoneaiabilling.com`, save.
4. **DNS records in Namecheap (Advanced DNS):** delete any parking-page or redirect records Namecheap added, then add:
   - `A Record`, host `@`, value `185.199.108.153`
   - `A Record`, host `@`, value `185.199.109.153`
   - `A Record`, host `@`, value `185.199.110.153`
   - `A Record`, host `@`, value `185.199.111.153`
   - `CNAME Record`, host `www`, value `<github-username>.github.io.` (no repo name)
5. Wait for the DNS check in GitHub Pages to pass (minutes to 24 hours), then tick **Enforce HTTPS**.

Values from GitHub's docs, "Managing a custom domain for your GitHub Pages site."

## Handoff checklist
- [ ] Allie owns the GitHub account and the repo
- [ ] Allie owns the domain at Namecheap, in her name
- [ ] Logins stored in a password manager, two-step login turned on
- [ ] Andrew added back as a collaborator (optional)

## Waiting on Allie
- About text (replace the two paragraphs in the About section of `index.html`)
- Testimonial approvals (5 quotes in the value proposition deck)
- Payment-cycle chart images (deck slides 9 and 10)
- Higher-resolution logo
- Calendly link (optional; replace the `mailto:` link on the contact button)
