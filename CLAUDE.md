# CLAUDE.md

Guidance for AI assistants (Claude Code and others) working in this repository.

## What this repository is

This is a **GitHub special profile repository** (`Cyber-Mario1979/Cyber-Mario1979`).
Because the repo name matches the GitHub username, the `README.md` at its root is
rendered directly on the owner's GitHub profile page at
`https://github.com/Cyber-Mario1979`.

There is **no application code, build system, test suite, or package manager** here.
The repository's sole purpose is to present and maintain the owner's public profile.
Treat it as a content/documentation repo, not a software project.

## Repository structure

```
.
├── README.md        # The profile content rendered on the GitHub profile page
├── CLAUDE.md        # This file — guidance for AI assistants
├── ASBP.png         # Banner/header image referenced at the top of README.md (~2 MB)
└── assets/
    └── banner.png   # Placeholder file (currently 1 byte, not in use)
```

That is the entire tree. Do not expect or invent source directories, configs, or CI.

## How content renders

- `README.md` is the deliverable. Its first line embeds the banner via a raw
  GitHub URL:
  `![ASBP](https://raw.githubusercontent.com/Cyber-Mario1979/Cyber-Mario1979/refs/heads/main/ASBP.png)`
- The image is referenced by an **absolute raw URL pinned to `main`**, not a
  relative path. If you rename, move, or delete `ASBP.png`, or change the default
  branch, this link breaks. Update the URL to match.
- GitHub renders GitHub-Flavored Markdown. Use standard GFM; avoid HTML/JS that
  GitHub strips.

## Content conventions

The README follows a deliberate, consistent voice and structure. Preserve it when editing:

- **Tone:** professional, declarative, systems-architecture framing. Short
  assertive statements over marketing prose.
- **Emphasis:** key concepts are **bold**. Keep this sparing and intentional.
- **Structure:** top banner image → name (`#`) → role (`##`) → themed sections
  separated by `---` horizontal rules.
- **Sections currently present (in order):** name (`# Amr Hassan`) → role
  (`## Systems Architect — AI-Augmented Workflows`) → intro paragraph → What I Work
  On → Selected Systems (*Valor* — CQV/regulated engineering; *Alex* — IGCSE
  education) → Architectural Principles → What I'm Not Doing → Current Direction.
- Closing line is an italicized statement of intent.
- Bullet lists use `-`.

When asked to update the profile, edit prose in place and keep the section rhythm
intact rather than restructuring wholesale, unless explicitly told otherwise.

## Development workflow

- **Default branch:** `main`.
- **Active working branch for AI-assisted changes:** `claude/claude-md-docs-behxdf`.
  Develop and commit here; do not push to `main` without explicit permission. AI
  changes land on `main` via pull request (see PR #1, which introduced this file).
- There is nothing to build, lint, run, or test. "Verifying" a change means
  reviewing the rendered Markdown and confirming image links resolve.
- Keep commits small and descriptively messaged (the existing history uses concise
  messages like "Update README with author details and title").

## Working on images

- `ASBP.png` is a large binary (~2 MB). Don't read it as text; reference it by path.
- `assets/banner.png` is a 1-byte placeholder. If a real banner is added there,
  wire it into `README.md` and remove or repurpose the placeholder.

## Guardrails

- Don't add tooling, frameworks, or scaffolding the repo doesn't need.
- Don't break the profile render: validate Markdown and the pinned raw image URL.
- Treat all README content as public — it is shown on the owner's GitHub profile.
