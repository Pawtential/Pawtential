# Pawtential — Play With Purpose

A standalone, responsive static website for Pawsibilities Ranch and its four public Discord bots. **No Bark-Caster connection, database, server, or API key is needed.**

## Publish on GitHub Pages
1. Create a GitHub repository (a new repository lets your old PackTracker site remain live).
2. Upload **all the contents** of this folder to the repository root, including `index.html`, `dogs.json`, and the `assets` folder.
3. In repository **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)` and save.
4. Open the Pages URL and test on both your phone and computer. Pages may take a few minutes to deploy.

## Update rescue dogs yourself
Read **EDITING-DOG-PROFILES.md** for step-by-step instructions. All 19 current approved profiles and their photos are already included. `dogs.json` is the sole profile list; the website reads it each time the Meet the Pack page loads. No Bark-Caster connection is used.

## What works out of the box
- Responsive desktop and mobile pages, including collapsible mobile navigation.
- All 19 rescue dog profiles: 14 adoptable and 5 sanctuary, with full stories and local photos.
- Dog name/story search and adoptable/sanctuary filter.
- Four public bot showcases and clearly labeled simulated demos.
- Pawzmo's simple on-site FAQ guide; donation links; click-to-email/contact form using visitor's email app; phone/text links.
- Draft privacy, terms, and data-deletion policies; see `legal-review.html` for items to confirm.

## Before publishing publicly
- Confirm each dog's current adoption/sanctuary status.
- Confirm any pricing, Premium checkout terms, data retention and legal disclosures in the policy drafts.
- Add verified invite URLs for PackTracker, Sticker Hunt and Prize Park. Yap-Caster's supplied invite URL is included.
- The contact form opens an email app; it does not send email directly or send SMS alerts. The donation buttons open external providers; no payment processing happens on this site.

## Security and privacy
Only put **publicly approved** dog details and photos into `dogs.json` and `assets/dogs`. Everything committed to a public GitHub Pages repository is publicly accessible. Never upload bot tokens, passwords, Discord staff transcripts, private adopter data, or database files.


## Flat GitHub upload
All files are in one directory. Extract the ZIP, select all files inside, and drag them into the root of the GitHub repository. Do not upload the ZIP itself.
