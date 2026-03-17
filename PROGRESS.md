# ProveForUs.com Landing Page — Project Progress

## Project Overview
A standalone, high-converting landing page for **ProveForMe.com** hosted at **ProveForUs.com** via GitHub Pages.

- **Live URL:** https://proveforus.com
- **GitHub Pages URL:** https://tobuku.github.io/pfm-landing-page/
- **GitHub Repo:** https://github.com/tobuku/pfm-landing-page
- **CNAME:** `proveforus.com` (configured)

---

## Purpose
ProveForUs.com exists solely as a conversion landing page to sign up:
1. **Investors** — create an Investor Account at proveforme.com/register
2. **Boots on the Ground** — create a BG Account at proveforme.com/register

---

## Platform Links
| Action | URL |
|--------|-----|
| Create Account (Investor or BG) | https://www.proveforme.com/register |
| Sign In | https://www.proveforme.com/login |

---

## Page Sections (in order)
1. **Navigation** — sticky nav, logo, How It Works / Use Cases / For Investors links, Sign In + Create Account CTA
2. **Hero** — centered headline, italic cost tagline, subheadline, dual CTAs, dashboard mockup with real before/after photos
3. **Stat Bar** — 48hr / 100% / GPS / Skip the Trip
4. **Problem Section** — 3 pain point cards (travel cost, slow inspectors, draw delays)
5. **ROI Comparison Table** — side-by-side: flight vs. draw inspection vs. ProveForMe (cost + turnaround)
6. **Solution Section** — 3 benefit cards (fast, independent, cost-effective)
7. **How It Works** — 4-step process with animated connector line
8. **Use Cases** — 8 cards (stop failed inspections ★, rehab verify, condition check, lender docs, occupancy, rental monitoring, pre-closing, catch what others miss ★)
9. **Marketplace (Two Sides)** — Investor card + Boots on the Ground card with CTAs
10. **Trust Section** — 4 trust badges (GPS, Stripe, Independent, Clear Instructions)
11. **Final CTA** — dual buttons, "no credit card required"
12. **Footer** — logo, nav links, copyright

---

## Files in Repo
| File | Purpose |
|------|---------|
| `index.html` | Full landing page |
| `pfm-logo.png` | Logo (used in nav + footer) |
| `pfm-logo.jpg` | Logo alternate |
| `b4frnt.JPG` | Before photo — front exterior |
| `afterfrnt.jpeg` | After photo — front exterior |
| `b4ktn.JPG` | Before photo — kitchen |
| `aftrktn.JPG` | After photo — kitchen |
| `CNAME` | Custom domain: proveforus.com |
| `PROGRESS.md` | This file |

---

## GSAP Animations Implemented
All animations use **GSAP 3.12.5 + ScrollTrigger** via CDN (no build tools).

| Animation | Trigger | Details |
|-----------|---------|---------|
| Hero entrance timeline | Page load | Badge → headline → subtext → buttons → trust row → mockup card → floating badges → photo wipe |
| Before/After photo wipe | Part of hero timeline | `clipPath` wipe left-to-right, staggered 0.13s each |
| Floating badge loops | After hero TL completes | Gentle vertical float, sine easing, yoyo repeat |
| Stat bar counters | Scroll into view | 48hr and 100% count up; GPS + Skip the Trip pop in with spring |
| Section intro fade-up | Scroll into view | All `.section-intro` headings and subtext |
| Stagger card reveals | Scroll into view | All `.card` elements inside `[data-stagger]` containers |
| Marketplace card stagger | Scroll into view | `.mkt-card` elements stagger in |
| How It Works connector draw | Scroll into view | `scaleX` 0→1, left-to-right, 1.2s |
| How It Works step stagger | Scroll into view | `.how-step` elements stagger in 0.15s apart |

---

## Marketing Strategy (from session 2026-03-16)

### Positioning
- **Primary message:** "See your rehab. Not just hear about it."
- **One-liner:** ProveForMe is the on-demand property verification platform that gives remote investors independent, GPS-verified eyes on the ground — faster and cheaper than any alternative.
- **For Boots on the Ground:** "Get paid to be the local eyes investors can't afford to ignore."

### Key Value Proposition — Draw Inspection Cost Savings
**IMPORTANT — Accurate HML Inspector flow:**
- Hard money lenders require their OWN inspector to inspect and approve designated items before releasing a draw. ProveForMe does NOT replace that inspector.
- HML inspector fees: **$125–$150 per visit**, charged whether the work passes or not.
- If the GC's work is incomplete and the HML inspector shows up, the investor pays the full $125–$150 fee AND has to schedule another inspection (and pay again).
- ProveForMe value: A $25–$75 "trust but verify" check-in confirms the phase is fully complete *before* the investor calls the HML inspector — preventing the cost of a failed/repeat visit.
- Tagline: "ProveForMe doesn't replace your lender's inspector — it makes sure the work is done before you call one."

### Key Value Proposition — Catch What Others Miss
GCs focus on their contracted scope. HML inspectors check only designated draw items. Neither is tasked with — or looking for — issues like:
- Leaning or encroaching trees
- Gate issues or perimeter problems
- Property changes that surface between scheduled visits
- Issues a property manager wouldn't notice or report

These are real problems experienced by remote/out-of-state investors (including founder's personal experience). ProveForMe gives trusted, independent eyes on the **full picture** — not just the checklist. This is a major differentiator vs. any inspector or GC.

### Social Media Content Pillars
1. **Draw Inspection Hook** — "Did you know your hard money lender charges for every draw inspection? Use ProveForMe to verify before you call."
2. **Origin Story** — "A hard money lender asked me one question I couldn't answer: 'Who's your boots on the ground?' That question built ProveForMe."
3. **BG Recruitment** — "Earn cash this weekend without a 9-to-5. Get paid to take photos/videos for remote investors near you."
4. **Myth vs. Reality Carousel** — Myth: "I have to fly out." Reality: Local BG delivers GPS-verified photos in 48 hours for a fraction of the cost.
5. **Lender Trust Angle** — "Your lender doesn't take your word for it — they want GPS-stamped, time-verified, third-party proof. That's ProveForMe."

### Best Platforms
- **Facebook Groups** — Real estate investor groups are the fastest organic channel
- **Instagram / TikTok** — Short Reels showing before/after proof concept
- **LinkedIn** — For serious investors and hard money lenders

---

## Decisions & Notes

### Stat Bar — "Skip the Trip"
Original stat was `$0 / Travel cost to you` — removed because investors DO pay the BG a service fee, making `$0` misleading. Replaced with **"Skip the Trip" / "Pay for verification, not airfare"** which is 100% accurate and still compelling.

### Video Section
Removed temporarily. Section was: "Watch It in Action / See How ProveForMe Works / Demo video coming soon." Add back when a real demo video is ready to embed.

### Domain Strategy
- `ProveForMe.com` — main product/app platform
- `ProveForUs.com` — conversion landing page only (this repo)

---

## TODO / Future Work
- [ ] Add demo video when ready (re-add video section)
- [ ] Replace logo placeholder with final brand logo if updated
- [ ] Add real testimonials / social proof once platform has users
- [ ] Add pricing section if/when pricing is public
- [ ] Consider adding a FAQ section
- [ ] Set up Google Analytics or similar tracking
- [ ] A/B test CTA button copy
- [ ] Build email campaign using `proveforus.com` as the CTA link to measure landing page conversion from email traffic
- [ ] Build out social media content calendar (5 pillars documented in Marketing Strategy section above)
- [ ] Create content for the origin story post (the hard money lender question hook)

---

## Commit History Summary
| Commit | Changes |
|--------|---------|
| Initial | `hello world` placeholder |
| Launch | Full 9-section landing page, all CTA links to /register, logo integrated |
| Photos + Login | Real before/after property photos, Sign In → /login |
| GSAP + Polish | Full GSAP animation suite, hero centering, stat fix, video section removed |
| Marketing Update | Hero cost tagline, ROI comparison table (new section), "Stop Failed Inspections" use case card, marketing strategy docs in PROGRESS.md |
| Accuracy + Selling Points | Fix HML inspector accuracy ($125–$150, pass or fail), add "Catch What Others Miss" use case card, update ROI table and problem card copy, remove inaccurate hero tagline claim |
| Em Dash Removal | Removed all em dashes from landing page copy, replaced with commas or periods |
