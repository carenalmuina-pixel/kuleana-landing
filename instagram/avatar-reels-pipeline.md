# Avatar Reels Pipeline — Selenite + Caren's Voice (MCC & KUL)

How to produce more reels in the style of the newest @yenclaims post, using
the **Selenite** avatar and **Caren's own voiceover**, on both channels,
inside each state's rules. Nothing here is published automatically — every
reel goes through Caren's review first.

---

## 1 · Anatomy of the post we're replicating

**@yenclaims · DbVmUdsjkUT · posted Jul 28, 2026** ("Do this BEFORE the
next storm… or your claim starts at $0.") — archived in this repo:
`video/mcc-latest-post.mp4`, cover `img/mcc-latest-post-thumb.jpg`.

| Element | What it does |
|---|---|
| 8s, 9:16, cinematic golden-hour interior | Elegant, warm, *unmistakably Monarch* — a pattern interrupt in a niche full of storm-wreckage footage |
| Avatar figure in business attire walking through the room | Human presence without a filming day; reads as "the adjuster in the house" |
| `MONARCH` micro-watermark, top-left | Brand claim on every frame |
| 3 text cards on dark translucent panels | Hook ("…claim starts at **$0**") → instruction ("Film everything. *Today.*") → CTA card |
| Playfair italic headlines, gold accent words | Exactly the System-A brand book |
| Gold pill button "Comment "POLICY"" | Ties into the DM automation keyword |
| Personal promise ("I'll personally call you within 24 hours") | Converts a brand ad into a person you can reach |
| License line + full FL solicitation disclaimer **on the end card** and in the caption | Compliant twice over — this is the template to keep |
| Dust-particle transition, warm grade | Continuity between scenes |

Early numbers (first ~9 hours): 137 plays / 19 unique views — too early to
judge, but the format is the strongest thing on the feed and matches the
brand book perfectly. The one thing it lacks: **sound**. Adding Caren's
voice is the single highest-impact upgrade — reels with a human voice hold
attention longer and feel like advice, not advertising.

## 2 · The production pipeline

Per reel: ~4 assets, ~30–45 min of machine time, one 30-second phone
recording from Caren.

### Step A — Scenes (Selenite avatar)
Generate 2–3 brand-graded scenes with the **Selenite** Soul
(`552fcf5e-ffad-4faf-8f19-bf8bf5f6748b`) via Higgsfield:
1. `nano_banana_pro` still at native 2K (never 4K-upscale text) — Selenite
   in the branded scene: MCC = golden-hour interiors, marble, warm glass
   offices; KUL = lanai light, monstera shadows, plantation-style rooms.
2. `kling3_0_turbo` image-to-video, 5s, 9:16 per scene (walking, turning,
   pointing at a ceiling, opening a policy binder).

### Step B — Voice (Caren's own)
Two options, both "her voice":
- **Record it (recommended).** A 20–30s script read on the phone in a
  quiet room, voice memo → uploaded to the chat or Drive. Authentic,
  zero AI-voice questions, and the scripts are short.
- **Clone it (for scale).** One good 60–90s recording → Higgsfield
  `create_voice` → generate any script in her voice. Fine legally (it's
  her own voice, her consent), but treat clone output as AI-generated in
  the disclosure step below. Best reserved for batch weeks.
Optional polish either way: Adobe `media_enhance_speech` / Descript to
clean room noise.

### Step C — Assembly (in-repo, already proven)
The same ffmpeg pipeline that built the 7 KUL reels:
1. Text cards authored in HTML (brand fonts embedded) → transparent PNGs.
   MCC cards: Playfair + DM Sans, dark panel, gold accents. KUL cards:
   Cormorant/Cinzel, cream/terracotta panels.
2. Overlay cards on the Kling scenes, crossfade scenes, end on the CTA
   card with license + disclaimer.
3. Lay in the voiceover, `afade` out, export 1080×1920 H.264.

### Division of labor per reel
- Caren: pick the topic, read 30 seconds into her phone, approve the cut.
- Pipeline: everything else.

## 3 · Compliance — the per-state layer

Same reel skeleton, different legal skin. These are the non-negotiables
baked into the templates:

**MCC (@yenclaims — Florida, plus LA·TX·GA·CO where licensed):**
- Name + license on every ad: `Caren Almuina · FL Public Adjuster Lic.
  #W583930` — end card **and** caption.
- The solicitation disclaimer on every lead-generating reel, verbatim,
  on-screen and in caption: *"This is a solicitation for business. If you
  have had a claim for an insured property loss or damage and you are
  satisfied with the payment by your insurer, you may disregard this
  advertisement."*
- No settlement amounts, no outcome promises, no fee percentages.
- Post-catastrophe: FL tightens solicitation after declared events — pause
  keyword campaigns and keep content purely educational during/after a
  declared storm.

**KUL (@kuleanaclaims — Hawaiʻi):**
- License line every asset: `HI Public Adjuster License #19246735 ·
  Hawaiʻi DCCA Insurance Division`.
- HRS ch. 431 art. 9 (2020 NAIC-model act): no misrepresentation
  (§431:13-102), no advertising fee terms, "many claims" never "most,"
  no outcome promises.
- Law-update reels: cite the act number on-screen, describe what the law
  says, never advise a specific coverage decision.

**Both channels — AI transparency:**
- Selenite scenes and any cloned-voice narration are AI-generated: keep
  the caption line **"(Footage is an illustrative recreation.)"** and tag
  Meta's "AI-generated" label on upload when the content shows a
  realistic person. Recorded-voice narration needs no voice disclosure.
- Selenite is built from Caren's own likeness — publicity rights are hers.
  Don't use the avatar to depict things that didn't happen on a *specific
  real claim* (illustrative scenes: fine; fake case footage: no).

## 4 · Proposed first batch (on approval)

Six reels, alternating channels, topics straight from the existing queues:

| # | Channel | Topic (source) | CTA |
|---|---|---|---|
| 1 | MCC | Hurricane deductible math (checklist carousel companion) | Comment POLICY |
| 2 | KUL | The 10-minute phone baseline — Hawaiʻi version of the post analyzed above | DM POLICY |
| 3 | MCC | ACV vs. RCV in 20 seconds (tile M15–M17 companion) | Comment POLICY |
| 4 | KUL | The Hurricane Relief Fund is back (Act 296, 2025) | educational, no keyword |
| 5 | MCC | A denial is a position, not a verdict | Call (305) 495-7177 |
| 6 | KUL | Free inspection — what actually happens (voice remake) | DM POLICY |

Scripts are ~70 words each — ready to draft the moment Caren wants the
batch; she records six voice memos, the pipeline does the rest.
