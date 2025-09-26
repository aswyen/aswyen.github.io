---
title: "Building My Personal Portfolio Website"
layout: default
date: 2025-09-01
category: projects
---

## Building My Personal Portfolio Website with GitHub Pages

*September 2025*

Over the past few weeks, I wanted to create a central online location to showcase my work, share tutorials, and document projects. I decided on a personal portfolio website using **GitHub Pages** because it’s free, flexible, and integrates seamlessly with version control.

### Step 1: Set Up the Repository
I created a new repository on GitHub under my username (`aswyen`) named `alecwyen.github.io`. GitHub Pages automatically hosts this repository at `https://alecwyen.github.io` when using the main branch.

### Step 2: Connect My Custom Domain
I already owned `alecwyen.com`. To point it to GitHub Pages, I added a `CNAME` file with my domain and updated the DNS records (A records for `@` and `CNAME` for `www`). GitHub confirmed the domain after DNS propagation.

### Step 3: Enable HTTPS
Initially, HTTPS wasn’t available because the certificate had not yet issued. After DNS confirmed, GitHub issued the SSL certificate, allowing me to enforce HTTPS and secure the site.

### Step 4: Organize Directory Structure
I decided to separate content for maintainability:
- `blog/` for articles
- `projects/` for project pages
- `styles/` for CSS
- `scripts/` for JavaScript
- `images/` for screenshots and thumbnails

### Step 5: Build Pages and Layouts
Using simple HTML templates, I created:
- An **index page** for the landing experience
- A **resume page** with my full professional experience
- **Projects and blog overview pages** using responsive card layouts
- Individual pages for projects and articles

### Step 6: Decoupled CSS and JS
All styling resides in `/styles/style.css` and scripts in `/scripts/script.js`. This keeps HTML clean and allows future updates without touching the HTML content.

### Step 7: Using AI Tools to Accelerate Development
I leveraged ChatGPT to help generate templates, debug deployment issues, and ensure consistency across pages. It was like having a virtual assistant for front-end development.

### Next Steps
From here, I plan to populate more blog articles, document tutorials for firmware and BIOS development, and add project showcases. With the directory structure in place, adding new content will be straightforward.
