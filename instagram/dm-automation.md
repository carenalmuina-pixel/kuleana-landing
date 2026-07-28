# Comment-to-DM Automation — @kuleanaclaims (KUL) & @yenclaims (MCC)

The captions in this repo use keyword CTAs ("DM 'POLICY' for a free review").
**Nothing responds automatically until this automation is set up** — this doc
is the build spec. Recommended tool: **ManyChat** (Instagram-API partner, one
dashboard for both accounts). Fallback: Meta Business Suite → Inbox →
Automations (per-account, more limited).

---

## Keyword triggers

Configure each keyword to match **comments on any post** and **new DMs**,
case-insensitive, "message contains" (so "Policy!", "POLICY 🙏" match):

| Keyword | Account | Purpose |
|---|---|---|
| `POLICY` | both | Free policy review request |
| `PROTECT` | MCC | Legacy CTA from earlier @yenclaims posts (IG DXBLjedjpRs) |
| `INSPECT` | KUL | Optional second CTA for inspection-focused posts |

Exclusions: don't trigger on comments made by the account itself; don't
re-trigger the same user within 30 days (ManyChat: set re-entry cooldown).

---

## Flow 1 — KUL (@kuleanaclaims)

**Trigger:** comment or DM contains `POLICY` (or `INSPECT`).

**Step 1 · Public comment reply** (only when triggered by a comment; rotate
3 variants so replies don't look robotic):
- "Aloha — just sent you a DM! 🌺"
- "Sent you the details in your inbox! 🤙"
- "Check your DMs — mahalo! 🌺"

**Step 2 · DM, immediately:**
> Aloha! 🌺 Thanks for reaching out about your policy. I offer free policy
> reviews for Hawaiʻi homeowners — no cost, no obligation, no pressure.
> Reply here with a good time to talk, call/text (808) 444-9420, or book at
> kuleanaclaims.com.
> — Caren, Licensed Public Adjuster, State of Hawaiʻi DCCA · Lic. #19246735

Buttons (ManyChat quick replies):
- **📞 Call/text now** → tel link (808) 444-9420
- **📅 Book online** → kuleanaclaims.com
- **💬 I have a question** → tags conversation `human-needed`, notifies Caren

**Step 3 · Follow-up, +24h if no reply and no button tap:**
> Just making sure this didn't get buried 🌺 If you'd like that free policy
> review, reply with a day and time that works and I'll call you — or if now's
> not the right season for it, no worries at all. Mahalo!

**Step 4 · Close-out:** any reply at any step tags `human-needed` and stops
automation — a person finishes the conversation. No further automated
messages after Step 3, ever (one follow-up maximum).

---

## Flow 2 — MCC (@yenclaims)

**Trigger:** comment or DM contains `POLICY` (or `PROTECT`).

**Step 1 · Public comment reply variants:**
- "Just sent you a DM! 👑"
- "Details are in your inbox! 👑"

**Step 2 · DM, immediately:**
> Thanks for reaching out! 👑 We offer free policy reviews so you know exactly
> what your coverage says before you need it. Reply with a good time to talk
> or call/text (305) 495-7177 and we'll take it from there.
> — Monarch Claims Consultants #ClaimWhatsYours

Buttons:
- **📞 Call/text now** → tel link (305) 495-7177
- **💬 I have a question** → tag `human-needed`, notify

**Step 3 · Follow-up, +24h if silent:**
> Following up in case this got buried 👑 If you'd like that free policy
> review, just reply with a good day and time and we'll call you. No pressure
> either way!

**Step 4 · Close-out:** same rule — any human reply stops the automation.

---

## Compliance guardrails (both accounts)

1. Auto-messages describe **free services and how to reach a human** — never
   outcomes, settlement amounts, or fee percentages (Hawaii DCCA / FL DFS
   advertising rules; see `compliance.md`).
2. KUL messages carry the license identity line; MCC messages should carry
   the Florida license identity once its number is confirmed for the footer.
3. One follow-up maximum, then silence — no drip sequences to non-responders.
4. During a declared disaster, review message tone before campaigns run
   (solicitation rules tighten post-catastrophe; when in doubt, pause the
   `PROTECT`/`INSPECT` campaigns and leave `POLICY` educational).
5. Log conversations that turn into claims consultations — the DM thread is
   often the first record of the client relationship.

## Setup checklist

- [ ] Both IG accounts switched to Professional (Business) and connected to
      their Facebook Pages.
- [ ] ManyChat Pro connected to both accounts (Settings → Instagram →
      connect; approve message permissions).
- [ ] Build Flow 1 and Flow 2 as above; set re-entry cooldown 30 days.
- [ ] Turn on ManyChat "Conversation started" notifications to Caren's phone
      for the `human-needed` tag.
- [ ] Test from a personal account: comment `POLICY` on a KUL post, confirm
      comment reply + DM + buttons; repeat on MCC.
- [ ] Only then publish captions that promise the keyword ("DM 'POLICY'…").
      Until the automation is live, phrase captions as "DM me the word
      POLICY" and answer manually.
