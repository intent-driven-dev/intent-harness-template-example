---
name: glossary
description: Consult existing glossary Markdown to compress prose with canonical terms and bold them in responses and documents.
---

Accept optional `glossary_location`, defaulting to `docs/glossary`. Resolve relative paths from the repository root; accept an absolute path, a Markdown file, or a directory of Markdown files including subdirectories. Read the glossary before drafting relevant content. Use its canonical terms and meanings, including documented aliases to identify preferred terminology. Use canonical terms in place of the descriptions they encode. Treat their glossary meanings as implicit; do not append definitions, paraphrases, or redundant properties unless the user requests an explanation or a distinction requires clarification. Bold every occurrence of glossary terms in assistant prose and written Markdown, preserving code, URLs, and syntax-sensitive content without duplicating existing bold markers. If the location is missing or has no Markdown files, report this briefly and continue without inventing entries. Consult the glossary without creating or editing entries unless separately requested.
