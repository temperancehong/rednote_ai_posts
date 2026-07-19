---
name: xiaohongshu-ai-longform
description: Create Chinese Xiaohongshu/RedNote long-form article drafts from AI or technology articles, papers, notes, links, or source text. Use when Codex needs to turn source material and reading notes into a natural Chinese long article, not a carousel, with source metadata, title options, sectioned body, caveats, and hashtags while keeping important AI jargon in English.
---

# Xiaohongshu AI Longform

## Overview

Turn AI/tech source material into a Chinese RedNote long article that reads like thoughtful personal notes, not a generic explainer. Use this when the user asks for a long article, longform post, reading-note article, or explicitly wants no carousel/card character limits.

## Workflow

1. Gather source context.
   - If the user provides a URL and the article content is not already available, read or browse the source before drafting.
   - Capture original title, author, publisher, URL, original publish date, source language, draft date, and related paper links when relevant.
   - Use `Unknown` for unavailable source fields; do not invent bylines.
   - Treat the user's reading notes as the priority signal for angle, emphasis, and personal reaction.

2. Extract the article angle.
   - Identify the central thesis, the key experiment or evidence, and the caveats.
   - Add source-relevant points the user's notes missed, especially limitations, safety implications, methodology, and what the paper does not prove.
   - Correct misunderstandings gently by narrowing claims rather than sounding like a referee.

3. Draft as a long article.
   - Read [references/longform-template.md](references/longform-template.md) before saving.
   - Save to `artifacts/YYYY-MM-DD-<topic-slug>-longform-rednote.md`.
   - Include metadata, 3-5 title options, sectioned body, optional closing lines, and hashtags.
   - Do not use carousel conventions: no `图 1`, no one-point-per-image structure, and no image/card character limits.

4. Write in a natural RedNote reading-note voice.
   - Use Chinese as the main language; keep core AI terms in English when they are the concept being discussed, such as `J-space`, `J-lens`, `Chain of Thought`, `access consciousness`, `activations`, `intervention`, `alignment`, or `Agent`.
   - Sound like a careful reader explaining what they noticed, not a marketing page, lecture transcript, or AI-generated summary.
   - Prefer concrete article-specific sentences over broad openings. Start close to the source, not with generic claims about AI.
   - Use first person only when it carries real judgment: "我读到这里先停了一下", "我觉得这里要收住", "这点比标题更重要".
   - Avoid redundant heading/first-sentence pairs. If the heading says "AI safety", the next sentence should add new substance, not repeat it.
   - Avoid stock AI-ish phrasing, especially: "这个说法很抓人", "不是读心术", "打开大脑直播", "最放不下的是", "总结一下", "这给我们带来启示", and over-neat contrast chains.
   - Keep paragraphs short enough for mobile reading, but do not make every sentence a slogan.

5. Preserve nuance.
   - Distinguish observation from intervention, correlation from causation, and strong claims from weaker proven claims.
   - Include what the source does not prove, especially for consciousness, safety, or capability claims.
   - For consciousness discussions, keep `phenomenal consciousness` separate from `access consciousness`; do not imply subjective experience unless the source supports it.

6. Final pass.
   - Scan for AI-sounding transitions, generic filler, repeated sentence shapes, and over-polished thesis statements.
   - Replace generic reactions with source-grounded observations.
   - Ensure the output can be copied as a RedNote long article and the saved artifact is new unless the user explicitly asks to overwrite.
