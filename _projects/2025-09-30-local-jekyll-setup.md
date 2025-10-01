---
title: "How I Set Up My Local Jekyll Development Server"
layout: single
date: 2025-09-30
categories: [blog, tutorial]
tags: [jekyll, github-pages, ruby, local-dev, tutorial]
read_time: true
toc: true
excerpt: Step-by-step guide to installing Ruby, Jekyll, and running a local development server for your GitHub Pages site.
---

After migrating my portfolio to Jekyll and GitHub Pages, I needed a reliable way to preview changes before pushing them live. Here’s how I set up a local Jekyll server on Ubuntu (WSL), following best practices for Ruby version management and dependency installation.

---

## Why Run Jekyll Locally?

- **Preview changes instantly** before deploying to GitHub Pages
- **Debug build errors** in your own environment
- **Test new layouts, plugins, and content** safely

---

## Step 1: Install System Dependencies

First, update your package lists and install the required build tools and libraries:

```sh
sudo apt update
sudo apt upgrade
sudo apt install -y git curl autoconf bison build-essential libssl-dev libyaml-dev libreadline6-dev zlib1g-dev libncurses5-dev libffi-dev libgdbm6 libgdbm-dev
```

---

## Step 2: Install Ruby with rbenv

Using [rbenv](https://github.com/rbenv/rbenv) makes it easy to manage Ruby versions and avoid system conflicts.

```sh
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
source ~/.bashrc
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
rbenv install 3.2.2
rbenv global 3.2.2
ruby -v
```

---

## Step 3: Install Jekyll and Bundler

With Ruby set up, install Jekyll and Bundler:

```sh
gem install bundler jekyll
```

---

## Step 4: Install Project Dependencies

Navigate to your Jekyll site’s directory and install dependencies:

```sh
cd ~/repos/aswyen.github.io/
bundle install
```

---

## Step 5: Serve Your Site Locally

Start the Jekyll server with live reload:

```sh
bundle exec jekyll serve --livereload
```

Visit [http://localhost:4000](http://localhost:4000) in your browser to preview your site.

---

## Troubleshooting Tips

- Always use `bundle exec` to ensure the correct gem versions are used.
- If you add new gems, run `bundle install` again.
- Use `rbenv` to manage Ruby versions and avoid system Ruby conflicts.
- If you see build errors, check your Ruby version and installed gems.

---

## Summary

Setting up a local Jekyll server lets you preview and test your site before deploying. With rbenv and Bundler, you can manage dependencies cleanly and avoid common pitfalls. This workflow has made my site development much smoother and more reliable.
