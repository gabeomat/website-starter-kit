# Website Build Prompt

Use this prompt after placing `README.md`, `CLAUDE.md`, `AGENTS.md`, `docs/brand.md`, and `docs/seo-ai-readiness.md` into a new project folder.

```txt
I want you to help me build a simple, maintainable, search-friendly, AI-readable website.

Before writing code, read:

- README.md
- CLAUDE.md
- AGENTS.md
- docs/brand.md
- docs/seo-ai-readiness.md

Then build the site using the guidance in those files.

Site goals:

- Clear home page
- About page
- Work With Me / Services page
- Blog index
- Individual blog post template
- Contact page
- Sitemap page or sitemap support
- Privacy policy
- 404 page
- Public robots.txt
- Public sitemap.xml
- Public llms.txt

Technical goals:

- Use a simple static-site-friendly structure.
- Keep content easy to update.
- Use Markdown for blog posts if possible.
- Use reusable components and layouts.
- Keep important content as crawlable text.
- Make the site responsive on mobile and desktop.
- Prepare the site for deployment on Netlify.

Design goals:

- Follow docs/brand.md.
- Keep the design clean, credible, and easy to navigate.
- Prioritize clarity over complexity.
- Make calls to action obvious.

Important rules:

- Do not over-engineer the project.
- Do not add fake testimonials, fake client logos, fake credentials, or unsupported claims.
- Do not hide important text in images.
- Do not block important public pages from crawlers.
- Prefer small, understandable files and patterns that a beginner can maintain.

Start by proposing the project structure and implementation plan. Then build the first version.
```
