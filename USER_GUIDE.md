# WhaGrOU — a quick guide

**What it is.** WhaGrOU is a calm desktop app that helps you stay personally connected
on WhatsApp. It finds people you've drifted out of touch with, drafts a warm message to
each — in your own voice — and lets you reach the members of a group one‑to‑one. **Nothing
is ever sent without you approving it.** Everything runs on your own computer; there's no
server and nothing is uploaded.

---

## First time (about 10 minutes)

### Opening the app the first time

WhaGrOU isn't signed with an Apple developer certificate (or a paid Windows one) —
that's expected for a free indie tool; the app is built straight from the public
release you downloaded. Your computer is just being cautious. You only do this once.

**Mac — macOS 15 Sequoia and later:**

1. Open WhaGrOU once. macOS blocks it ("Apple could not verify…"). Click **Done**
   (not *Move to Trash*).
2. Open **System Settings → Privacy & Security**, scroll down to the **Security**
   section, and click **Open Anyway** next to the WhaGrOU message.
3. Confirm with **Open Anyway** (Touch ID or your password). From then on it opens
   like any other app.

> **Older macOS (14 Sonoma and earlier)?** There's a shortcut: **right‑click the
> app → Open → Open**. (On Sequoia and later this no longer works — use the steps
> above.) Power users can instead run
> `xattr -dr com.apple.quarantine /Applications/WhaGrOU.app` in Terminal.

**Windows:**

If SmartScreen shows a blue **"Windows protected your PC"** screen, click
**More info**, then **Run anyway**.

### Set it up

1. **Open WhaGrOU** and go to **Settings**.
2. **Link WhatsApp** — click *Open / Scan QR* and scan the code with your phone
   (WhatsApp → Linked Devices → Link a Device). This is the same as WhatsApp Web.
3. **Add your AI key** — paste your Anthropic API key in *Settings → AI → Save*. It's
   stored only in your Mac's Keychain.
4. **Pull your photos** (optional) — *Settings → Refresh photos* fetches contact pictures.

> Tip: the more you use it, the better it learns your voice — it reads how *you* actually
> write to each person.

---

## Bring in your old chats (optional)

WhaGrOU writes in *your* voice by reading how you've actually talked with each
person — so the more history it can see, the better the drafts. There are two ways
to bring your history in.

### Option A — Everything at once (full backup, Android)

Import your entire WhatsApp history — every 1:1 contact and all their messages — in
one go. This is the fastest way to get set up.

1. **Turn on an encrypted backup with a 64‑digit key.** On your phone, open
   **WhatsApp → Settings → Chats → Chat backup → End‑to‑end encrypted backup →
   Turn on**, and choose **"Use a 64‑digit encryption key instead"** (not a
   password). Write the 64‑character key down — you'll paste it into WhaGrOU. Let the
   backup finish.

2. **Copy your database file to your computer.** Connect your Android phone by USB
   and copy the file at
   `Internal storage → Android → media → com.whatsapp → WhatsApp → Databases →
   msgstore.db.crypt15`
   (older phones: `Internal storage → WhatsApp → Databases → msgstore.db.crypt15`).
   It's the most recent `msgstore.db.crypt15`.

3. **Import it.** In WhaGrOU go to **Settings → Import old data → Full WhatsApp
   backup**, paste your **64‑digit key**, click **Choose backup**, and pick the
   `msgstore.db.crypt15` file. WhaGrOU decrypts it **on your own computer**, then adds
   every 1:1 contact and their full message history. Already‑imported messages are
   skipped, so re‑importing is always safe.

> **iPhone?** Apple doesn't let apps read the WhatsApp database file, so use Option B
> below for the chats that matter most.

### Option B — One chat at a time (any phone)

1. **Export the chat from WhatsApp** (on your phone):
   - **iPhone** — open the chat → tap the person's name at the top → scroll down →
     **Export Chat** → **Without Media**.
   - **Android** — open the chat → **⋮** (top‑right) → **More** → **Export chat** →
     **Without Media**.
   - Send the file to yourself (AirDrop, email, or *Save to Files*) so it lands on
     your computer. It's a plain `.txt` file.

2. **Tell WhaGrOU who *you* are.** In **Settings → Identity → Your name**, type the
   exact name that appears as the sender on *your* own messages in the export. That's
   how WhaGrOU tells your side of the conversation from theirs. You only do this once.

3. **Import it.** Go to **Settings → Import old data → WhatsApp chat export →
   Choose .txt** and pick the file you exported. WhaGrOU reads the full history,
   matches it to the right contact (or creates one), and skips anything it already
   has — so re‑importing is always safe.

> Have a spreadsheet of people instead? **Settings → Import old data → Contacts CSV**
> adds them in bulk from a simple `name, phone` file.

Everything you import is read **locally on your own computer and never uploaded** —
same as everything else in WhaGrOU.

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
| **Settings** | WhatsApp link, AI key, import old chats, sending pace + daily cap, quiet hours, your name. |

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
