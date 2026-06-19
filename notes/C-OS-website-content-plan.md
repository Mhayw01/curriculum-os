# SUPERSEDED — do not use

This draft jumped ahead to planning before grounding was aligned. The active document is **`01-bobldobl-grounding.md`**. Planning will resume only after the grounding is confirmed.

---

*(old draft below, retained only for reference)*

---

## 1. Grounding: where we're starting from

### The old product (bobldobl)
A single-page pre-launch landing site for **AI lesson planning**. Its whole story is built around one job: helping teachers find, edit, schedule and share individual lessons.

- **Headline:** "Revolutionise your lesson planning with AI"
- **Three pillars:** search/filter lessons · design your own resources · share & manage your curriculum
- **Features (all lesson-level):** find lessons instantly, edit & customise with AI, schedule & manage, share & collaborate, create from scratch
- **One CTA everywhere:** *Sign Up Now* → early-access offer (£50/yr, save £130, 1 month early, 1-on-1 founder training, user-testing invite, optional paid lesson creation)
- **Tone:** friendly, benefit-led, time-saving ("more time teaching, less time creating resources")

**The gap:** bobldobl sells a *tool that produces documents*. It's flat — you ask, it makes a lesson, done. There's no memory, no loop, no whole-curriculum view, and nothing for schools as organisations. That's exactly what C-OS is built to outgrow.

### Brand assets (carry forward)
From the Bobldobl Brand Logo Guide:

| Element | Value |
|---|---|
| Navy (primary) | `#093A5A` |
| Orange | `#FA602F` |
| Amber | `#D37F0F` |
| Mint | `#B8DED5` |
| Pink | `#E9496C` |
| Light grey | `#EFEFEF` |
| Typeface | SK Modernist (sans-serif), modern & simple |
| Logo logic | Monogram fusing **b + d** inside a **circle** = brand + audience synergy, global reach |

**Keep:** the palette, the SK Modernist type feel, the clean modern aesthetic.
**Change:** the logo. C-OS needs its own mark — a **book / open-book or stacked-layers** motif works (book = curriculum; layers = "operating system / stack"). Treat the circle device as optional heritage. *(Logo is a later task — flagged, not done here.)*

### Tech / repo
Repo `bobldobl-landing-page` (GitHub, private) is on your laptop but not in the connected folder, so I couldn't inspect it this session. Drop it into the **Curriculum OS** folder and I'll analyse the stack and reuse components for the rebuild. Hosting plan noted: **GitHub → Netlify → Squarespace DNS.**

---

## 2. Positioning: what C-OS *is*

> **bobldobl planned a lesson. Curriculum OS runs your teaching.**

Curriculum OS is the **operating system for teaching** — it doesn't just generate a lesson, it plans whole schemes of work, builds the resources, and then *learns from how each lesson actually went* to reshape what comes next. It's a partner, not a printout.

**One-line positioning:**
*Curriculum OS is the AI curriculum operating system that plans, builds, and adapts your teaching — a partner that learns from every lesson.*

**The category shift to land everywhere:**
| From (lesson planners) | To (Curriculum OS) |
|---|---|
| One lesson at a time | A whole term / scheme of work |
| A static document | A living curriculum that updates |
| You do the reflection | Reflections become tomorrow's actions, automatically |
| Same plan for every class | Regressions & progressions per learner |
| A tool you use | A partner that remembers |
| Built for one teacher | Org-aware: school knowledge baked into planning |

---

## 3. Messaging pillars (the 4 things C-OS does that a planner can't)

**1. It learns. (the headline differentiator)**
Add a quick reflection or feedback after each lesson; the next day's plan auto-updates with agreed actions and recommendations. The curriculum compounds instead of resetting.

**2. It builds, end-to-end.**
Generate worksheets, videos, and interactive lessons — and plan a full term's scheme of work — not just a single lesson outline.

**3. It adapts to every learner.**
Every lesson carries built-in **regressions and progressions**. A learner-level RAG system tracks preferences and surfaces actions for the teacher, so planning is personalised, not one-size-fits-all.

**4. It knows your school. (org tier)**
School accounts get an **organisation knowledge base** — upload your key skills docs, schemes, and standards, and the AI references them in every plan and recommendation. Plus automated learner reports and an optional registration/attendance module.

---

## 4. Audience framing

- **Primary (homepage lead):** individual teachers — the daily pain of planning, the relief of a partner that remembers. Drives self-serve early-access signups.
- **Secondary (dedicated track / "For Schools"):** schools & MATs/orgs — org RAG, embedded standards, automated reporting, attendance, consistency across staff. Higher contract value; drives "Book a demo."

Rationale: edtech adoption is bottom-up — teachers love it, then bring it to their school. Lead with the teacher, but make the org story prominent and credible so decision-makers see the platform play.

---

## 5. Sitemap & section-by-section content plan

**Recommended: a richer single landing page + a dedicated `/for-schools` page** (orgs need their own depth). Optional later: `/how-it-works`, `/pricing`, blog.

### Navigation
`Logo  ·  Features  ·  How it works  ·  For Schools  ·  Pricing  ·  Sign in  ·  [Get early access]`

### Homepage sections

**1. Hero**
- **Headline:** *The curriculum operating system.* (or *Lesson planning was the start. This is the whole system.*)
- **Sub:** *Plan a whole term, generate every resource, and let Curriculum OS learn from each lesson to shape the next. A teaching partner — not a flat plan.*
- **Primary CTA:** Get early access · **Secondary:** Watch the 90-sec demo (▶)
- Visual: product shot of the daily loop / a scheme-of-work board.

**2. The shift (problem → reframe)**
- *Most "AI planners" hand you a document and forget it. Curriculum OS remembers.*
- Short before/after using the From→To table above. This is where you separate from bobldobl-era tools.

**3. The daily loop (lead with the differentiator)**
- **Headline:** *Teach. Reflect. Tomorrow updates itself.*
- 3-step visual: ① Teach the lesson → ② Add a 30-second reflection / feedback → ③ Next day's plan returns with agreed actions & recommendations.
- Line: *Every lesson makes the next one better.*

**4. Plan the whole term**
- Scheme-of-work builder; drag-and-drop curriculum calendar; regressions & progressions on every lesson.

**5. Generate anything**
- Worksheets · videos · interactive lessons · full schemes — "from a prompt to a printable in minutes."

**6. Adapts to every learner**
- Learner RAG: preferences + teacher actions. Personalised planning without the spreadsheet.

**7. For Schools (org teaser → links to /for-schools)**
- *Your school's knowledge, in every plan.* Upload skills docs & standards; the AI plans against them. Automated learner reports. Optional attendance module. CTA: **Book a demo.**

**8. Why teachers love it** (carry/upgrade bobldobl's benefits: save planning time, lift lesson quality, stay organised, collaborate).

**9. Social proof / founder** (testimonials when available; keep the founder-led, "shape the platform" early-access energy).

**10. Pricing** (structure now, numbers later — see §6).

**11. FAQ** (What's different from a lesson planner? Is my data private? Can my school use it? What about the old bobldobl? Do I need to install anything?).

**12. Final CTA + footer** (reuse footer: Terms, Help, Cookies, Parental Guidance, Privacy, Accessibility, Contact, Socials).

### `/for-schools` page (org track)
Hero: *One curriculum. Every classroom. Consistent.* → Org RAG / knowledge base · embedded standards & skills docs · automated learner reports · attendance/registration module · admin & multi-teacher consistency · data & privacy · **Book a demo** CTA throughout.

---

## 6. CTA strategy

| Context | Primary CTA | Secondary |
|---|---|---|
| Teacher pages | **Get early access** | Watch demo |
| Schools page / org sections | **Book a demo** | Get early access |
| Sticky header | Get early access | — |

- Keep the **early-access incentive** from bobldobl (1 month early, founder training, user-testing seat) — it converts and you already have the model.
- One dominant action per screen; don't dilute with five competing buttons.

**Pricing:** hold specific numbers pre-launch, but show the *shape*: **Teacher** (individual, monthly/annual) vs **School** (per-seat or site licence, "Contact us / Book a demo"). Add a "founding member" price anchor if you want continuity with the £50 early offer.

---

## 7. Brand carry-over checklist
- ✅ Palette (navy/orange/amber/mint/pink/grey) and SK Modernist type
- ✅ Clean, modern, friendly tone
- 🔁 New name lockup: **Curriculum OS** (consider "C-OS" as shorthand mark)
- 🆕 New logo: book / layered-stack motif (later task)
- 🔁 Reposition all copy from "lesson planning tool" → "curriculum operating system / partner"

---

## 8. Open decisions for you (react, don't fill a form)
1. **Hero line** — go with *"The curriculum operating system"* (brand-forward) or *"Lesson planning was the start. This is the whole system."* (story-forward)?
2. **Name treatment** — "Curriculum OS" everywhere, or introduce "C-OS" as the short brand?
3. **Schools** — full `/for-schools` page now, or a homepage section until you have org customers?
4. **Pricing** — show "founding member" price, or fully hidden until launch?
5. **Demo video** — reuse the bobldobl explainer for now, or hold for a new C-OS one?

---

## 9. Next steps
1. You react to §8 + drop the repo into this folder.
2. I lock the final copy (exact headlines/body for every section).
3. Logo concepts for C-OS.
4. Build the site (reuse repo components) → GitHub → you open Netlify + Squarespace → push live.
