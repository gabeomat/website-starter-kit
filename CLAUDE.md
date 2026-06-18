# Claude Code Instructions

You are helping build and maintain a simple, search-friendly, AI-readable website.

Before making design, copy, structure, or SEO changes, read:

- `README.md`
- `docs/brand.md`, if present
- `docs/seo-ai-readiness.md`

## Primary Goal

Keep the website simple, maintainable, crawlable, and easy for a non-technical person to update with AI assistance.

Prefer small, targeted edits over broad rewrites.

## Editing Rules

- Preserve the existing project structure unless there is a clear reason to change it.
- Reuse existing components, layouts, styles, and content patterns.
- Do not rewrite unrelated files.
- Do not replace the entire site when the request is for a small update.
- Keep content in Markdown or simple structured data where possible.
- Keep reusable UI in components.
- Keep page-level composition in pages or layouts.
- Avoid adding heavy dependencies unless the user explicitly approves them.
- Make mobile-friendly changes by default.

## Content Rules

- Use clear, direct language.
- Make the page purpose obvious near the top of each page.
- Include helpful internal links between related pages.
- Do not invent testimonials, client names, credentials, prices, guarantees, or results.
- If information is missing, use a clear placeholder and tell the user what is needed.
- Keep important text as real HTML text, not embedded in images.

## Search And AI Rules

- Every important page needs a unique title and meta description.
- Every important page should have one clear `h1`.
- Use semantic heading order.
- Add descriptive alt text to meaningful images.
- Keep URLs short, readable, and stable.
- Keep blog posts crawlable and internally linked.
- Update `sitemap.xml` or the sitemap generation config when pages are added.
- Update `llms.txt` when important pages or cornerstone content changes.
- Do not block important public pages in `robots.txt`.

## Design Rules

- Follow `docs/brand.md` when it exists.
- Keep the visual system consistent across pages.
- Use reusable spacing, typography, and color patterns.
- Prioritize clarity over visual complexity.
- Make calls to action easy to find.
- Avoid decorative sections that do not help the visitor understand the site.

## Netlify Rules

- Keep the site compatible with Netlify static hosting unless the user asks for server-side features.
- Do not require server-only functionality for basic pages or blog posts.
- Use environment variables only when necessary.
- If redirects are needed, use Netlify-compatible redirects.

## Good Update Pattern

When making a requested update:

1. Identify the smallest set of files that need to change.
2. Make the change using existing patterns.
3. Check that the site still builds.
4. Summarize what changed and mention any follow-up needed.

## Do Not Do These

- Do not redesign the whole site for a content edit.
- Do not delete existing content without permission.
- Do not add fake business claims.
- Do not hide important content from search engines.
- Do not make navigation dependent on JavaScript when plain links would work.
- Do not make private content public.
