# alejoespinosa.com — Portfolio Site 🚀

> DevOps engineer who ships, software architect who builds. Based in Germany. Hire me.

**Status:** 💡 Planning  
**Domain:** ✅ alejoespinosa.com  
**Email:** ✅ Configured  

---

## Architecture

```
alejoespinosa.com/
├── src/
│   ├── pages/
│   │   ├── index.astro        # Home / Hero
│   │   ├── projects.astro     # Projects list
│   │   ├── about.astro        # About me
│   │   └── blog/              # Blog posts (optional)
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── ProjectCard.astro
│   │   └── SkillBadge.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── content/
│   │   ├── projects/          # Markdown files for each project
│   │   └── blog/              # Blog posts
│   └── styles/
│       └── global.css
├── public/
│   ├── images/
│   ├── resume.pdf
│   └── favicon.ico
├── astro.config.mjs
└── package.json
```

### Infrastructure

```
┌─────────────────────────────────────────────────────────────┐
│                     GitHub Repository                       │
│                                                             │
│  - Source code                                              │
│  - Content (Markdown)                                       │
│  - GitHub Actions workflow                                  │
│                                                             │
└─────────────────────────┬───────────────────────────────────┘
                          │ Push to main
                          ▼
┌─────────────────────────────────────────────────────────────┐
│                    CI/CD Pipeline                           │
│                   (GitHub Actions)                          │
│                                                             │
│  1. Install dependencies                                    │
│  2. Build static site                                       │
│  3. Run lighthouse audit                                    │
│  4. Deploy to hosting                                       │
│                                                             │
└─────────────────────────┬───────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────┐
│                      Hosting                                │
│                                                             │
│  Options:                                                   │
│  - Cloudflare Pages (fast, easy DNS)                        │
│  - GitHub Pages (halbardhobby.com already runs there)       │
│                                                             │
└─────────────────────────┬───────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────────┐
│                   alejoespinosa.com                         │
│                                                             │
│  - Custom domain                                            │
│  - HTTPS (automatic)                                        │
│  - CDN (automatic)                                          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

## MVP Scope (v0.1)

## In Scope
- [ ] Hero section with name, title, CTA
- [ ] About section (2-3 paragraphs)
- [ ] 3 project cards with descriptions
- [ ] Skills section (grouped)
- [ ] Contact section (email, LinkedIn, GitHub)
- [ ] Mobile responsive
- [ ] Dark mode toggle
- [ ] Resume PDF download
- [ ] Deploy to Cloudflare Pages or GitHub Pages
- [x] Custom domain (alejoespinosa.com)

### Out of Scope (v1.0+)
- Blog
- Analytics (add later)
- Contact form (email link is fine for now)
- Animations beyond basics
- Multi-language (German & Spanish versions)

### Timeline

| Phase | Tasks | Time |
|-------|-------|------|
| Setup | Astro init, theme choice, repo setup | 1-2 hours |
| Content | Write about, project descriptions | 2-3 hours |
| Styling | Customize theme, responsive fixes | 2-4 hours |
| Deploy | Cloudflare Pages, domain config | 1 hour |
| Polish | Lighthouse audit, final tweaks | 1-2 hours |
