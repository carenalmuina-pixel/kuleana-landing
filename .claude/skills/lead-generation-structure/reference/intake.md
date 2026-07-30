# Intake — Ask This Before Building Anything

Everything downstream — compliance rules, content topics, caption voice,
automation copy, even which conversion channel to build — depends on the
answers here. A landing page or content calendar built without this context
ends up generic enough to belong to any competitor, which is the opposite of
what makes a lead-gen system work. If this is a live conversation, ask the
user directly. If it's an autonomous task with no one to ask, make the most
reasonable assumption from available context, state it explicitly in your
output, and flag it as an assumption rather than silently guessing.

## The questions

1. **What does the business do, in one sentence a stranger would
   understand?** Avoid jargon the customer doesn't use themselves.

2. **Who is the customer, and what triggers them to look for this business
   right now?** An emergency (burst pipe, injury, denied claim)? A recurring
   need (bookkeeping, haircuts)? A life event (buying a house, starting a
   business)? The trigger shapes the tone — urgent and reassuring vs.
   informative and unhurried.

3. **Is this a regulated or licensed profession?** Insurance, legal,
   medical, financial, contracting, real estate, and similar fields all have
   an advertising-rules layer that must inform copy from the first draft. If
   yes: what's the license/credential, which body regulates it, and where
   can a prospect verify it independently? → triggers
   `reference/compliance-framework.md`.

4. **How is the business paid?** Contingency ("no recovery, no fee"), flat
   fee, hourly, retainer, subscription, commission. The fee model often
   determines what can legally be said in an ad (e.g., some professions
   reserve exact fee percentages for the written contract, not marketing
   copy) and always determines what the CTA should emphasize ("free
   consultation" lands differently for a contingency practice than a
   by-the-hour one).

5. **What's the geographic service area?** Hyperlocal (a neighborhood or
   island), regional, statewide, national, or remote/anywhere. This affects
   everything from ad targeting to whether "island-wide" vs. "nationwide"
   belongs in the copy.

6. **What social or web assets already exist?** Active accounts, dormant
   accounts with a real follower history, an old website. Don't default to
   building from zero — a dormant account with an audience is often worth
   more than a fresh one. → triggers `reference/account-transformation.md`.

7. **Is there more than one brand or account to run?** Multiple service
   lines, multiple locations, a founder's personal brand alongside the
   company brand, or genuinely separate businesses sharing an owner. →
   triggers the multi-brand rules in `reference/posting-schedule.md`.

8. **What's the best conversion channel for this specific audience?** Phone
   call, DM, an online booking link, a web form, or a walk-in. High-stakes,
   high-trust purchases (anything involving money, health, or legal
   exposure) often convert better through a real, named person on the phone
   or in DMs than through a form that disappears into a CRM queue — but a
   high-volume, lower-stakes business might genuinely want the scale a form
   + autoresponder gives it. Don't assume a form is the default; ask.

9. **What should the business never promise, even informally?** Outcomes,
   settlement amounts, cure rates, guaranteed timelines, savings figures.
   Get this named explicitly up front — it's much easier to write good copy
   inside a known constraint than to catch a violation on review.

## Using the answers

Map each answer to what it triggers:

- Q3 (regulated) → do the compliance pass (`reference/compliance-framework.md`) before or alongside the landing page draft, not after.
- Q6 (existing dormant asset) → run the transformation playbook (`reference/account-transformation.md`) before publishing new content to that account.
- Q7 (multiple brands) → use the multi-brand posting-queue rules from the start (`reference/posting-schedule.md`), even if only one brand is active today — it's much easier to design the queue for multiple accounts from day one than to retrofit it later.
- Q8 (conversion channel) → build the DM/comment automation (`reference/dm-automation.md`) only if the answer is DM/comment; otherwise design a web-form + autoresponder equivalent using the same structure (immediate acknowledgment with a real next step, one timed follow-up, human handoff, no drip sequence).
