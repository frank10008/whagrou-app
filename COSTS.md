# WhaGrOU — what it costs to run

WhaGrOU itself is free and runs on your computer. The only cost is the **AI** that writes
the drafts, billed by **Anthropic** to **your own API key** — you pay only for what you use,
and it's small. (WhaGrOU never charges you; there's no subscription.)

## The models it uses

| Job | Model | Why |
|---|---|---|
| Reading tone / quick checks | **Haiku** (cheapest) | fast, light |
| Building profiles + writing drafts | **Sonnet** | the everyday workhorse |
| "Best" regeneration (optional) | **Opus** | only when you ask for it |

Anthropic bills per **million tokens** (≈ 750k words). Approximate rates — **check
anthropic.com/pricing for the current numbers**, they change:

| Model | Input (per 1M) | Output (per 1M) |
|---|---|---|
| Haiku | ~ $1 | ~ $5 |
| Sonnet | ~ $3 | ~ $15 |
| Opus | ~ $15 | ~ $75 |

WhaGrOU uses **prompt caching**, so the shared instructions in a batch are billed once, not
per message — which keeps batch costs down.

## What that means in real money

| You do… | Roughly costs |
|---|---|
| One **draft** | ~ **1¢** |
| Building one **contact profile** (once) | ~ **2¢** |
| A **batch of 50** reconnections (first time, profiles + drafts) | ~ **$1–1.50** |
| The same batch later (profiles already built) | ~ **$0.50** |
| A personal note to a **300‑member group** (rotated variations) | ~ **20–40¢** |
| Profiling **all ~2,000 contacts** once (spread out, only as you use them) | ~ **$30–40 total, one time** |
| A teacher reconnecting with **~50–100 people a week** | ~ **$2–6 / month** |

So a typical teacher spends a **few dollars a month**, often less. Profiles are built lazily
(only when a contact is actually drafted), so you never pay up front for people you don't message.

## Keeping it low

- Drafts default to **Sonnet**, not Opus — Opus is opt‑in for "make this one perfect."
- Caching means re‑scanning the same batch is cheap.
- **Large groups rotate** a handful of wording variations instead of writing one draft per
  person — so reaching a 300‑member group costs cents, not dollars.
- You set a **daily cap**, which also caps spend.

> Want to watch your spend live? **Settings → Usage & cost** shows tokens used and the
> estimated dollar amount, today and this month.
