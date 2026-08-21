# QA report

Result of the release checks for version 1.0.0, run on 2026-08-18.

## Summary

| Check | Result |
|---|---|
| Entries | 96 across 12 categories |
| Required files | Present |
| Issue forms parse against GitHub's schema | Pass |
| README section order and canonical names | Pass |
| Contents block — every section listed, every anchor resolves | Pass |
| Entry format on every entry | Pass |
| Alphabetical ordering within every category | Pass |
| Duplicate names | None |
| Duplicate URLs | None |
| Pricing and platform labels within the vocabularies | Pass |
| Description length and quality rules | Pass |
| TiorAI link budget | 2 deep links, 2.1% of entries (cap 15%) |
| External links checked | 96 |
| **Broken links** | **0** |
| Secret and credential scan | Clean |
| Internal URL and local path scan | Clean |

## Categories

| Category | Entries |
|---|---:|
| Coding agents | 10 |
| Browser and computer-use agents | 8 |
| Research agents | 7 |
| Customer support agents | 8 |
| Sales and outbound agents | 7 |
| Data and analytics agents | 5 |
| Workflow automation agents | 8 |
| Agent building platforms | 8 |
| Agent frameworks | 11 |
| Multi-agent orchestration | 7 |
| Agent infrastructure | 10 |
| Evaluation and observability | 7 |

Every category holds at least 4 entries, and none exceeds the ceiling of roughly 15.

## Link checking

Method: browser user agent, redirects followed to a depth of 8, 12-second connect and
30-second total timeout, at least 400ms between requests to the same host, single flight per
host, `HEAD` first with a `GET` fallback.

- **Answered normally:** 87
- **Bot protection or rate limit:** 9
- **Broken:** 0

Hosts that challenged the checker: `consensus.app`, `devin.ai`, `flowiseai.com`, `gptr.dev`, `julius.ai`, `www.ada.cx`, `www.make.com`, `www.parloa.com`, `www.perplexity.ai`.

None is treated as dead. A challenged host was re-probed by a second route, normally the bare
origin and then `robots.txt`, and confirmed to be answering. A challenge response says the
host declines automated requests; it says nothing about whether the site works.

A small number of hosts refused every request from this build network, including the bare origin. Rather than record them as broken or quietly drop the entries, each was confirmed live through an independent route, and the evidence is kept in the build record:

| URL | Checker result | Confirmed by |
|---|---|---|
| `https://flowiseai.com/` | connection timeout (WinError 10060) | independent web search index |
| `https://gptr.dev/` | connection timeout (WinError 10060) | independent web search index, plus the project's GitHub repository |
| `https://www.parloa.com/` | connection timeout (WinError 10060) | independent web search index |

**Broken links:** None.

TiorAI links were verified separately: 5 checked, 5 resolved with a
`200`, 0 broken.

## What QA does not cover

Automated checks confirm that a URL resolves, that the format is right, and that ordering and
vocabularies hold. They cannot confirm that a description is accurate or that a product still
does what it claims. Those were checked by reading each category back as a block against the
vendor's current site, which is also the only way the "could these two descriptions swap
places unnoticed" test can be applied.

Pricing is the fastest-moving fact here and the most likely to be wrong first. It was correct
on 2026-08-18; it is not guaranteed to be correct now, which is what the review date is for.
