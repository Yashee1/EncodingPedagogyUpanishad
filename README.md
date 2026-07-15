# EncodingPedagogyUpanishad
TEI encoding pilot for pedagogical structures in the Kena and Katha Upanishads- DH2026

## What this is

This repository documents a pilot project that treats a TEI (Text Encoding
Initiative) schema as a research instrument, not just a delivery format. The
question driving it: what can a markup language carry about *teaching*, and
what does it drop?

Working from Patrick Olivelle's English translation of two Upanishads, this
project built a pedagogical ontology from close reading (thirteen categories,
seven carried forward for this pilot), then encoded it as a custom TEI
schema (ODD) treating every schema error encountered along the way as
data about where the initial reading had been imprecise, not just a bug to
fix quietly.

## Status
Work in progress. This is a pilot: seven passages, not a complete corpus.
Categories marked "excluded" in the schema are retained in the record but
not presented on the poster see `/docs` for the full rationale.

## Repository structure
/poster.pdf   DH2026 conference poster
/schema       the ODD customization and its generated RELAX NG schema
/corpus       TEI-encoded passages (short excerpts only — see note below)
/styles       author-mode CSS for reading-view rendering in Oxygen
/docs         methodology notes and category decision rules

## The category system
Seven pedagogical categories, each given a Western and (where genuinely
attested) an Indic technical term:

| Code | Category | Indic Term |
| A | Aporia | Neti Neti |
| D | Repetition | Āvṛtti |
| F | Readiness | Adhikāra |
| G | Analogy | Dṛṣṭānta |
| K | Outcome Statement | Phalaśruti |
| L | Negative Reference Group | — |
| M | Interior Motif | Guhā |

Six further categories were identified but excluded from this pilot's scope
(documented in `/docs`), either because they leaned on imported Western
vocabulary with no attested Indic counterpart, or because they did not hold
under re-testing.

## Method, briefly
Categories were not imported from a theory and applied, they were built
upward from plain-language observation across two close readings, then
progressively named using both Western pedagogical/rhetorical vocabulary
and Indic technical terms where the tradition offers its own. A category
was only promoted from "observed" to "named" once it appeared at least
three times across both texts. Full reasoning is in `/docs`.

## Validating the schema
The RELAX NG schema in `/schema` was generated from the ODD via
[Roma](https://roma.tei-c.org), the TEI Consortium's own ODD-to-schema tool.
To validate the corpus files against it, open them in
[Oxygen XML Editor](https://www.oxygenxml.com/) (or any RELAX NG–aware
validator) with the schema associated via an `xml-model` processing
instruction at the top of the XML file.

## A note on the source text
Verse excerpts in `/corpus` are drawn from Patrick Olivelle's translation,
*The Early Upaniṣads* (Oxford University Press, 1998). Excerpts here are
limited to short passages included solely to demonstrate the encoding
method; this repository is not a redistribution of the translation. All
rights to the translation remain with Olivelle and Oxford University Press.

## License
The schema, code, and original documentation in this repository are
released under the MIT License (see `LICENSE`). This license does **not**
extend to the quoted translation excerpts described above.

## Citation
> Frank Fischer, Yashee Singh(2026). *Encoding Pedagogy: Interpreting the Upanishads through Small-Scale Semantic Annotation* DH2026.
> https://github.com/Yashee1/EncodingPedagogyUpanishad

## Acknowledgments
Supervised by Prof. Dr. Frank Fischer, Chair, Digital Humanities, FU Berlin.
