# SEO And AI Readiness

This document explains how to keep the website easy for search engines and AI agents to discover, understand, and cite.

## Core Principle

The website should make important information available as clear, crawlable text.

Do not rely on images, animations, hidden tabs, or JavaScript-only content for essential information.

## Required Pages

The site should include:

- Home
- About
- Work With Me / Services
- Blog index
- Individual blog posts
- Contact
- Privacy policy
- Sitemap page, if useful for visitors
- 404 page

## Page-Level Checklist

Each important page should include:

- One clear `h1`
- A unique page title
- A unique meta description
- A clear primary topic
- Descriptive headings
- Internal links to related pages
- Descriptive image alt text
- Canonical URL
- Open Graph title, description, and image

## Blog Post Checklist

Each blog post should include:

- Clear title
- Short description
- Publish date
- Author
- Topic tags or categories
- One primary question, idea, or outcome
- Internal links to related posts or services
- A clear next step for the reader

When possible, blog posts should directly answer the question implied by the title in the first few paragraphs.

## Machine-Readable Files

The public folder should include:

```txt
public/
├── robots.txt
├── sitemap.xml
└── llms.txt
```

### robots.txt

`robots.txt` tells crawlers which public URLs they may access. It is not a security tool.

Recommended simple version:

```txt
User-agent: *
Allow: /

Sitemap: https://example.com/sitemap.xml
```

Do not block important public pages such as the home page, blog, about page, services page, or contact page.

### sitemap.xml

`sitemap.xml` helps search engines discover public URLs.

It should include important public pages and blog posts.

Update it when pages are added, removed, or renamed. If the site framework generates sitemaps automatically, confirm that all important pages are included.

### llms.txt

`llms.txt` is an emerging convention for giving AI systems a curated guide to the most important content on the site.

Recommended simple version:

```md
# Site Name

> One-sentence description of who this site helps and what it provides.

## Core Pages

- [Home](https://example.com/): Short description.
- [About](https://example.com/about/): Short description.
- [Work With Me](https://example.com/work-with-me/): Short description.
- [Blog](https://example.com/blog/): Short description.
- [Contact](https://example.com/contact/): Short description.

## Key Topics

- [Topic or guide title](https://example.com/blog/example-post/): Short description.
```

Keep `llms.txt` short, accurate, and focused on the most useful pages.

## Structured Data

Use structured data where it accurately describes visible page content.

Useful schema types for a basic expert, creator, coach, or service-provider website:

- `Person`
- `Organization`
- `WebSite`
- `WebPage`
- `Article`
- `BlogPosting`
- `BreadcrumbList`
- `FAQPage`, only when the page visibly contains FAQs
- `Service`, when describing a real service

Do not add structured data for information that is not visible on the page.

## Internal Linking

Important pages should not be isolated.

Minimum internal links:

- Home links to About, Work With Me, Blog, and Contact.
- About links to Work With Me and Contact.
- Blog index links to every published post.
- Blog posts link back to the blog index.
- Relevant blog posts link to Work With Me when appropriate.
- Footer links to core pages, privacy policy, and sitemap.

## URL Rules

Use short, readable URLs:

```txt
/about/
/work-with-me/
/blog/
/blog/how-to-plan-a-simple-website/
/contact/
```

Avoid:

```txt
/page?id=123
/new-final-v3/
/services-and-things/
```

## Image Rules

- Use descriptive filenames when possible.
- Add alt text for meaningful images.
- Use empty alt text for purely decorative images.
- Compress large images before publishing.
- Avoid placing important text inside images.

## AI Citation Readiness

To make the site easier for AI tools to cite:

- Publish clear source-of-truth pages.
- Keep claims specific and consistent.
- Add author names and dates to blog posts.
- Include original ideas, examples, frameworks, or definitions.
- Make contact and business information easy to verify.
- Keep important pages accessible without login walls.

## Launch Checklist

Before launch:

- Confirm the site builds.
- Confirm all core pages load.
- Confirm mobile layout works.
- Confirm metadata exists on every important page.
- Confirm `/robots.txt` loads.
- Confirm `/sitemap.xml` loads.
- Confirm `/llms.txt` loads.
- Confirm contact forms or booking links work.
- Submit the sitemap in Google Search Console.
- Test social sharing previews if possible.

## Maintenance Checklist

Monthly:

- Add or refresh useful blog content.
- Check broken links.
- Check Search Console for indexing issues.
- Review top pages and improve weak titles or descriptions.
- Update `llms.txt` when cornerstone pages change.
- Confirm offers, contact details, and testimonials are current.
