# Peter Nguyen - Personal Website & Resume

This is my personal website and online resume, built with Jekyll and hosted on GitHub Pages.

## Features

- Single-page resume with smooth scrolling navigation
- Dark mode toggle with preference persistence
- Blog section with full post support
- Responsive design for mobile and desktop
- Professional sections: About, Experience, Skills, Projects, Contact
- Downloadable PDF resume option
- Social media integration

## Customization Guide

### 1. Update Site Configuration

Edit `_config.yml` to update your personal information:

```yaml
title: Your Name
description: Your tagline
email: your.email@example.com
github_username: your-github-username
linkedin_username: your-linkedin-username
```

### 2. Customize Your Resume Content

Edit `index.md` to update:

- **About Me**: Add your bio and background
- **Professional Experience**: Add your work history
- **Skills**: List your technical skills
- **Projects**: Showcase your portfolio projects
- **Contact**: Update your contact information and social links

### 3. Add Your PDF Resume

1. Create/export your resume as PDF
2. Save it as `assets/resume.pdf`
3. The download link is already configured

### 4. Write Blog Posts

Create new blog posts in the `_posts` directory following this naming convention:

```
YYYY-MM-DD-post-title.md
```

Each post should have front matter:

```yaml
---
layout: default
title: "Your Post Title"
date: YYYY-MM-DD
author: Your Name
tags: [tag1, tag2]
excerpt: "Brief description of your post"
---
```

### 5. Customize Styling

The site uses inline styles in `index.md` and `blog.md`. You can:

- Modify colors in the CSS sections
- Adjust the dark mode theme colors
- Change fonts and layouts

## Local Development

To test your site locally:

1. Install Jekyll:
   ```bash
   gem install bundler jekyll
   ```

2. Create a `Gemfile`:
   ```ruby
   source 'https://rubygems.org'
   gem 'github-pages', group: :jekyll_plugins
   ```

3. Install dependencies:
   ```bash
   bundle install
   ```

4. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```

5. Visit `http://localhost:4000` in your browser

## GitHub Pages Deployment

This site is automatically deployed via GitHub Pages. Any commits to the main branch will trigger a rebuild.

To publish your site:

1. Ensure your repository is named `yourusername.github.io`
2. Go to repository Settings > Pages
3. Set source to the main branch
4. Your site will be available at `https://yourusername.github.io`

## Project Structure

```
.
├── _config.yml           # Site configuration
├── index.md              # Main resume page
├── blog.md               # Blog index page
├── _posts/               # Blog posts directory
│   └── YYYY-MM-DD-title.md
├── assets/               # Static assets
│   ├── resume.pdf        # Your PDF resume
│   └── images/           # Images for blog posts
└── README.md             # This file
```

## Dark Mode

The site includes a dark mode toggle that:
- Saves user preference to localStorage
- Automatically applies saved preference on page load
- Works across all pages

## Technologies Used

- Jekyll - Static site generator
- GitHub Pages - Hosting
- Markdown - Content format
- CSS3 - Styling with custom properties
- Vanilla JavaScript - Dark mode functionality

## Support

For issues or questions about the site, please open an issue in this repository.

## License

This project is open source and available for personal use.

---

Built with ❤️ using Jekyll and GitHub Pages
