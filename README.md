# Developer Portfolio Website

Three files, no build step and no dependencies:

- index.html : page structure (HTML)
- style.css  : design, colours, layout, dark/light theme, responsive rules (CSS)
- script.js  : behaviour and all your content (JavaScript)

Keep the three files in the same folder, then open index.html in a browser.

## 1. Add your details
Open script.js and edit the `const P = { ... }` object at the top.
Name, roles, skills, projects, timeline, education, certifications, resume text and
social links are all defined there. The whole page is built from that object.

## 2. Add your photo
Put your picture in this folder (for example profile.jpg) and in script.js set:

    photo: "profile.jpg",

Leave it empty to show your initials instead.

## 3. Change colours or fonts
Open style.css. The colour tokens are at the top (`:root { --bg, --ink, --accent ... }`).

## 4. Deploy on Vercel

### From GitHub

1. Open https://vercel.com/new and import `ranatbayee-collab/RANAT-KUMAR-PORTFOLIO`.
2. Set **Root Directory** to `RANAT-KUMAR-PORTFOLIO`.
3. Leave **Framework Preset** as `Other`.
4. Leave **Build Command** empty and deploy.

Vercel will serve `index.html` directly. The included `vercel.json` enables clean URLs
and disables trailing slashes.

### From the command line

Run these commands from this folder:

    npx vercel

For production deployment:

    npx vercel --prod

## Notes
- Links that are `#` are placeholders. Replace them with your own.
- The contact form opens the visitor's email app (mailto). For a real form backend,
  use a service such as Formspree or Web3Forms.
- Fonts (Bricolage Grotesque, Figtree) load from Google Fonts.
