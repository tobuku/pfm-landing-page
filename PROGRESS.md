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

## Top 10 Promotion Channels (Researched 2026-03-16)

### #1 — BiggerPockets Rehabbing & Flipping Forum
- **URL:** https://www.biggerpockets.com/forums/67-rehabbing-and-flipping-forum
- **Audience:** Investors
- **Reach:** 3M+ platform members, 210K+ forum posts
- **Tactic:** Value posts + case studies on draw inspection failures. Also list in BP Professional Services Directory (paid).
- **Hook:** "My HML charges $125 every time their inspector shows up — even when the contractor isn't done. Here's how I've passed 4 draws in a row on the first try."
- **Rules:** No overt self-promotion. Build 10–20 helpful posts before inserting product mentions.

### #2 — r/realestateinvesting (Reddit)
- **URL:** https://www.reddit.com/r/realestateinvesting/
- **Audience:** Investors
- **Reach:** 1.5M subscribers
- **Tactic:** Problem/solution story post. Comment authentically on threads about HML loans, remote investing, rehab management.
- **Hook:** "Remote investors: how are you verifying rehab progress between draw inspections without flying out or trusting a contractor's word?"
- **Rules:** Strict anti-spam. New accounts get filtered. No direct promotional posts.

### #3 — Facebook: "Wholesaling Houses Full Time"
- **URL:** https://www.facebook.com/groups/WholesalingFT/
- **Audience:** Investors
- **Reach:** Largest wholesaler FB group online
- **Tactic:** Participate 1–2 weeks first. Post scenario thread asking about draw inspection pain. Message admin about sponsored post slots.
- **Hook:** "When your HML inspector shows up and work isn't done, you lose the draw AND pay $125+ anyway. Here's how flippers are pre-verifying."
- **Rules:** Read pinned rules. Most groups allow tool posts on designated days.

### #4 — Connected Investors
- **URL:** https://connectedinvestors.com/
- **Audience:** Both (Investors + Boots on the Ground)
- **Reach:** 500K–2M members
- **Tactic:** Create company profile, post in Hard Money & Fix-and-Flip forums, contact for paid/sponsored listing. BG recruitment in "Bird Dogs" sections.
- **Rules:** Commercial promotion more accepted here than Reddit/BP, but account standing matters.

### #5 — 7 Figure Flipping Podcast (Guest Pitch)
- **URL:** https://www.7figureflipping.com/podcast
- **Audience:** Investors (serious 6–7 figure flippers)
- **Reach:** 31,700+ FB followers, top fix-and-flip podcast
- **Tactic:** Pitch as guest with founder story. Contact: contact@7figureflipping.com. Alternatively pitch for paid mid-roll sponsorship.
- **Hook:** "I realized every failed draw inspection is a $125+ tax on remote investors who could verify for under $50 with a local photographer."
- **Rules:** Must be founder/operator story — no pure product pitches.

### #6 — r/sidehustle (Reddit) — FOR BOOTS ON THE GROUND
- **URL:** https://www.reddit.com/r/sidehustle/
- **Audience:** Boots on the Ground
- **Reach:** 3.1M subscribers
- **Tactic:** Post as a user who found a new gig type — NOT as the company. "I've been doing a side hustle visiting houses, taking GPS-tagged photos for out-of-state investors — $30–$75 per property, paid via Stripe."
- **Rules:** No direct solicitation. First-person "gig I found" posts are allowed and perform very well.

### #7 — National REIA Network (Chapters + Newsletter)
- **URL:** https://nationalreia.org/ | Chapters: https://nationalreia.org/find-a-reia/
- **Audience:** Investors (primary), BG recruitable at local meetings
- **Reach:** 40,000 dues-paying members, 120+ local chapters
- **Tactic:** Sponsor National REIA newsletter. Contact local chapter leaders for 10-min guest presenter slot (in person or Zoom). Frame as draw-inspection optimization strategy.
- **Hook:** "Raise your hand if you've paid for a draw inspection that failed because the contractor wasn't done. [Pause.] I built a tool for exactly that problem."
- **Rules:** Each chapter independently operated. Some charge vendor fees. Pre-arrange with organizer.

### #8 — Facebook: "Real Estate Investors Group"
- **URL:** https://www.facebook.com/groups/realestategrouponline/
- **Audience:** Investors
- **Reach:** 131,000 members
- **Tactic:** Problem/solution thread — ask what their process is for remote rehab verification, then follow up with ProveForMe answer in comments. Also targetable via Facebook Ads.
- **Hook:** "Has anyone had a HML draw inspection fail because the contractor wasn't done? What did it cost you? This is a silent killer for flip margins."

### #9 — Flipping Mastery TV — Jerry Norton (YouTube)
- **URL:** https://www.youtube.com/c/FlippingMasteryTV
- **Audience:** Investors + BG recruitment
- **Reach:** 500K+ subscribers, 45M+ total views
- **Tactic:** Strategic comments on rehab/contractor/draw videos. Pitch team for sponsorship at https://flippingmastery.com. YouTube pre-roll ads targeted at fix-and-flip viewers.
- **Hook (comment):** "For draw inspection timing — ProveForMe.com lets locals take GPS-verified rehab photos before you call your HML inspector. Saves a lot of failed inspection fees."

### #10 — Facebook: "Private Money for Real Estate Investors" (HIGHEST INTENT)
- **URL:** https://www.facebook.com/groups/370850469716283/
- **Audience:** Investors — specifically hard money borrowers
- **Reach:** 22,000 hyper-targeted members
- **Tactic:** Case study post + admin partnership for tool demo or Live Q&A. Ask a data-driven question about draw inspection failure rates to spark discussion.
- **Hook:** "If your HML charges $125–$150 per inspection visit whether work is done or not, you need a way to verify before you make that call."
- **Rules:** Keep content tightly focused on the HML/private lending angle. Admin approval likely required for commercial posts.

### Priority Actions — Start This Week
1. **BiggerPockets Pro listing** — list ProveForMe in Professional Services directory
2. **Reddit double post** — "failed draw inspection" story on r/realestateinvesting + "new gig" on r/sidehustle
3. **7 Figure Flipping guest pitch** — email contact@7figureflipping.com with founder story
4. **Private Money FB group** — join and post a data-driven draw inspection question (highest-intent investor audience on this list)

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
