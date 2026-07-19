# AGENTS.md

## Project Purpose

This repository stores Xiaohongshu / Rednote post drafts adapted from AI and technology articles, essays, papers, and personal notes. The main outputs are copy-ready Chinese carousel drafts and natural Chinese long-form article drafts saved as Markdown artifacts.

## Repository Layout

- `artifacts/`: final or near-final Markdown post drafts.
- `.codex/skills/`: repo-local Codex skills that should travel with this project.
- `.codex/skills/xiaohongshu-ai-carousel/`: the local skill for turning AI/tech source material into Xiaohongshu carousel drafts.
- `.codex/skills/xiaohongshu-ai-longform/`: the local skill for turning AI/tech source material and reading notes into RedNote long articles.

## Default Workflow

When asked to create or revise a Xiaohongshu post:

1. Use `$xiaohongshu-ai-carousel` for short image carousel drafts, and `$xiaohongshu-ai-longform` for long articles or reading-note essays.
2. If the user provides a URL, read the source before drafting unless the user has already supplied enough source text.
3. Preserve source metadata in the artifact: title, author, original link, original publish date, draft date, source language, and draft language.
4. Save carousel drafts in `artifacts/` using `YYYY-MM-DD-topic-slug-rednote.md`; save long articles using `YYYY-MM-DD-topic-slug-longform-rednote.md`.
5. For carousel drafts, keep one clear point per image section.
6. For long articles, use natural section headings and do not apply carousel card character limits.
7. Include title options, caption or body copy, and hashtags.

## Writing Style

- Write primarily in Chinese, keeping English terms only when they are the concept being explained.
- Sound like a thoughtful reader making useful notes, not a generic explainer.
- Avoid hype, empty inspiration, slogan-like transitions, and repeated template frames.
- Prefer concrete, inspectable claims over broad statements.
- Keep carousel text short enough to place on mobile images.
- For long articles, write like thoughtful reading notes rather than a generic explainer.
- Include the caveats and risks from the original article, not only the exciting parts.

## Source Discipline

- Do not invent missing source fields. Use `Unknown` when needed.
- If the article is recent or the user asks for the latest/source-accurate version, verify with the source before drafting.
- Make corrections gently when user notes conflict with the source.
- Do not put dense citations into image copy unless the user asks for citation-heavy graphics.

## Repo Hygiene

- Do not create global skills for this project; keep project-specific skills under `.codex/skills/`.
- Do not commit unless the user explicitly asks.
- Do not remove or overwrite existing artifacts unless the user asks for replacement.
- Keep generated files, OS metadata, and temporary scratch files out of commits.
