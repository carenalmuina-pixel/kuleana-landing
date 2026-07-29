# Trust-First Landing Page

The landing page's job is narrow: convert a stranger who already has some
intent (they clicked an ad, a bio link, or a DM button) into a call, a
booking, or a message. It is not a brochure of everything the business does
— it's a trust-transfer machine. Optimize for that.

## Structure

- **Utility bar (sticky, always visible).** Phone number as a `tel:` link
  plus a one-line credential or trust badge (license number, years in
  business, "family-owned since…", certification). It should never scroll
  out of view — the whole point is that the fastest possible path to contact
  is always one tap away, on every screen, at every scroll position.

- **Hero.** One sentence value proposition plus an emotional anchor — why
  this matters to the visitor *right now*, not a mission statement. One
  primary call-to-action button (call or book). Resist the urge to explain
  everything above the fold; the hero's job is to confirm "yes, this is the
  right place" and move the visitor to the CTA or further down the page.

- **Trust signals near the top.** License/certification, a "who we actually
  work for" framing if there's an adversarial third party in the picture
  (an insurance carrier, a landlord, an opposing party — naming that tension
  explicitly is often the single most persuasive line on the page), and any
  credibility markers (years of experience, volume of cases/clients,
  recognizable affiliations).

- **FAQ, grouped by theme, with a jump nav.** Universal buckets that work
  across most industries: **Basics** (what do you actually do), **How This
  Works** (the process, step by step), **Cost & Payment** (how the business
  gets paid, what it costs the customer up front), **Your Situation**
  (edge cases, "is it too late," "does this apply to me"). Write every
  answer in the customer's own words, not corporate language — a good FAQ
  page does double duty as SEO and as objection-handling, and it's often the
  page visitors spend the most time on before they call.

- **Closing CTA band, repeated at the bottom of every page.** Restate the
  primary CTA with a "no pressure, no obligation" framing. This matters more
  than it looks — for anxious or high-stakes purchases, reducing the
  activation energy of the *first* contact (a free look, no commitment) is
  usually more persuasive than any feature description.

- **Footer.** Legal/compliance line if the business is regulated (license
  number, regulating body, exactly as it should read per
  `reference/compliance-framework.md`), copyright, and repeated contact
  info.

## Choosing the primary conversion mechanism

Don't default to a web form. For a high-trust, high-stakes local service, a
phone number and/or a DM channel staffed by (or automated on behalf of) a
real named person tends to convert better than a form that disappears into
an inbox — the visitor is trusting a person, not a company. For a
higher-volume, lower-stakes, or fully remote business, a form with an
instant, specific autoresponder (not just "we'll be in touch") plus a CRM
notification can be the right default. Decide this deliberately during
intake (`reference/intake.md`, question 8) rather than defaulting to
whichever is easiest to build.

## A no-build-step technical option

For a solo operator or small business that needs something live today
without hiring a developer or standing up a build pipeline: a single,
self-contained HTML file — fonts and images inlined (as `@font-face` data
URIs / base64 images), no external dependencies, no bundler — deploys to any
static host (GitHub Pages with a custom domain via a `CNAME` file works
well) and is trivially editable by hand. This trades some engineering
elegance for zero infrastructure and zero build-time failure modes, which is
usually the right trade for a business whose next hire is a client, not an
engineer. Graduate to a proper framework/build step only once hand-editing a
single file genuinely becomes the bottleneck (many pages, a team of editors,
a need for a CMS) — don't reach for tooling complexity the business doesn't
need yet.
