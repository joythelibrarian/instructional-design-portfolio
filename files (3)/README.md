# Your Name — Instructional Design Portfolio

A professional portfolio site showcasing eLearning projects, instructional design artifacts, and teaching experience. Built as a static site and hosted free on GitHub Pages.

**Live site:** https://yourusername.github.io

---

## About this site

This repository contains the source for my personal portfolio. The site is built with plain HTML and CSS — no frameworks, no build step — so it's fast, easy to maintain, and easy for anyone to inspect.

The site is organized around five sections:

1. **About** — Who I am and how I got here
2. **eLearning Projects** — Selected courses authored in iSpring Suite, with full case studies
3. **Process Artifacts** — Storyboards, prototypes, outlines, and assessments that demonstrate my design process
4. **Teaching Experience** — Classroom background and how it informs my instructional design work
5. **Contact** — How to reach me

---

## Repository structure

```
yourusername.github.io/
├── index.html              Main landing page
├── style.css               All site styling
├── README.md               This file
├── assets/
│   ├── resume.pdf          Downloadable CV
│   ├── images/             Profile photo, project screenshots
│   ├── storyboards/        Sample storyboard PDFs
│   ├── prototypes/         Sample prototype PDFs
│   ├── outlines/           Sample course outline PDFs
│   └── assessments/        Sample assessment PDFs
└── projects/               Individual case study pages
    ├── project-one.html
    ├── project-two.html
    └── project-three.html
```

---

## Setting it up (first time)

### 1. Create the GitHub repository

On GitHub.com, create a new public repository. **The name must be exactly `yourusername.github.io`** (replacing `yourusername` with your actual GitHub handle). This naming convention tells GitHub Pages to serve it as your main personal site.

### 2. Clone the repo via GitHub Desktop

In GitHub Desktop: **File → Clone Repository**, pick the new repo, and choose where on your computer it should live.

### 3. Add the site files

Copy `index.html`, `style.css`, `README.md`, and the `assets/` folder into the cloned repo folder on your computer.

### 4. Customize the placeholders

Open `index.html` in a text editor and search-replace the following:

| Placeholder | Replace with |
|---|---|
| `Your Name` | Your actual name |
| `YN` | Your initials |
| `your.email@example.com` | Your email |
| `linkedin.com/in/yourprofile` | Your LinkedIn URL |
| `City, State` | Your location |
| `20XX` | Real years for teaching dates |
| `Project Title One/Two/Three` | Real project names |
| `your-form-id` | Your Formspree form ID (see below) |

Also update the project specs (Audience, Duration, Role, Outcome) and teaching descriptions with your real information.

### 5. Drop in your assets

Place real files into the `assets/` subfolders. For each project, you'll want at minimum a hero screenshot. For process artifacts, export your storyboards, outlines, and assessments to PDF so they open in any browser.

### 6. Commit and publish

In GitHub Desktop:

- Review the changed files
- Add a commit message (e.g. "Initial portfolio site")
- Click **Commit to main**
- Click **Push origin**

Then on GitHub.com:

- Go to the repo's **Settings → Pages**
- Confirm the source is set to **Deploy from a branch** → `main` → `/ (root)`
- Wait 1–2 minutes; your site will be live at `https://yourusername.github.io`

---

## Updating the site

The workflow for any future change is the same:

1. Edit the files locally
2. Open GitHub Desktop — it shows what changed
3. Write a short commit message describing the change
4. **Commit to main**, then **Push origin**
5. Changes appear on the live site within about a minute

Good commit messages: "Added Project Four case study", "Updated About section bio", "Replaced resume PDF". Future-you will thank present-you.

---

## Adding a new project case study

The site's project section links to individual case-study pages under `/projects/`. To add a new one:

1. Duplicate `projects/project-one.html` and rename it (e.g. `project-four.html`)
2. Update the content inside
3. Add a new `<article class="project">` block in `index.html` linking to it
4. Drop a hero screenshot into `assets/images/`
5. Commit and push

Recommended case study structure:

- **Problem** — What learning gap or business need prompted this?
- **Audience** — Who were the learners? What was their context?
- **Learning Objectives** — What should learners be able to do after?
- **Design Approach** — ADDIE, SAM, or your variant. Why this approach?
- **Storyboard Sample** — Show a frame or two of the planning work
- **Final Product** — Screenshots or embedded preview of the iSpring output
- **Results** — Completion rates, assessment scores, learner feedback, business impact

This narrative arc is what separates instructional designers from "people who make slides," and hiring managers in this field look for it specifically.

---

## Setting up the contact form

The contact form uses [Formspree](https://formspree.io), which lets you receive form submissions by email without running a backend.

1. Sign up for a free Formspree account
2. Create a new form, pointed at your email address
3. Copy the form's endpoint URL (it looks like `https://formspree.io/f/abcd1234`)
4. In `index.html`, find `action="https://formspree.io/f/your-form-id"` and replace `your-form-id` with the ID from your URL

Formspree's free tier allows 50 submissions per month, which is more than enough for a job-search portfolio.

---

## Hosting alternatives

GitHub Pages is recommended (free, simple, integrated with your existing GitHub Desktop workflow), but the site is portable. The same files will work on:

- **Netlify** — drag-and-drop deploy, custom domains, free
- **Cloudflare Pages** — fast, free, good analytics
- **Vercel** — free for personal sites
- Any traditional web host that serves static files

To use a **custom domain** (like `yourname.com`) with GitHub Pages, buy the domain from any registrar, add a `CNAME` file to this repo containing just the domain name, and update DNS records as GitHub's docs describe.

---

## Browser support

The site uses modern CSS (CSS Grid, custom properties, `aspect-ratio`, `backdrop-filter`) and works in all current versions of Chrome, Firefox, Safari, and Edge. It degrades gracefully on older browsers — the layout reflows, but content stays readable.

The site is responsive and tested at common breakpoints (mobile, tablet, desktop). Reduced-motion preferences are respected.

---

## Credits

Typefaces:
- **Cormorant Garamond** (display) by Christian Thalmann, via Google Fonts
- **Inter Tight** (body) by Rasmus Andersson, via Google Fonts
- **JetBrains Mono** (accents) by JetBrains, via Google Fonts

Designed and built by Your Name. The code is available for reference but the content, photography, and case studies are © Your Name.

---

## Contact

The best way to reach me is email: **your.email@example.com**
