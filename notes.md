
---

## FILE: notes.md

```md
# Project Notes

## Purpose of the current version

This version of the project is meant to establish a professional and trustworthy front-end shell before the actual DPIA tool is implemented.

It should:
- look credible and serious
- be easy to open locally
- be easy to host with GitHub Pages
- be easy for non-technical contributors to understand
- remain clean enough to extend later

## Design direction

The design is intentionally restrained.

Keywords:
- legal
- professional
- quiet
- structured
- institutional
- modern, but not flashy

The site should feel closer to a law firm or legal-tech consultancy than to a student portfolio or startup demo page.

## Current technical decisions

### 1. Single HTML entry point
Everything important is available through `index.html`. This keeps the project easy to run and lowers the chance of setup issues.

### 2. CSS embedded in `index.html`
The CSS is currently included directly in the HTML file to make the first version portable and easy to understand. Later, the styling can be moved into a separate `styles.css` file if the project grows.

### 3. Minimal JavaScript only
`app.js` only handles small quality-of-life improvements:
- mobile navigation toggle
- active section highlighting
- subtle reveal effect on scroll

The page should still remain understandable without deep JavaScript knowledge.

## Repository governance

This repository should be operated with one clear owner and a simple review structure.

Recommended model:
- the owner creates and controls the repository
- three other team members are added as collaborators
- collaborators work in their own branches
- collaborators open pull requests
- the owner reviews and merges to `main`

This is the cleanest solution for a small student team because it keeps responsibility clear and reduces the chance of chaos in the main branch.

## Owner email privacy

The repository owner wants their personal email hidden on GitHub.

That means two separate things must be handled:

### 1. GitHub account settings
The owner should enable:
- **Keep my email addresses private**
- **Block command line pushes that expose my email**

### 2. Local Git configuration
The owner should set Git locally to use the GitHub `noreply` address, not their real email.

Example:

```bash
git config --global user.name "hakgr96"
git config --global user.email "270322742+hakgr96@users.noreply.github.com"