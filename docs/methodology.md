# Methodology and Category Rationale
This document explains how the seven pedagogical categories used in this
pilot were arrived at, why six further categories were identified but
excluded from this pilot's scope, and the decision rules used to keep
adjacent categories distinct during encoding.

## How categories were built
Categories were not imported from a pedagogical theory and applied to the
text. They were built upward from close reading, in three stages:
1. **Plain-language observation** both Upanishads were read twice, once
   without annotation, once marking any verse that felt like it contained a
   teaching move, described in the plainest possible terms (e.g. "use of an
   example to teach a lesson").
2. **Functional description** plain-language notes were re-read and
   clustered by similarity of function, without yet reaching for technical
   vocabulary.
3. **Technical naming** only once a cluster was stable did it receive a
   Western pedagogical/rhetorical term and, where the tradition offers a
   genuinely precise equivalent, an Indic term alongside it.
A cluster was only promoted to a named category once it appeared **three or
more times** across both texts. Three was chosen deliberately: across two
texts, finding one instance per text is easy — a third occurrence is what
turns a coincidence into a pattern.

## Final selection: seven categories
| Code | Category | Term | Occurrences |
| A | Aporia | Neti Neti | 7 |
| D | Repetition | Āvṛtti | 5 |
| F | Readiness | Adhikāra | 6 |
| G | Analogy | Dṛṣṭānta | 4 |
| K | Outcome Statement | Phalaśruti | 4 |
| L | Negative Reference Group | — | 3 |
| M | Interior Motif | Guhā | 4 |
These seven were selected for the poster and presentation because they show
the clearest term-parity between Western and Indic vocabulary, and are the
most consistently saturated across both texts.

## Excluded categories
Six further categories cleared the three-occurrence threshold but were
excluded from this pilot's scope. Exclusion here is a decision about scope
and confidence, not a claim that these categories are wrong. All six
remain fully defined in the project's working ontology.
- **B — Epistemic Humility.** Leans on imported Western vocabulary
  ("negative capability") with no comparably precise term the tradition
  uses for itself.
- **C — Assessment (Parīkṣā).** Every tagged instance already carries a
  secondary tag under another retained category, adding a category to
  defend without adding a distinct reading.
- **E — Anagnorisis.** Borrows a term from Aristotelian poetics rather than
  pedagogy, a parallel problem to B.
- **H — Formative Labelling.** The strongest evidence-based exclusion:
  tested twice under re-examination and did not hold cleanly either time,
  despite a respectable original occurrence count.
- **I — Inverted Scaffolding.** Imports a term from Vygotskian developmental
  psychology with no textual warrant from the tradition itself.
- **J — Imperative Closure.** Thinnest independent category by count; all
  instances already carry a companion tag under a retained category.

## Edge-case decision rules
Two category pairs proved hardest to distinguish during encoding. Each was
given an explicit, testable rule rather than left to per-verse judgment:
**A (Aporia) vs. G (Analogy)** — If the figure can be paraphrased as a
simile ("it is like...") without losing its point, tag G. If paraphrasing
destroys the point — because the faculty that would grasp it is itself what
is being grasped — tag A.
**F (Readiness) vs. H (Formative Labelling, excluded)** — If a passage shows
the student's own action or reasoning with no teacher commentary yet, tag
F. If the passage shows the teacher explicitly naming or classifying that
action, tag H, even immediately following an F-tagged passage.

## A note on sub-categories
During encoding, two patterns emerged that resembled possible sub-divisions
within existing categories: a "hard" vs. "soft" distinction within Aporia,
and an "ascending hierarchy" ladder-pattern within Analogy. Neither has been
formally promoted to a sub-category. Both are recorded here as observed
instances for future research, consistent with this project's position that
a pattern should only be named once it is genuinely stable — not simply
because it is noticed.

## Tagging conventions used in the schema
- The `@ana` attribute's **first pointer** is always the primary category
  for a passage; any further pointers are secondary tags on the same
  passage.
- `@type` on `<note>` is restricted to two values: `translationFlag` (a
  concern about the English translation's word choice) and `taggingNote` (a
  record of a category-testing or recoding decision). These are kept on
  separate tracks deliberately, so a translation concern is never confused
  with a methodological one.
