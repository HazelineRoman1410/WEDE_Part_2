# Mastercard Foundation Website — Part 2

## Student Information

- **Name:** Zintle Hazel Roman
- **Student Number:** ST10438046
- **Module:** Web Development (WEDE5020)
- **Part:** Part 2 — CSS Styling and Responsive Design
- **Academic Year:** 2026

## Project Overview

This project is a multi-page informational website for the Mastercard Foundation. The website presents information about the Foundation, its programmes and services, opportunities for enquiries, a gallery, and contact information.

Part 2 builds on the HTML website submitted in Part 1 by moving the styling into a shared external CSS stylesheet and improving the desktop, tablet, and mobile layouts.

## Part 1 Feedback Addressed

The Part 1 marking rubric recorded a total of **82/100**. The following feedback has been specifically addressed in Part 2:

| Part 1 feedback | Part 2 action |
|---|---|
| File and folder management must be corrected. | Reorganised the website into a clean root folder with six HTML pages and a dedicated `css/` folder. |
| Fix the broken navigation to the home page. | Renamed the homepage to `index.html` and updated navigation links so all pages point to the correct homepage. |
| GitHub repository was not provided. | The project is prepared for Git/GitHub. The repository URL must be added by the student after creating/pushing the repository. |
| Part 2 requires CSS and responsive design. | Added a shared external `css/style.css` file, desktop styling, tablet/mobile breakpoints, relative units, focus states, and responsive layouts. |

## Website Goals and Objectives

- Increase awareness of the Mastercard Foundation's mission and programmes.
- Provide clear information about services and programmes.
- Allow visitors to submit volunteer or sponsorship enquiries.
- Showcase the Foundation's work through the gallery page.
- Provide contact information and office-location information.
- Present the website clearly across desktop, tablet, and mobile screen sizes.

## Pages

1. **Home (`index.html`)** — Hero section, impact statistics, services preview, and mission content.
2. **About (`about.html`)** — Foundation background, Scholars Program information, mission/vision content, and timeline.
3. **Services (`services.html`)** — Detailed programme/service information.
4. **Enquiry (`enquiry.html`)** — Volunteer and sponsorship enquiry form.
5. **Gallery (`gallery.html`)** — Gallery content, video section, and partner information.
6. **Contact (`contact.html`)** — Contact form and office-location information.

## Part 2 CSS Features

### External Stylesheet

All six HTML pages are linked to:

```text
css/style.css
```

The stylesheet contains the shared visual design and responsive rules rather than page-specific inline `<style>` blocks.

### Base Styling

The stylesheet includes:

- CSS reset
- `box-sizing: border-box`
- Consistent typography
- CSS custom properties for the colour palette
- Consistent spacing and layout
- Shared navigation and footer styling
- Buttons and interactive states
- Form styling

### Layout

CSS Grid and Flexbox are used where appropriate for:

- Homepage hero section
- Statistics
- Services
- About-page content
- Gallery
- Partner section
- Contact layout
- Forms
- Footer and navigation

### Responsive Design

The website includes breakpoints for:

- Desktop
- Tablet: `max-width: 1024px`
- Mobile: `max-width: 768px`
- Small phones: `max-width: 480px`

Responsive changes include:

- Multi-column layouts changing to single-column layouts.
- Navigation wrapping and adapting to smaller screens.
- Responsive typography using relative sizing and `clamp()`.
- Responsive spacing and content widths.
- Gallery and partner grids adapting to available screen width.
- Full-width buttons on small screens.
- Images, SVGs, and embedded content constrained to their containers.

### Accessibility and Usability Improvements

- Visible keyboard focus states using `:focus-visible`.
- Hover/focus/interactive transitions.
- `prefers-reduced-motion` support.
- Responsive viewport configuration.
- Content is prevented from overflowing horizontally on small screens.

## File and Folder Structure

```text
WEDE_Part_2_Submission/
├── index.html
├── about.html
├── services.html
├── enquiry.html
├── gallery.html
├── contact.html
├── css/
│   └── style.css
└── README.md
```

The Part 1 PDF is not included in the website deployment folder because it is assessment evidence rather than a website asset.

## How to Run the Website Locally

No server-side software is required for the basic HTML/CSS website.

### Method 1 — Open directly

1. Extract the ZIP file.
2. Open the `WEDE_Part_2_Submission` folder.
3. Double-click `index.html`.
4. Use the navigation menu to test the other pages.

### Method 2 — Visual Studio Code

1. Open Visual Studio Code.
2. Select **File → Open Folder**.
3. Open the `WEDE_Part_2_Submission` folder.
4. Open `index.html`.
5. If the **Live Server** extension is installed, right-click `index.html` and choose **Open with Live Server**.
6. Test every navigation link.

## Testing Checklist

Before submitting, test the following:

- [ ] `index.html` opens correctly.
- [ ] Home navigation works from every page.
- [ ] About page opens.
- [ ] Services page opens.
- [ ] Enquiry page opens.
- [ ] Gallery page opens.
- [ ] Contact page opens.
- [ ] External CSS loads on every page.
- [ ] No horizontal scrolling occurs on mobile.
- [ ] Navigation remains usable at tablet and mobile widths.
- [ ] Forms display correctly.
- [ ] Buttons and links have visible hover/focus states.
- [ ] Gallery and embedded content fit their containers.
- [ ] Website is checked in browser Developer Tools at desktop, tablet, and mobile widths.

## Responsive Screenshot Evidence

Part 2 requires screenshot evidence of different screen sizes. Add screenshots to the repository after testing in browser Developer Tools.

Recommended evidence:

```text
screenshots/
├── desktop-home.png
├── tablet-home.png
└── mobile-home.png
```

### How to capture the screenshots

In Chrome or another Chromium-based browser:

1. Open the website.
2. Open Developer Tools with `F12` or `Ctrl + Shift + I`.
3. Select the device/viewport toolbar.
4. Test a desktop-sized viewport.
5. Capture the homepage and save it as `desktop-home.png`.
6. Test a tablet-sized viewport and save `tablet-home.png`.
7. Test a mobile-sized viewport and save `mobile-home.png`.
8. Repeat testing on other pages if required by the lecturer.
9. Add the `screenshots/` folder to the repository.
10. Update this README with the final screenshot filenames.

## Git and GitHub Submission

### 1. Install Git

If Git is not installed, install Git and restart Visual Studio Code.

### 2. Open the project folder

Open the `WEDE_Part_2_Submission` folder in Visual Studio Code.

### 3. Initialise Git

Open the VS Code terminal:

```bash
git init
```

### 4. Add the files

```bash
git add .
```

### 5. Create the first Part 2 commit

```bash
git commit -m "Complete Part 2 CSS and responsive design"
```

### 6. Use the existing Part 1 GitHub repository

Part 2 should remain in the **same GitHub repository as Part 1** so your lecturer can see the project progress. Do not create a second repository for Part 2.

If the project folder is already connected to your Part 1 repository, check it with:

```bash
git remote -v
```

If no remote is shown, add the URL of your existing Part 1 repository:

```bash
git remote add origin YOUR_EXISTING_PART_1_REPOSITORY_URL
```

### 7. Commit and push the Part 2 changes

If the GitHub repository uses `main` as its default branch:

```bash
git branch -M main
git push -u origin main
```

### 9. Future CSS/file changes

Whenever you change the CSS or HTML:

```bash
git status
git add .
git commit -m "Update responsive CSS and website layout"
git push
```

Use descriptive commit messages so your development history is clear.

## GitHub Pages / Live Deployment

If your lecturer requires a live deployment, GitHub Pages can be used for a static HTML/CSS website.

After pushing the project:

1. Open the GitHub repository.
2. Open **Settings**.
3. Find **Pages**.
4. Select the branch containing the website, normally `main`.
5. Select the repository root as the publishing folder if prompted.
6. Save the Pages configuration.
7. Wait for the deployment to complete.
8. Open the generated live URL.
9. Test every page and navigation link on the live website.

Record the final live URL here:

```text
GitHub Repository:
PASTE YOUR GITHUB REPOSITORY URL HERE

Live Website:
PASTE YOUR GITHUB PAGES OR NETLIFY URL HERE
```

## Changelog

### Part 2 — CSS Styling and Responsive Design

| Date | Change |
|---|---|
| 2026-09-17 | Reviewed the Part 1 feedback and identified the required corrections to file/folder management and the broken homepage navigation. |
| 2026-09-17 | Renamed the homepage from `index (1).html` to `index.html` so the standard homepage filename matches the navigation links and deployment conventions. |
| 2026-09-17 | Corrected the website folder structure by placing the six HTML pages in the project root and creating a dedicated `css/` directory. |
| 2026-09-17 | Created `css/style.css` as the shared external stylesheet and linked all six HTML pages to it. |
| 2026-09-17 | Migrated the existing page styling from inline CSS into the external stylesheet. |
| 2026-09-17 | Added shared CSS reset/base rules, typography, colour variables, spacing, layout rules, interactive states, and form styling. |
| 2026-09-17 | Added responsive breakpoints for desktop, tablet, mobile, and small-phone screen sizes using media queries. |
| 2026-09-17 | Added responsive Grid/Flexbox layout changes so multi-column sections can adapt to smaller screens. |
| 2026-09-17 | Added responsive typography and sizing using relative units and `clamp()` where appropriate. |
| 2026-09-17 | Added keyboard focus styling and reduced-motion support to improve accessibility and usability. |
| 2026-09-17 | Updated the README to document Part 2 requirements, changes made, file structure, testing, screenshot evidence, and Git/GitHub submission steps. |

## References

The following references were used/retained from the Part 1 project:

- Mastercard Foundation. Available at: https://mastercardfdn.org
- Anver, M., 2020. *Mastercard Foundation Overview*.
- Langevin, M., Brunet-Belanger, A. and Lefevre, S.A., 2023. *Financialization through payment infrastructure: the philanthrocapitalism of the Mastercard foundation*. In *Financializations of Development*, pp. 141–154. Routledge.
- Miles, A., 2015. *Reaching the excluded responsibly: The MasterCard Foundation's strategy for financial inclusion*. *Innovations*, 10(1–2).
- HubSpot, 2020. *Web Design 101: How HTML, CSS, and JavaScript Work*.
- WordStream, 2022. *The 25 Best Ways to Increase Your Online Presence*.
- Visual Studio Code. *Getting Started with Visual Studio Code*.
- Swearingen, R., 2020. *Validating Code with the W3C Validator* [YouTube video].
- Mastercard Foundation. *Mastercard Foundation* [YouTube video].

## Part 2 Submission Checklist

- [ ] Six HTML pages included.
- [ ] `css/style.css` included.
- [ ] All HTML pages link to the external stylesheet.
- [ ] Homepage is named `index.html`.
- [ ] Navigation to the homepage has been corrected.
- [ ] Folder structure is clean and organised.
- [ ] Desktop layout tested.
- [ ] Tablet layout tested.
- [ ] Mobile layout tested.
- [ ] Screenshots added to the repository.
- [ ] README updated with the changelog.
- [ ] Git commits created with descriptive messages.
- [ ] GitHub repository pushed successfully.
- [ ] GitHub repository URL copied for LMS submission.
- [ ] Live deployment URL copied for LMS submission, if required.
