# Contributing to Mission Built

Thanks for taking the time to improve the book.

This is the open-source source-of-truth for *Mission Built*. The canonical reading site at [missionbuilt.io](https://missionbuilt.io) renders from these files, so a fix here can land in the live book.

## What to contribute

Most welcome:

- **Typos and grammar fixes.**
- **Broken or moved links** in the Sources section.
- **Factual corrections** — wrong date, wrong name, misattributed quote.
- **Clarity suggestions** where a sentence is genuinely confusing.

Less welcome (please open a Discussion first):

- **Voice or style rewrites.** The voice is intentional. If a passage reads as awkward, that's worth a Discussion before a PR.
- **Structural changes** — moving sections, changing chapter order, adding/removing material.

## How to contribute

### Report something

- **Issues** — for typos, broken links, factual errors, or anything you think is wrong: [open an issue](../../issues).
- **Discussions** — for general feedback, questions, suggestions, or "I think this whole section could be sharper": [start a discussion](../../discussions).

### Submit a fix

1. **Fork** this repository.
2. **Find the file.** The book lives in two places — both should be edited together:
   - The chapter file in [`book/`](book/). Chapter file numbers match the book's chapter numbers (e.g., Chapter 1 is `book/01-mission-before-metrics.md`, Chapter 13 is `book/13-ai-is-the-new-os.md`). Front matter uses a `00` prefix (`00a-` through `00d-`); back matter uses `99` (`99a-` through `99d-`).
   - The same passage in [`manuscript.md`](manuscript.md) at the repo root (the assembled single-file version).
3. **Make your change** in both files. Keep the diff minimal — don't reformat surrounding text.
4. **Submit a pull request** with a short description of what you changed and why. Reference any related issue.

### Editorial conventions

A few things to know before a PR:

- **The motto is "give a shit"** (not "giving a damn" or other variants). The motto attribution chain runs through Prologue → Ch 1 → Ch 8 → Ch 13 → Ch 14. Don't soften it.
- **Em-dashes** are used sparingly. Long colons or full stops are preferred.
- **Specific examples are load-bearing.** If you remove an example, the surrounding paragraph usually needs reworking. Better to fix the example's facts than to delete it.
- **Citations live in [`book/99a-sources.md`](book/99a-sources.md).** New claims should add a citation there, not inline.

## Code of conduct

Be respectful. Argue ideas, not people. The book is opinionated, but the project welcomes disagreement that's curious rather than combative.

---

Thank you for helping make this book stronger.
