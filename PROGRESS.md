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
2. **Hero** — centered headline, subheadline, dual CTAs, dashboard mockup with real before/after photos
3. **Stat Bar** — 48hr / 100% / GPS / Skip the Trip
4. **Problem Section** — 3 pain point cards (travel cost, slow inspectors, draw delays)
5. **Solution Section** — 3 benefit cards (fast, independent, cost-effective)
6. **How It Works** — 4-step process with animated connector line
7. **Use Cases** — 6 cards (rehab verify, condition check, lender docs, occupancy, rental monitoring, pre-closing)
8. **Marketplace (Two Sides)** — Investor card + Boots on the Ground card with CTAs
9. **Trust Section** — 4 trust badges (GPS, Stripe, Independent, Clear Instructions)
10. **Final CTA** — dual buttons, "no credit card required"
11. **Footer** — logo, nav links, copyright

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
- [ ] **NEXT SESSION:** Build email campaign using `proveforus.com` as the CTA link to measure landing page conversion from email traffic

---

## Commit History Summary
| Commit | Changes |
|--------|---------|
| Initial | `hello world` placeholder |
| Launch | Full 9-section landing page, all CTA links to /register, logo integrated |
| Photos + Login | Real before/after property photos, Sign In → /login |
| GSAP + Polish | Full GSAP animation suite, hero centering, stat fix, video section removed |
