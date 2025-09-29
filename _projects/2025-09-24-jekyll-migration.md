---
title: "Migrating My Portfolio Site to Jekyll: Streamlined Content Management"
layout: single
date: 2025-09-24
category: blog
---

After launching my personal portfolio site with basic HTML and GitHub Pages, I quickly realized that managing new articles and projects was becoming tedious. Each update required manual HTML edits, link management, and directory juggling. To solve this, I migrated my site to [Jekyll](https://jekyllrb.com/), a static site generator that integrates seamlessly with GitHub Pages and dramatically improves content management.

### Why Jekyll?

Jekyll is designed for building static websites with minimal effort. It lets you write content in Markdown, automatically generates pages and navigation, and supports powerful templating with Liquid. For a portfolio site with blog articles and project showcases, Jekyll’s structure is a perfect fit.

### Key Benefits I Gained

- **Easy Content Creation:**  
  I now write blog posts and project entries as simple Markdown files. Jekyll automatically converts them to HTML and adds them to the site.
- **Automatic Navigation & Organization:**  
  No more manual link updates—Jekyll dynamically lists posts and projects using Liquid loops.
- **Consistent Theming:**  
  After starting with the built-in minima theme, I switched to the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme for a more modern, feature-rich look. Minimal Mistakes provides beautiful layouts, flexible navigation, and built-in support for author profiles, cards, and collections.
- **Separation of Content and Layout:**  
  Layouts and includes keep navigation, headers, and footers consistent across all pages, while content stays clean and focused.

### How I Made the Switch

1. **Set Up Jekyll Structure:**  
   I added a `_config.yml` file and organized my content into `_posts` for blog articles and `_projects` for project showcases.
2. **Converted Pages to Markdown:**  
   All main pages (home, resume, contact) and posts are now Markdown files with YAML front matter, making editing and updates much easier.
3. **Leveraged Liquid Templating:**  
   I created index pages for both blog and projects that use Liquid loops to automatically list all entries.
4. **Enabled Theming:**  
  I started with minima, but quickly upgraded to Minimal Mistakes. This theme gave my site a professional look, easy navigation, and powerful features like card-based layouts and author profiles—all with minimal configuration.

### Lessons Learned

- **Version Control is Effortless:**  
  Every change is tracked in Git, and deploying updates is as simple as pushing to GitHub.
- **Scalability:**  
  Adding new articles or projects is now just a matter of dropping a Markdown file in the right folder.
- **Customization:**  
  Jekyll’s layouts and includes make it easy to tweak the look and feel without touching every page.

### What’s Next?

With Jekyll in place, I’m excited to focus on writing more blog articles—especially technical tutorials and book reviews—and showcasing new projects. I plan to explore custom themes and advanced Liquid features to further personalize my site.

**If you’re building a portfolio or blog on GitHub Pages, I highly recommend giving Jekyll a try. It’s a game-changer for managing and growing your site!**