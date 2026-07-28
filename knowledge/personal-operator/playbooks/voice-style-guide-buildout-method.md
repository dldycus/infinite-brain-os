---
id: "playbook-voice-style-guide-buildout-method"
aliases: ["playbook-voice-style-guide-buildout-method", "voice-style-guide-buildout-method"]
type: "Knowledge"
namespace: "personal-operator"
lifecycle_state: "research"
summary: "Reusable method and blank scaffold for building a directive-format voice style guide for the operator, so an agent can write in the operator's actual voice, mechanically, across registers. Genericized template, not filled in for any specific operator; copy the shape, fill it from real samples."
confidence: 0.85
retrieval_class: "domain"
export_class: "internal"
edges:
  - target: "[[operator-profile]]"
    relation: "supports"
    confidence: 0.75
created: "2026-07-27"
---

# Voice Style Guide Buildout Method

Derived from a real buildout run in a sibling deployment (see that deployment's own provenance record
for the full history; not restated here since this is a generic method node, not that deployment's
specific findings). Copy the method and the blank scaffold below when a new operator wants an agent to
write in his or her actual voice, mechanically, not just tonally.

## What the resulting guide is for

A directive format reference, never a personality profile. It should produce usable rules, never use X,
prefer Y over Z, rather than descriptive observations, tends to be formal. Organize it by register,
technical or notes, casual or internal, corporate or external persuasive, fiction, and any other register
the operator actually writes in, rather than one blended voice. Register shifting itself is a common,
stable trait worth naming explicitly rather than smoothing over as inconsistency; ask the operator
directly whether and why his or her voice shifts by context before assuming one blended voice would do.

## Method: two phases, in sequence

1. Static sample extraction. Have the operator supply raw writing samples, proposals, emails, before or
   after edit pairs, and extract mechanical patterns, sentence structure, punctuation, word choice, into
   directives. This phase is a reasonable starting point but produces weaker, less falsifiable findings
   on its own.
2. Head to head prediction versus actuality testing. For any register where the operator produces
   original content in scene or in context, fiction narration is the clearest case, draft a predicted
   response to a prompt before seeing the operator's actual reply, then compare the two directly. Every
   real miss directly overturns or refines a rule. This method is more diagnostic than static extraction
   alone and should become the primary engine once the guide has a base to test against.

## Method: periodic consolidation

As the guide grows past roughly one hundred fifty to two hundred lines, run a consolidation pass that
explicitly checks two things in both directions:

- whether a finding logged as an extension of an existing rule is actually a distinct finding mislabeled
  to fit a convenient bucket
- whether an existing merged rule is actually a false merge of two genuinely distinct findings

Both directions reliably turn up real corrections. An append only log of findings accumulates mislabeled
relationships if it is never re-examined, so schedule this pass deliberately rather than waiting for it
to become necessary.

## Confidence tiers

Track every directive at one of three tiers, and say so in the document itself rather than presenting
everything as equally settled:

- high confidence: confirmed by direct explanation plus multiple samples, or by explicit operator
  correction
- medium confidence: a pattern held across two to four samples, internally consistent, not yet stress
  tested further
- lower confidence, thin evidence: flagged as such, not treated as settled, a candidate for the next
  round of testing rather than a rule to apply confidently

## Known process pitfalls

- Editing a dense, multiply revised section from memory is risky. Re read the current file state
  immediately before editing a section that has already been touched more than once, rather than trusting
  recall of what it currently says.
- Round or pairing bookkeeping matters. Confirm what a new piece of input is actually responding to
  before logging it as a new, independent data point; feedback on a draft and the actual reply to that
  same draft can otherwise be mislogged as two separate rounds.
- A correction to structure discipline applies here too: if the operator corrects the same finding twice,
  absorb it into the rule directly rather than waiting for a third correction.

## Blank scaffold

Copy this section skeleton into the operator's own knowledge namespace, under a name such as
`synthesis/voice-style-guide.md`, and fill it from real samples. Do not invent example directives; an
empty field awaiting real evidence is honest, a fabricated rule is not.

```text
# Voice Style Guide

Governing concepts: name any deliberate, stable trait that explains why this operator's voice shifts
by context (or does not). State it plainly; do not assume one exists if the operator has not confirmed
it.

## 1. Source Samples Log
Table: sample, context, date pulled. Track what you pulled from, so gaps are visible later, for
example all samples being short messages, none long form.

## 2. Sentence Mechanics
Average length and variance, rhythm pattern, subordinate clause habits, fragment use, sentence openers.
Fill separately per register once more than one register is confirmed.

## 3. Punctuation Habits
Em dash, en dash, semicolon, comma, and period preferences, oxford comma, ellipsis use, parenthetical
frequency, exclamation point frequency.

## 4. Paragraph and Structure Rhythm
Typical paragraph length, how ideas transition, list versus prose preference, opening move, closing
move.

## 5. Word Level Habits
Overused words or phrases, avoided words or phrases including common AI tics, contraction default,
hedging language kept or cut, baseline register and what shifts it.

## 6. Voice Contrast Examples
For each confirmed finding: a generic or default version, the operator's actual version, and a one line
note on what changed. Real head to head pairs, prediction versus actual reply, are the strongest form
of this section.

## 7. Context Specific Variants
One subsection per confirmed register. State the deltas from the baseline explicitly rather than
repeating shared material.

## 8. Refinement Log
Table: date, what a draft got wrong, the rule added or changed in response. This is the audit trail for
every correction absorbed into the guide.

## 9. Open Items
Running list of unresolved questions, so they are not lost between sessions. Mark an item resolved in
place rather than deleting it, so the resolution's reasoning stays visible.
```
