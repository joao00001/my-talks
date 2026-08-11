# Contributing a Talk

## Adding a New Talk

1. Create a new directory under `talks/` following the naming convention:

   ```
   talks/<year>-<event-slug>/
   ```

   Example: `talks/2026-pgconf-brasil/`

2. Inside the directory, add:
   - `README.md` with all required fields (see checklist below).
   - `slides.pdf` as the canonical slide file name.
   - Optional `assets/` for supporting files used by the talk.

3. Update the **Talks** table in the root `README.md` with a link to your new directory.

## Required fields in each talk README

- Talk title
- Event
- Date
- Location
- Track
- Duration
- Abstract
- Slides link
- Slide summary (3 to 6+ bullets)
- Resources (event page, recording when available, related links)

## Naming conventions

- Directory: `talks/<year>-<event-slug>/`
- Slides file: `slides.pdf`
- Optional files: place under `assets/`

## Publication checklist

- [ ] Directory follows `talks/<year>-<event-slug>/`
- [ ] `README.md` includes all required metadata
- [ ] `README.md` includes "Slide summary"
- [ ] Slides are available as `slides.pdf`
- [ ] Root `README.md` talks table is updated
- [ ] Links were checked (event page, references, recording if available)

## Reusable README template

```markdown
# Talk Title

**Event:** Event Name  
**Date:** YYYY-MM  
**Location:** City, Country  
**Track:** Track name  
**Duration:** 30-60 min  
**Speaker:** Name / Team

## Abstract

Short description of the talk.

## Audience

- Audience profile

## Key takeaways

- Key takeaways

## Slide summary

1. Topic
2. Topic
3. Topic

## Slides

- [slides.pdf](slides.pdf)

## Resources

- Event page
- Link to video recording (if available)
- Any related blog posts or repositories
```
