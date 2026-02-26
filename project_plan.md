# Project Plan: IL Animal Welfare Bill Tracker

## Goal
Build a tool that automatically monitors animal welfare legislation in Illinois
and surfaces relevant information for our organization without manual checking.

---

## Phase 1: Research & Site Structure (CURRENT)
**Goal:** Understand how ILGA.gov is structured before writing any real scraper.

### Tasks
- [~] Check if ILGA.gov exposes an XML sitemap (`/sitemap.xml` or `/robots.txt`)
- [~] Check if there are RSS or XML data feeds
- [✓] Manually inspect 2-3 bill pages and note their HTML structure
- [✓] Document the URL pattern for bills (e.g., what makes HB4475 vs SB7891 different)
- [✓] Decide: scrape HTML directly, or use an XML feed?

### Why This Matters
Jumping straight to scraping without understanding the site structure leads to
brittle code. If ILGA has XML feeds, they're far more reliable than HTML scraping.
