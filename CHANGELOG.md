# Changelog

All notable changes to *Mission Built* are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), adapted for a book rather than software.

---

## [2.1] — 2026-09 (Second Edition, Revised)

Same book, same structure, same examples. The prose is Mike's again.

### Changed

- **Voice restored throughout.** The v2 line edit had chopped the prose into fragments, single-sentence "emphasis" paragraphs, and slogan pairs, against the author's actual cadence. Every chapter and the front matter were revised against the updated `mike-nichols-voice` skill: fragment stacks rejoined into flowing sentences, lone-line paragraphs folded back in, one crystallizing line per section at most, em dashes removed from prose, corporate and AI-flavored words replaced, generic roles no longer gendered. Mean sentence length roughly 9 → 16 words; sentences of four words or fewer 24% → 9%.
- **Pull quotes** cut by more than half, at most one per section.
- **Edition label** on the title page is now *Second Edition, Revised · 2026*. Editions are about content and versions are about text; nothing was added or removed, so this is a point release, not a third edition.
- **A Note on the Second Edition** now addresses early second-edition readers, explains the revision in one paragraph, and drops the "about ten pages shorter" line.
- **Chapter 8** names both deployed Combined Air Operations Centers (Prince Sultan Air Base, Saudi Arabia; Al Udeid Air Base, Qatar) so they are not confused with the CAOC at Nellis in the prologue. "The soldiers downrange" replaces "my brothers in arms."
- **Chapter 10** customer quote reworded to how a customer talks: *"Wait, I just get the endpoint too? For what I'm already paying?"*
- **Chapter 13** boardroom close rewritten to land on the user as a person ("...ship faster to people you stopped seeing"); "stay lovable enough" was a stray and is gone.

### Not changed

- No example, story, name, number, quotation, heading, list, or citation was added or removed. Sources, license, and the Loadout are untouched.

### Editorial

- New `editorial/v2.1/` (local, not committed): the full voice review, the rewrite brief used for the pass, and `voice_diagnostics.py`, a script that measures the drift patterns per chapter.

---

## [2.0] — 2026-05

The second edition. Same backbone. New chapter. Tighter prose.

### Added

- **New chapter: *AI Is the New OS*** (Chapter 13). A standalone treatment of what AI changes — and what it doesn't — for builders. Written in two movements (Under the Bar, In the Boardroom) with a closing argument that the motto holds. Roughly 3,000 words. Sits between the original Chapter 12 and the Conclusion.
- **New front-matter note: *A Note on the Second Edition.*** A short framing for readers coming back from the first edition.
- **2024–2026 examples** added throughout: Cursor / Anysphere pivot (Ch 2), Linear's Cycles framework (Ch 3), Dovetail AI for research synthesis (Ch 4), Anthropic's Claude release cadence (Ch 5), Change Healthcare ransomware (Ch 8), Air Canada chatbot tribunal ruling (Ch 12), and the Humane AI Pin / Boeing Alaska Airlines 1282 pairings in Ch 1.
- **Drift framework named explicitly** in four chapters (1, 6, 12, 13) — recovery-shaped, legacy-shaped, AI-shaped — building on the original introduction in Chapter 1.
- **Motto attribution chain** strengthened. The motto's origin (VMM-364, the Marine tiltrotor squadron known as the Purple Foxes) is named in the Prologue. Personal transmission from Nathaniel Fick at Endgame is preserved in Chapter 1. The motto recurs in Chapters 8, 13, and 14.

### Changed

- **Subtitle.** Previously *Lessons from the Barbell and the Boardroom.* Now *A Field Guide for Building Things That Matter.*
- **Sources** section curated and renamed. The prior open-ended Further Reading list (~84 entries) is now a load-bearing Sources section (~63 entries) supporting specific claims, quotes, and named events.
- **Acknowledgments** restructured. *To my beyond* now opens. Veteran mentions and Nathaniel Fick combined into one paragraph.
- **Prose tightened throughout.** Roughly 1,700 words cut from chapters 1–12 for spine and clarity. No examples were removed; only padding.
- **Chapter 4** (*Feedback Is a Superpower*) tightened to remove the cross-section overlap between *Strong Feedback Builds Strong People* and *Listening Is a Lift*.
- **Chapter 7** (*Train the Engine*) deepened with the Endgame architectural rebuild story (front end language, agent communication, back end architecture).
- **Chapter 9** (*Ship It Like You Show Up*) anchored with the Red Flag launch payoff — the agent worked, red team asked to turn down protections, operator's award.
- **Chapter 11** epigraph: *"The hardest lift is putting your ego down."*
- **Chapter 9** epigraph: *"Empathy isn't softness, it's clarity."*

### Removed

- The "Lovable" reference from Acknowledgments.
- The standalone Strong Feedback Builds Strong People / Listening Is a Lift overlap in Ch 4.
- Roughly 1,700 words of prose padding spread across chapters 1–12.

### Repository

- **Restructured.** The repo previously held only a README and brand assets. It now hosts the actual manuscript (single file at [`manuscript.md`](manuscript.md), and chapter-by-chapter in [`book/`](book/)).
- New **CONTRIBUTING.md** describing how to PR a fix.
- New **CHANGELOG.md** (this file).
- Brand-icon PNGs moved to [`assets/`](assets/).

---

## [1.13] — 2025

The first edition. Originally published as *Mission Built: Lessons from the Barbell and the Boardroom.*

Twelve chapters plus prologue and conclusion. Foreword by the Loadout. Released under CC BY-NC-SA 4.0.

The first edition is preserved at [missionbuilt.io](https://missionbuilt.io) under the version-1 archive.

---

## Earlier

Pre-1.0 development happened in private. The first public release was version 1.0 in mid-2025; subsequent point releases through 1.13 carried minor corrections and source updates.
