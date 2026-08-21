# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 288 |
| Shortlisted after scope filtering | 134 |
| **Published** | **96** |

## Why candidates were dropped

- **Not actually agentic.** The largest exclusion by far. A chat interface with tool calling is an assistant; an agent decides what to do next and keeps going. Products marketed as agents that ship a single-shot prompt with a webhook were dropped.
- **Abandoned.** A large share of the agent projects that were prominent in 2023 and 2024 have had no meaningful commit in over a year. Popularity at the time is not a reason to list something now.
- **Absorbed or renamed.** Several frameworks were folded into a vendor's main SDK. The surviving name is listed; the historical one is not.
- **Demo repositories.** Star counts on agent repositories are unusually detached from whether anyone can run the thing.
- **Duplicate abstraction.** Where several libraries wrap the same idea with no meaningful difference, the maintained one is listed.
- **Category already well covered.** Applied hardest to frameworks, where the count could easily have tripled without helping anyone choose.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 96 distinct external URLs were checked:
87 answered normally, 9 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
