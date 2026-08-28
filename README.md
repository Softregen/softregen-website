# softregen-website

The Softregen company website — **softregen.com**.

Public by necessity as well as by nature: GitHub Pages does not serve a private repository on the
`free` plan, and a marketing site is public content anyway.

> ⚠️ **This repository is public.** Nothing confidential, no credentials, no customer detail, no
> internal fleet tooling. Product and infrastructure work belongs in the private product repository.

## What this is

One site, one audience. Softregen builds two things — an EU AI Act compliance product and the engine
underneath it — and the site exists so that a person who hears about either can establish, in about a
minute, that the company is real and competent.

```
softregen.com
├─ /            Softregen — who we are and what we build
├─ /ask         The chat: what the EU AI Act requires, and what AIMS Agent does about it
├─ /aims        AIMS Agent — the compliance product   → app at aimsagent.ai
├─ /eventus     EventusBuilder — the engine underneath. Named, not sold.
└─ /contact     One route in
```

`aimsagent.ai` is the **product's** address, where people sign in and work. This site explains; that
one does.

## Status

**Nothing is built yet.** The design is finished and lives in the private product repository:

- `docs/superpowers/specs/2026-08-26-softregen-website-design.md` — structure, guardrails, hosting, phasing
- `docs/plans/2026-08-26-ai-help-and-ai-chat-eb-flow.md` — how the chat works and where conversations are stored

### Phases

| phase | contents | blocked by |
|---|---|---|
| **1** | `/`, `/aims`, `/eventus`, `/contact` — static | **nothing** |
| 2 | `/ask` — the chat | a server, the chat entities, the AI-help rail |
| 3 | registration continues the conversation | Clerk wired to the chat, privacy notice, deletion route |
| 4 | link out to product options | the product hosted and its wizard finished |

Phase 1 does not depend on any of the later ones. It should ship first and on its own.

## Decisions already made

- **One site, a section per product** — the company's track record is what makes two unknown products
  credible, so splitting them across domains would start each from zero trust.
- **EventusBuilder is named, not sold.** Its licence question is unresolved, and a sales page would
  commit before that decision.
- **The chat explains, but never rules.** It cites Articles and Annexes; it will not tell a visitor
  whether their own system is high-risk, because that needs their system properly described — which is
  what the product is for. The limit is the argument, not a caveat.
- **No contact form** until there is volume to manage. An email address and a scheduling link.
- **No live human chat.** Two people across time zones cannot answer it, and an unanswered chat bubble
  reads worse than none.

## Where issues go

| about | where |
|---|---|
| this site — content, layout, build, deploy | **here** |
| the chat backend, storage, the product | the private product repository |

No project board. A label and a milestone do the same job without spending the GraphQL budget the rest
of the fleet shares.

---

Softregen LLC
