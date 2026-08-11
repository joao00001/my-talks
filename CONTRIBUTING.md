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

3. Add the metadata required for the root `README.md` talks table. After a `presentation` PR is merged, the repository workflow updates that table automatically.

## Required fields in each talk README

- Talk title
- Event
- Date
- Location
- Track
- Duration
- Theme
- Language
- Status
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
- [ ] `README.md` includes the metadata used to update the root talks table (`Theme`, `Language`, and `Status`)
- [ ] Links were checked (event page, references, recording if available)

## Pull request labels

- Use the `presentation` label when the PR adds or updates presentation files such as `.pdf`, `.pptx`, `.odp`, or slide assets like `.png`.
- Use the `code-write` label for repository maintenance changes that should bypass the presentation-file validation.
- If a PR has multiple labels, `code-write` takes precedence and bypasses the presentation validation.
- `presentation` PRs also validate the talk metadata used by the root `README.md` table and, after merge, automatically sync that table on `main`.

## Reusable README template

```markdown
# Talk Title

**Event:** Event Name  
**Date:** YYYY-MM  
**Location:** City, Country  
**Track:** Track name  
**Duration:** 30-60 min  
**Speaker:** Name / Team  
**Theme:** Main topic for the root talks table  
**Language:** PT-BR / EN / ES  
**Status:** Draft / Final

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
