# Rednote AI Posts

This repository stores Xiaohongshu / Rednote carousel drafts adapted from AI and technology articles, essays, papers, and notes.

The goal is to keep each post source-aware, copy-ready, and easy to revise later. Drafts are written in Chinese, with original source metadata preserved in each Markdown artifact.

## Structure

- `artifacts/`: Markdown drafts for individual Xiaohongshu posts.
- `.codex/skills/xiaohongshu-ai-post/`: repo-local Codex skill for turning AI/tech source material into Rednote carousel drafts.
- `AGENTS.md`: working instructions for future Codex/agent sessions in this repo.

## Draft Format

Each post artifact should include:

- post title and draft date;
- original title, author, link, and publish date;
- image-by-image carousel copy;
- Xiaohongshu title options;
- caption and hashtags.

The default filename pattern is:

```text
YYYY-MM-DD-topic-slug-rednote.md
```

## Writing Notes

The house style is clear, concise, and human. Posts should read like useful notes from someone who actually read the source, not like generic AI-generated explainers.

Keep one idea per image, avoid slogan-like templates, and include the caveats or risks from the original source when they matter.

## Codex Skill

Use the repo-local skill when drafting or revising posts:

```text
$xiaohongshu-ai-post
```

The skill keeps source metadata, carousel structure, and Xiaohongshu writing constraints consistent across posts.
