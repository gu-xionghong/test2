# Research Webpage Template

A professional, responsive Jekyll template for academic researchers to showcase their work, publications, and professional information.

## Features

- **Modern Design**: Clean, professional interface with responsive layout
- **Research Showcase**: Display your papers with filtering by year and topic
- **Automatic Processing**: Markdown files in `_research` folder are automatically converted to beautiful research pages
- **GitHub Pages Ready**: Deploy directly to GitHub Pages with automated workflows
- **Responsive**: Works seamlessly on mobile, tablet, and desktop devices
- **Customizable**: Easy to modify colors, content, and layout

## Quick Start

### 1. Create a new repository

Use this template to create a new repository in your GitHub account.

### 2. Update the configuration

Edit `_config.yml` to customize your site:

```yaml
title: "Your Name - Research"
description: "Personal research website of Your Name"
url: "https://yourusername.github.io"
baseurl: ""

# Personal information
author:
  name: "Your Full Name"
  email: "your.email@example.com"
  bio: "Brief bio about your research and expertise"
```

### 3. Add your research papers

Create Markdown files in the `_research` directory following this structure:

```markdown
---
layout: research
title: "Paper Title"
date: 2023-12-01
authors: "Author 1, Author 2, Author 3"
venue: "Conference/Journal Name"
pdf: "https://link.to/pdf"
code: "https://github.com/yourusername/repo"
slides: "https://link.to/slides"
image: "/assets/images/research/paper-image.jpg"
tags:
  - Machine Learning
  - Computer Vision
color: "3498db"
excerpt: "Brief abstract or description of the paper"
---

## Abstract

Your paper abstract goes here...
```

### 4. Customize your pages

- Update `about/index.html` with your academic background, education, and experience
- Update `contact/index.html` with your contact information and social profiles
- Replace `assets/images/profile.jpg` with your profile picture

### 5. Deploy to GitHub Pages

The template includes a GitHub workflow that automatically builds and deploys your site to the `gh-pages` branch when you push to `main`.

To enable GitHub Pages:
1. Go to your repository settings
2. Under "Pages", select `gh-pages` as the source branch
3. Your site will be available at `https://yourusername.github.io/repository-name/`

## Local Development

To preview your site locally:

1. Install Jekyll and dependencies:
   ```bash
   bundle install
   ```

2. Start the development server:
   ```bash
   bundle exec jekyll serve
   ```

3. Open your browser and navigate to `http://localhost:4000`

## Customization

### Colors

Modify the color variables in `assets/css/main.css`:

```css
:root {
  --primary-color: #2c3e50;    /* Main text color */
  --secondary-color: #3498db;  /* Accent color */
  --background-color: #f9f9f9; /* Background color */
  --card-bg-color: #ffffff;    /* Card background */
  --text-muted: #7f8c8d;       /* Muted text color */
}
```

### Fonts

The template uses Inter font by default. You can change it in `_layouts/default.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

### Navigation

Update the navigation links in `_includes/header.html`:

```html
<nav class="nav-menu">
  <a href="{{ "/" | relative_url }}" class="nav-link">Home</a>
  <a href="{{ "/research/" | relative_url }}" class="nav-link">Research</a>
  <a href="{{ "/about/" | relative_url }}" class="nav-link">About</a>
  <a href="{{ "/contact/" | relative_url }}" class="nav-link">Contact</a>
</nav>
```

## License

This template is available under the MIT License. Feel free to use and modify it for your personal research website.