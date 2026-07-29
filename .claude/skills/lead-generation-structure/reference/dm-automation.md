# DM / Comment Lead-Capture Automation

Applies when intake (`reference/intake.md`, question 8) identifies DMs or
comments as the best conversion channel — typically Instagram, TikTok, or
Facebook, and especially for high-touch businesses where a real person
replying beats a form. If the best channel is a web form instead, use the
same *structure* below (immediate acknowledgment → one timed follow-up →
human handoff → no drip sequence) implemented as a form autoresponder plus a
CRM/inbox notification.

**Never publish a caption that promises an automated response before the
automation is actually built and tested end-to-end.** Until then, phrase the
CTA as a manual ask ("DM me the word [KEYWORD]") and answer by hand — a
caption that promises something the business hasn't built yet is the kind of
small trust violation that compounds.

## Structure

**Trigger.** Pick one primary keyword — short, on-brand, easy to type under
thumb-typo conditions. Match case-insensitively and as "contains" rather
than "equals" (so "keyword!", "KEYWORD 🙏" still match). Add: a cooldown so
the same person isn't re-triggered within some window (e.g. 30 days), and an
exclusion so the account's own comments/replies never self-trigger.

**Step 1 — public comment reply** (only fires when the trigger was a public
comment, not a direct DM). Rotate 2-3 short variants so replies don't read
as obviously robotic. This step also confirms to everyone else watching the
thread that a DM is coming — free social proof that the business actually
responds.

**Step 2 — immediate DM.** State the free/low-commitment offer in one or
two sentences. Include the credential/identity line if the business is
regulated (`reference/compliance-framework.md`). Offer 2-3 concrete
next-step buttons or quick replies:
- Call/text now (a `tel:` deep link where the platform supports it)
- Book online (a direct link)
- "I have a question" — this branch should **always** tag the conversation
  for human handoff. Automation should never attempt to actually answer a
  substantive question; its job is to acknowledge and route, not converse.

**Step 3 — one timed follow-up** (commonly +24h) if the person hasn't
replied or tapped a button. Restate the offer briefly, and give a graceful
out ("if now's not the right time, no worries at all"). This is the only
follow-up. No drip sequence, no second or third nudge — repeated automated
pings after silence read as spam and damage the account's standing with
both the platform and the prospect.

**Step 4 — human handoff and close-out.** Any reply, at any step, tags the
conversation for a human and stops further automation permanently for that
thread. A person finishes every real conversation; automation's only job is
to get the first response out fast and route correctly.

## Compliance guardrails

(Fold in the applicable rules from `reference/compliance-framework.md`
directly into the scripted messages — automation is still advertising.)

1. Automated messages describe free/low-commitment services and how to
   reach a human — never outcomes, amounts, or guarantees.
2. Include the credential/license line if regulated.
3. One follow-up maximum, then silence — no exceptions for "high-value"
   leads; the rule exists precisely so it doesn't need judgment calls in
   the moment.
4. During a declared emergency/disaster or other sensitive period, pause
   urgency-driven keyword campaigns and leave only educational content live
   — solicitation rules often tighten exactly then.
5. Log every conversation that turns into a real consultation or sale — the
   DM/comment thread is frequently the first record of the client
   relationship, and it's easy to lose if it only lives in the platform's
   inbox.

## Setup checklist

- [ ] Convert the account(s) to a business/professional/creator profile as
      the platform requires, and connect to whatever backing page/business
      account the automation tool needs.
- [ ] Choose an automation tool. A dedicated platform (e.g. ManyChat or
      similar) is usually more capable than the native in-app automation
      inbox, but the native tool is a reasonable fallback for a simpler
      setup.
- [ ] Build the flow exactly as scripted above; set the re-entry cooldown.
- [ ] Turn on a real-time notification to a human for anything tagged
      "human needed."
- [ ] **Test end-to-end from an outside account** before publishing any
      caption that promises the keyword — trigger it, confirm the comment
      reply, the DM, and the buttons all fire correctly.
- [ ] Only after that test passes, publish captions that promise the
      keyword. Until then, ask for the keyword manually and answer by hand.
