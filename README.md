# Intern Portfolio

A responsive one-page portfolio for Hashim Anwar, a BSc Computer Science student at Lahore Leads University. It was built as a first-day internship task to practise clean HTML and CSS, Git commits, and automated linting with GitHub Actions.

## What the project includes

- A home page (`index.html`) with About, Skills, Experience and Contact sections
- Responsive styling (`style.css`) for mobile, tablet and desktop
- Valid, accessible HTML: one `h1`, landmarks, skip link, visible keyboard focus
- A CI workflow that lints the HTML and CSS on every push

## Setup steps

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/intern-portfolio.git
   cd intern-portfolio
   ```
2. Open `index.html` in your browser. No build step is needed.
3. Optional: run a local server so the page loads at a root URL:
   ```bash
   npx serve .
   ```
   then open the address it prints (usually `http://localhost:3000`).
4. Optional: run the linters locally (requires [Node.js](https://nodejs.org) 20 or newer):
   ```bash
   npm install
   npm run lint
   ```

## Continuous integration

The workflow in `.github/workflows/lint.yml` runs on every push and pull request. It installs the dev dependencies and runs:

- **HTMLHint** on `index.html`
- **Stylelint** (standard config) on `style.css`

Check the **Actions** tab on GitHub to see the result of each run.

## Live site

Enabled with GitHub Pages (Settings, Pages, deploy from the `main` branch, root folder):
`https://YOUR-USERNAME.github.io/intern-portfolio/`

## Project structure

```
intern-portfolio/
├── .github/workflows/lint.yml   CI workflow
├── index.html                   Home page
├── style.css                    Responsive styles
├── package.json                 Lint scripts and dev dependencies
├── .htmlhintrc                  HTMLHint rules
├── .stylelintrc.json            Stylelint config
└── README.md
```

## Author

Hashim Anwar
