# Simple Website Starter

This project is for a simple, search-friendly, AI-readable website that can be edited with Codex, Claude Code, or another coding agent inside VS Code.

The goal is to keep the site easy to understand, easy to update, and easy to publish on Netlify.

## Getting Started

1. Clone this repository to your computer.
2. Open the folder in VS Code.
3. Create your own brand guide by copying the template:

   ```bash
   cp docs/brand.example.md docs/brand.md
   ```

   Then fill in `docs/brand.md` with your colors, fonts, voice, and audience.
   You can ask Claude Code or Codex to help you write it. This file stays
   private to you — it is excluded from Git by `.gitignore`.
4. Start building your pages and ask your AI coding agent for small, targeted
   changes (see "Updating The Site With An AI Coding Agent" below).

## Recommended Pages

- Home
- About
- Work With Me / Services
- Blog
- Individual blog posts
- Contact
- Sitemap
- Privacy policy
- 404 page
- Thank-you page for forms, booking, or opt-ins

## Recommended Project Structure

Use this structure or something very close to it:

```txt
.
├── README.md
├── CLAUDE.md
├── AGENTS.md
├── docs/
│   ├── brand.example.md   # template — copy to brand.md and fill in
│   ├── brand.md           # your private brand guide (not committed to Git)
│   └── seo-ai-readiness.md
├── public/
│   ├── robots.txt
│   ├── sitemap.xml
│   ├── llms.txt
│   └── images/
└── src/
    ├── components/
    ├── content/
    │   └── blog/
    ├── layouts/
    └── pages/
```

## Content System

Blog posts should live as Markdown files in `src/content/blog/`.

Each blog post should include frontmatter:

```md
---
title: "Post Title"
description: "Short summary for search engines and social previews."
date: "2026-06-18"
author: "Author Name"
tags: ["topic", "example"]
image: "/images/post-image.jpg"
---
```

Pages should be built from reusable layouts and components rather than one-off custom sections whenever possible.

## Design Principles

- Keep the site simple and clear.
- Use readable typography and strong page hierarchy.
- Make the main call to action obvious.
- Use semantic HTML: one `h1` per page, descriptive headings, real links, and accessible buttons.
- Avoid hiding important content inside images, animations, tabs, or JavaScript-only interactions.
- Make all core pages usable on mobile.

## Search And AI Readiness

Before launch, the site should include:

- Unique title and meta description for each page
- Open Graph metadata for social sharing
- `robots.txt`
- `sitemap.xml`
- `llms.txt`
- Internal links between important pages
- Structured data where relevant
- Descriptive image alt text
- A crawlable blog index
- Canonical URLs

See `docs/seo-ai-readiness.md` for the full checklist.

## Updating The Site With An AI Coding Agent

When asking Codex or Claude Code to update this site, ask for small, targeted changes.

Good examples:

- "Add a new blog post using this draft."
- "Update the Work With Me page with this new offer."
- "Add a testimonial section to the home page using the existing design style."
- "Create a new FAQ section using the same typography and spacing as the rest of the site."

Avoid vague instructions like:

- "Make the site better."
- "Redesign everything."
- "Improve the SEO."

Instead, describe the specific page, section, or content you want changed.

## Deployment

Recommended deployment path:

1. Create the site locally in VS Code.
2. Commit the project to GitHub.
3. Connect the GitHub repo to Netlify.
4. Let Netlify build and deploy automatically when changes are pushed.
5. Use Netlify preview deploys to review changes before publishing.

## Before Launch

- Test all navigation links.
- Test the contact form or booking link.
- Check mobile layout.
- Confirm that `/robots.txt`, `/sitemap.xml`, and `/llms.txt` load publicly.
- Submit the sitemap in Google Search Console.
- Confirm analytics are installed, if using analytics.
- Check page titles and descriptions.
- Proofread the home, about, work with me, and contact pages.
