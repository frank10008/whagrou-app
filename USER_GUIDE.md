# WhaGrOU — a quick guide

**What it is.** WhaGrOU is a calm desktop app that helps you stay personally connected
on WhatsApp. It finds people you've drifted out of touch with, drafts a warm message to
each — in your own voice — and lets you reach the members of a group one‑to‑one. **Nothing
is ever sent without you approving it.** Everything runs on your own computer; there's no
server and nothing is uploaded.

---

## First time (about 10 minutes)

1. **Open WhaGrOU** and go to **Settings**.
2. **Link WhatsApp** — click *Open / Scan QR* and scan the code with your phone
   (WhatsApp → Linked Devices → Link a Device). This is the same as WhatsApp Web.
3. **Add your AI key** — paste your Anthropic API key in *Settings → AI → Save*. It's
   stored only in your Mac's Keychain.
4. **Pull your photos** (optional) — *Settings → Refresh photos* fetches contact pictures.

> Tip: the more you use it, the better it learns your voice — it reads how *you* actually
> write to each person.

---

## Your everyday flow — daily reconnections

**Today** → click **Scan & draft**. WhaGrOU picks a balanced set of stale contacts (some
recent, some long‑lost) and writes each a short, warm message. Pick any batch size you like.

For each draft you can:
- **Edit** the wording right in the box,
- **Approve** (it joins the send queue),
- **Skip**, or **Regenerate** (optionally with a hint like "shorter" or "mention the retreat").

Then **Send approved** — messages go out one at a time, with natural pauses and a daily
cap, so it never looks like spam.

---

## Reaching a group, one person at a time

Open **Groups**, pick a group, and type what you want everyone to hear — in your own words
(*"Leaving for ice at 6:30 — there by 7, ok?"* or *"Invite everyone to Sunday's satsang"*).
Click **Draft a personal message for each**. You get an individual 1:1 draft for every
member — never a broadcast — which you then review and send like any other batch.

A few things that make this work even when WhatsApp hides numbers:

- **Friends with no saved number.** WhatsApp now hides many group members' phone numbers
  (shown as "@lid"). If you've ever chatted with that person, WhaGrOU reaches them
  **through your existing 1:1 chat** — no number needed. The group shows these as
  *"via existing chat."*
- **Add a number.** For someone you've *never* chatted with, open them under **Show
  members**, and add their real number in their profile (**Add number**). They become
  directly reachable.
- **Large groups rotate the wording.** Above ~25 recipients, WhaGrOU writes a small pool of
  distinct wording variations (per language) and rotates them across everyone — so it's
  fast, cheap, and never reads as copy‑pasted. A **Cancel** button stops a long run anytime.
- **Send a group more than once.** You can message the same group again later with a
  *different* note — only an identical, repeated message is blocked (so you can't
  double‑send by accident).

---

## The tabs

| Tab | What it's for |
|---|---|
| **Today** | Your daily batch of reconnect drafts to review. |
| **Contacts** | Everyone, searchable, with photos. Click anyone to see their profile, your history, your private notes, add a number, or rebuild their AI profile. |
| **Groups** | Open a group, give an instruction, and get a personal 1:1 draft for every reachable member (including friends reached via your existing chat). |
| **Review** | All drafts awaiting approval, across reconnections and groups. |
| **Outbox** | What's queued, sent, failed, or skipped — your delivery log. |
| **Activity** | An audit trail of every draft, approval, and send. |
| **Settings** | WhatsApp link, AI key, sending pace + daily cap, quiet hours, your name. |

---

## Sending safely — how many is OK?

WhatsApp can restrict accounts that look like they're blasting strangers. The good news:
**the thing that matters most isn't the number — it's whether people welcome the message.**
Bans are driven mostly by **blocks and reports**, so messaging your own community in your own
voice is far safer than cold spam. Still, a few sensible habits:

- **Nothing sends on its own — you pace it by what you approve.** For a big push, approve in
  **waves** (e.g. ~50, see how the first day lands, then approve more).
- **Two limits live in Settings.** A **daily cap** (total messages/day) and a separate, much
  stricter **first‑ever‑contact cap** (people you've never messaged before — the real risk).
  The cold cap stays on no matter how high you set the daily cap.
- **Warm vs. cold.** People you already chat with can be messaged at a healthy pace. *Brand‑new*
  contacts should trickle out slowly — keep that cap low and watch the first day.
- **Watch for blocks/reports.** One or two is noise; a cluster means stop and reassess.
- **Use your normal, established number** — not a brand‑new SIM, which is far more fragile.

There's no official magic number, but for an established personal account messaging its own
community, a few dozen to a couple hundred warm messages a day, spread out, is reasonable —
ramp up only if the first day stays clean.

---

## Good to know

- **It writes as you.** Drafts mirror your greetings, length, emoji habit, and language.
  Always glance over them — occasionally the AI adds a detail that isn't true; that's exactly
  what the review step is for.
- **Identify "unknown" contacts.** For someone you don't recognise, WhaGrOU can pull the
  conversation and work out who they are, then keep a little note on them.
- **Safety rails are always on:** approval required, human‑like delays, a daily limit, a
  cold‑contact limit, quiet hours, and no accidental duplicate sends.

---

## Your privacy

Your contacts, chats, drafts, and notes live in a single local file on your Mac
(`~/Library/Application Support/whagrou`). There is no WhaGrOU server. The only thing that
leaves your machine is the text sent to your own AI key to write a draft.
