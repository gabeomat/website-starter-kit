# Agent Instructions

This file gives coding agents shared project guidance. It applies to Codex, Claude Code, and other AI coding tools working in this repository.

## Project Intent

Build a simple website that is:

- Easy for humans to navigate
- Easy for search engines to crawl
- Easy for AI agents to read and cite
- Easy for a non-technical site owner to update
- Easy to deploy on Netlify

## Source Of Truth

Read these files before making meaningful changes:

- `README.md` for project overview
- `docs/brand.md` for brand, voice, visual direction, and audience
- `docs/seo-ai-readiness.md` for search and AI-readiness requirements

If `docs/brand.md` does not exist yet, ask the user for brand direction before making major design or copy decisions.

## Architecture Principles

- Use a static-site-friendly architecture.
- Keep content separate from presentation.
- Store blog posts as Markdown when possible.
- Use reusable components for repeated sections.
- Use layouts for shared page structure.
- Keep public machine-readable files in `public/`.

## Expected Public Files

The launched site should expose:

- `/robots.txt`
- `/sitemap.xml`
- `/llms.txt`

These files should be updated when site structure changes.

## AI-Friendly Content Principles

- Make the site understandable from text alone.
- Use descriptive headings.
- Use direct answers in blog content.
- Link to source-of-truth pages such as About, Work With Me, and Contact.
- Keep cornerstone information consistent across the site.
- Avoid vague marketing copy that does not explain who the site is for or what is offered.

## Safe Change Policy

For small content updates, only edit the relevant content file.

For page updates, only edit the relevant page, component, or layout.

For design system updates, check all affected components and pages.

For SEO/crawlability updates, check metadata, internal links, sitemap behavior, robots rules, and `llms.txt`.

## Verification Checklist

After changes, verify the relevant items:

- Site builds without errors.
- Navigation links work.
- Mobile layout still works.
- Page title and description are present.
- Images have useful alt text.
- New pages are linked from at least one existing page.
- Sitemap and `llms.txt` are updated when needed.
- No important page is accidentally blocked by `robots.txt`.

## Communication Style

When reporting changes to the user:

- Be concise.
- Explain what changed.
- Mention files edited.
- Mention any tests or build checks run.
- Mention any open questions or missing content.
