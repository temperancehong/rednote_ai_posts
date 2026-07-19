---
name: xiaohongshu-ai-carousel
description: Create Chinese Xiaohongshu/RedNote short carousel drafts from AI or technology articles, papers, notes, links, or source text. Use when Codex needs to turn source material into a one-point-per-image carousel, short image copy, Chinese caption, title options, hashtags, and a Markdown artifact with source metadata. Do not use for RedNote long articles; use xiaohongshu-ai-longform for longform posts.
---

# Xiaohongshu AI Carousel

## Overview

Turn AI and technology source material into a Chinese Xiaohongshu/RedNote carousel draft. Preserve the source's main idea and caveats, but rewrite it as short, copy-ready image text with accurate attribution.

## Workflow

1. Gather source context.
   - If the user provides a URL and the article content is not already in context, read or browse the source first.
   - Capture the original title, author, URL, original publish date, source language, and draft date.
   - If a source field is unavailable, write `Unknown`; do not invent it.

2. Extract the post angle.
   - Identify the central thesis, the key distinction, and the most useful takeaway for a Xiaohongshu reader.
   - For AI workflow articles, look especially for: what changed, old way vs new way, operating cycle, building blocks, feedback/state, verification, risks, and human judgment.
   - Use the user's notes as priority signals, but correct misunderstandings gently when the source says otherwise.

3. Draft a carousel.
   - Default to 7-10 images unless the user asks for a different count.
   - Use one point per image.
   - Make 图 1 a strong cover, 图 2 a concise definition or contrast, middle images the structure/use case, and the last image the caution or takeaway.
   - Treat the carousel as short cards, not explainer pages. Enforce two visible-copy limits by default: no single image over 80 characters, and all image copy together under 500 characters. Exclude metadata, section headings, caption, title options, and hashtags from this count.
   - For a 7-10 image carousel, aim for roughly 40-70 visible characters per image so the total budget has room to breathe.
   - If a point needs more room, split it into another image or move the explanation into the caption.
   - Use short lines, no dense paragraphs, and no citations inside image copy unless requested.
   - If the user asks for a long article, reading-note essay, or no card/image character limits, stop using this skill and use `$xiaohongshu-ai-longform` instead.

4. Write in Xiaohongshu style.
   - Use Chinese as the main language.
   - Keep important English terms such as `Loop Engineering`, `Prompt Engineering`, `Agent`, or `Sub-agents` when they are the concept being explained.
   - Be clear, useful, and human; avoid hype, vague inspiration, exaggerated claims, and generic AI-sounding phrasing.
   - Use concrete contrasts when helpful, but vary the sentence shape. Avoid stock explainer hooks, slogan-like pivots, and repeated template frames.
   - Make the copy sound like a sharp personal note from someone who read the article, not like a templated explainer.

5. Save the Markdown artifact.
   - Default folder: `artifacts/` under the current workspace.
   - Default filename: `YYYY-MM-DD-<topic-slug>-rednote.md`.
   - Include metadata, image-by-image copy, title options, caption, and hashtags.
   - Before writing, read [carousel-template.md](references/carousel-template.md) and follow its structure.

6. Respond with the saved file path.
   - Link the created Markdown file.
   - Mention any source fields that were unavailable or uncertain.

## Quality Checklist

- The post explains the idea without assuming the reader has read the original.
- Each image has one clear job.
- Each image stays under 80 visible characters unless the user explicitly asks for text-heavy cards.
- The total visible image copy stays under 500 characters unless the user explicitly asks for text-heavy cards.
- Dense explanations belong in the caption, not on the images.
- The carousel includes the source's caution or limitation, not only the exciting part.
- The artifact metadata includes draft date and original source details.
- The caption sounds natural for Xiaohongshu and includes relevant hashtags.
