# Session Record: voice style guide template

```yaml
session_id: "session-2026-07-27-voice-style-guide-template"
runtime_session_id: "cowork-desktop-not-exposed"
date: "2026-07-27"
topic: "voice-style-guide-template"
status: "closed"
surface: "cowork"
provider: "anthropic"
model: "claude-sonnet-5"
operator: "the-operator"
repo_scope:
  - "infinite-brain-os"
goal: "Add a genericized voice style guide buildout method and blank scaffold to this template brain, so future brains forked from it inherit a reusable pattern for capturing an operator's actual writing voice, without carrying any specific operator's personal content."
linked:
  project: ""
  task: ""
  sprint: ""
  namespace: "personal-operator"
transcript_paths:
  - "sessions/logs/2026-07-27-voice-style-guide-template.log.md"
metering:
  usage_capture_status: "unavailable"
  usage_source: "Cowork desktop session; no token or cost metering is exposed to the agent in this environment"
  captured_at: ""
  input_tokens:
  output_tokens:
  cached_input_tokens:
  tool_calls:
  tool_cost_usd:
  estimated_cost_usd:
  usage_notes: "Metering fields intentionally left blank rather than estimated."
loaded_context:
  canon: []
  skills: []
  agents: []
  workflows: []
  nodes: ["knowledge/personal-operator/INDEX.md", "knowledge/personal-operator/playbooks/namespace-buildout-sprint-pattern.md", "knowledge/personal-operator/synthesis/template-vs-real-guide.md"]
```

## Goal

This brain is registered as an active reference fork of the public Infinite Brain OS starter, kept close
to stock so it stays mergeable with upstream, and is meant to be the template future brains are cloned
from. The task was to carry the operator's voice style guide work here in template form, not as this
specific operator's filled in content, per the operator's own direction that infinite-brain-os carries
the voice directives as a template to pass along, while the other three brains carry current directives.

## Assumptions and open questions

- Assumption: a fictional filled in example, matching the `_examples/about-this-company.md` pattern,
  would be actively misleading for a voice guide specifically, since the whole point of the method is
  empirical extraction from real samples. Chose a blank scaffold with instructions instead, placed as a
  real playbook rather than a fictional teaching scaffold.
- Assumption: this namespace's existing generic `s/he` pronoun convention, visible in `INDEX.md` before
  any edit, should be matched rather than defaulting to `he`, since this brain is not personalized to
  any specific operator.
- Open question: whether the operator wants a similar genericized scaffold added for other Sihaya
  specific assets in the future, or whether this one playbook is sufficient for now.

## Running notes

- This brain's `_system/validate.sh` and several of its check scripts carry Windows line endings and
  fail to run directly in this sandbox's bash. Ran a non destructive copy through `sed` to strip carriage
  returns and validated against that copy instead of the tracked file, so the tracked file itself was
  never modified to work around a pre-existing, unrelated infrastructure issue. 228 node files checked;
  the run's 7 failures are all pre-existing stock-starter issues (missing namespace frontmatter, a
  missing base surface in emberline-studio, a tool-three-layer check script with the same line-ending
  issue), none referencing the new file or the edited INDEX.md.
- Verified zero em or en dashes in the new file and in the edited section of INDEX.md.

## Outputs and changed files

- `knowledge/personal-operator/playbooks/voice-style-guide-buildout-method.md` (new)
- `knowledge/personal-operator/INDEX.md` (edited, added the new playbook to What is here and Map)

## Usage receipt

- Usage capture status: unavailable, see metering block above.

## Swarm touchpoints

- None.

## Closeout pointer

- `sessions/reviews/2026-07-27-voice-style-guide-template-closeout.md`
