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

## Your everyday flow

**Today** → click **Scan & draft**. WhaGrOU picks a balanced set of stale contacts (some
recent, some long‑lost) and writes each a short, warm message. Pick any batch size you like.

For each draft you can:
- **Edit** the wording right in the box,
- **Approve** (it joins the send queue),
- **Skip**, or **Regenerate** (optionally with a hint like "shorter" or "mention the retreat").

Then **Send approved** — messages go out one at a time, with natural pauses and a daily
cap, so it never looks like spam.

---

## The tabs

| Tab | What it's for |
|---|---|
| **Today** | Your daily batch of reconnect drafts to review. |
| **Contacts** | Everyone, searchable, with photos. Click anyone to see their profile, your history, your private notes, and rebuild their AI profile. |
| **Groups** | Search your groups; open one, give an instruction ("invite everyone to Sunday"), and get a personal 1:1 draft for every member. |
| **Review** | All drafts awaiting approval, across reactivation and groups. |
| **Outbox** | What's queued, sent, failed, or skipped — your delivery log. |
| **Activity** | An audit trail of every draft, approval, and send. |
| **Settings** | WhatsApp link, AI key, sending pace + daily cap, quiet hours, your name. |

---

## Good to know

- **It writes as you.** Drafts mirror your greetings, length, emoji habit, and language.
  Always glance over them — occasionally the AI adds a detail that isn't true; that's exactly
  what the review step is for.
- **Identify "unknown" contacts.** For someone you don't recognise, WhaGrOU can pull the
  conversation and work out who they are, then keep a little note on them.
- **Group members with hidden numbers.** WhatsApp now hides many members' phone numbers;
  WhaGrOU saves them by name and reaches the reachable ones — it never guesses a number.
- **Safety rails are always on:** approval required, human‑like delays, a daily limit,
  quiet hours, no duplicate sends.

---

## Your privacy

Your contacts, chats, drafts, and notes live in a single local file on your Mac
(`~/Library/Application Support/whagrou`). There is no WhaGrOU server. The only thing that
leaves your machine is the text sent to your own AI key to write a draft.
