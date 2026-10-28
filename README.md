# DevOps Portfolio Website

A responsive, static portfolio website for **Rushikesh Tayare**, built with HTML, CSS, and vanilla JavaScript. It is designed for GitHub Pages and requires no build tools, package manager, or server-side code.

## Preview

The intended GitHub Pages address is:

**https://RushikeshTayare.github.io**

That address works when this repository is named `RushikeshTayare.github.io` (GitHub Pages user site). If you choose a different repository name, GitHub Pages uses `https://RushikeshTayare.github.io/DevOps-Portfolio-Website/` instead.

## Features

- Responsive layout for desktop, tablet, and mobile
- About, toolkit, projects, learning journey, and contact sections
- Accessible mobile navigation and reduced-motion support
- No framework, build step, or dependencies
- MIT licensed

## Repository structure

```text
devops-portfolio-website/
├── index.html       # Page content and metadata
├── styles.css       # Responsive styling
├── script.js        # Mobile navigation and current year
├── README.md        # Setup, publishing, and maintenance guide
├── LICENSE          # MIT License
└── .gitignore       # Common local/editor files to ignore
```

## Run locally

The site is static. Open `index.html` in a browser, or serve the folder with any simple local web server. No installation is required.

## Publish to GitHub Pages

### 1. Create the repository

On GitHub, create a **public** repository named exactly `RushikeshTayare.github.io` for the short user-site URL above. Leave “Add a README” unchecked because this project already includes one. Alternatively, choose a project name such as `devops-portfolio-website`; its Pages URL will include that repository name.

### 2. Put the project files in a local folder

Unzip this download. In PowerShell, change into the extracted `devops-portfolio-website` folder. In Git Bash or macOS/Linux Terminal, use the equivalent `cd` command.

### 3. Initialize Git and publish

Replace `REPOSITORY-NAME` with `RushikeshTayare.github.io` or your chosen repository name. These commands publish the current folder to the `main` branch:

```bash
git init
git branch -M main
git add .
git commit -m "Create DevOps portfolio website"
git remote add origin https://github.com/RushikeshTayare/DevOps-Portfolio-Website.git
git push origin main
```

GitHub may ask you to authenticate in a browser or through your configured Git credential manager. Never put a password, access token, or other secret in the repository or in a Git remote URL.

If you already initialized a repository, skip `git init`, `git branch -M main`, and `git remote add origin ...`. If `origin` is already set, inspect it with `git remote -v` and update it with `git remote set-url origin https://github.com/RushikeshTayare/REPOSITORY-NAME.git` if needed.

### 4. Enable Pages

In the repository on GitHub, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save. GitHub Pages publishes the files from that branch and folder. The site address appears in the Pages settings when deployment is ready. [GitHub Pages publishing instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Maintain the repository

After editing the site, review and publish the changes:

```bash
git status
git diff
git add index.html styles.css script.js README.md
git commit -m "Update portfolio content"
git push
```

Use `git add .` instead when you intentionally want to include all new and changed files. Check the **Actions** tab on GitHub if a Pages deployment does not complete.

## Personalize before sharing

- Update the text, skills, journey, and project details in `index.html` so they reflect your actual experience.
- The GitHub links currently point to `RushikeshTayare`. Replace them if the account name changes.
- The portfolio deliberately uses GitHub as its contact link; no email address or other personal contact details were invented.
- The preview image in the Projects section is drawn with CSS, so no image files are required.
- Google Fonts are loaded from Google Fonts when a visitor has internet access. The site remains usable if those fonts cannot load.
- Avoid publishing passwords, access tokens, private keys, or other secrets. GitHub Pages websites are publicly accessible.

## License

This project is available under the MIT License. See [LICENSE](LICENSE).
