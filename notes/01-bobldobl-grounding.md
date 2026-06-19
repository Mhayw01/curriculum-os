# Grounding: What bobldobl is today

*Phase 1 only — a factual capture of what currently exists. No C-OS planning or recommendations here. For alignment before we move on.*

Sources reviewed in full: the live site (both pages), the explainer video, the Google Drive brand guide + logo/type/favicon assets, and the "Education App" Figma file. (Repo not yet accessible — see end.)

---

## 1. The website (bobldobl.com)

Two pages, both client-rendered React.

**Home (`/`)**
- Hero: **"Revolutionise your lesson planning with AI"** on a cyan gradient, with the bobl dobl logo top-left and an orange **Sign Up Now** button.
- Three pillars: *Search & filter to find lessons · Design your own resources · Share & manage your curriculum.*
- An embedded explainer video (see §2).
- Feature grid: Find lessons instantly · Edit & Customize with AI · Schedule & Manage your Curriculum · Share & Collaborate · Create lessons from Scratch.
- Benefits ("Why Educators Love this App"): Minimise planning time · Maximise lesson quality · Collaborate & Share · Stay Organised.
- Footer: Terms, Help, Cookies, Parental Guidance, Privacy, Accessibility, Contact, socials.
- Single repeated CTA throughout: **Sign Up Now** → `/early-access`.

**Early access (`/early-access`)** — the conversion/offer page
- Headline: **"Pay £50 now & your Summer is FREE"**, "Save £130 – Early Access Offer".
- Emotional hooks: *"No more Sunday night stress. No more planning through July & August."*
- What you get: search thousands of editable lessons; customise with AI; schedule & share curriculum; full access EARLY; BETA access to future tools; 1-to-1 onboarding with the Founder; training & walkthroughs.
- Commercials: **£50 one-time = one year** (no recurring), early access from May 4th (1 month before public launch), offer deadline-driven.
- Framing: "We're a small team of educators, not a big tech company… helping us build more content and improve the AI tools."
- FAQ + final CTA "Get Access Now – £50 for the Year" → checkout.

**Takeaway:** the site sells one job — *find/edit/schedule/share individual lessons* — with a founder-led, anti-burnout, early-access offer. It's a single-product, lesson-level story.

---

## 2. The explainer video

Self-hosted MP4, animated, caption-driven (no voiceover). Narrative arc:
brand intro → **"Instant content at your fingertips"** (lesson search/filter UI) → **"Use AI to adapt content to your needs"** (slide editor; a Division maths lesson) → **"Less Planning"** → **"More Teaching"** → **"More Impact"** → **"Sign up Today — Teach smarter!"** (dashboard of recent lessons).

Notable: the big emotional statements ("Less Planning", "More Teaching", "Instant content…") are set in an **editorial serif** display face — a deliberate contrast to the geometric sans used elsewhere.

---

## 3. Brand

There are effectively **two layers** of brand, and they don't fully match — worth deciding which is canonical for C-OS.

**(a) The 2022 Google Drive "Brand Logo Guide" (18 pp)** — the documented system
- **Logo:** a monogram fusing **b + d** into one icon, bounded by a **circle** ("synergy between brand and audience; reach/global engagement"). Variants: main lockup, wordmark, icon; coloured + white. SVG/PNG provided. Favicon + letterhead assets exist.
- **Palette (documented):** navy `#093A5A`, orange `#FA602F`, amber `#D37F0F`, mint/teal `#B8DED5`, pink `#E9496C`, grey `#EFEFEF`. Section pages are navy with translucent overlapping circles.
- **Type:** SK Modernist (geometric sans), bold for display; "modernism and simplicity". Font files (incl. SK Modernist Mono) provided.

**(b) The live brand (site + Figma) — what's actually shipping now**
- **Logo:** same b+d-in-a-circle monogram, rendered in **violet/purple**, with lowercase two-line **"bobl dobl"** wordmark in near-black. White version on dark/purple.
- **Primary colour: violet/purple `#5740f1`** (site theme colour) — used for hero gradients, primary app sections, filter pills, accent bars. This is the dominant brand colour now.
- **Secondary: cyan/teal gradient** (hero backgrounds, app headers).
- **Accent / CTA: orange** (Sign Up Now, Launch Lesson, Start Demo buttons).
- **Neutrals:** white cards, light grey, near-black text.
- **Type:** SK Modernist sans for UI/headlines + an **editorial serif** for emotional display lines (from the video).
- **Illustration:** flat, friendly, diverse vector characters with tablets/devices.
- **Tone of voice:** warm, energetic, teacher-empathetic, founder-led.

**Net:** the brand evolved from the navy-led 2022 guide to a **purple + cyan + orange** system in practice. The monogram-in-circle and SK Modernist carried over; the navy did not.

---

## 4. The product (Figma "Education App")

Far richer than the marketing site. Two Figma pages of desktop + mobile frames, plus a userflow/sitemap diagram. Screens/flows observed:

- **Dashboard with a weekly Timetable** (Monday…, drag-and-drop), "Share timetable", "Timetable options".
- **Discover** lessons + **Discover Results** page, with subject filter pills: **Literature, Maths, Biology, Art**.
- **Lesson cards** with ratings, year levels, durations.
- **Launch Lesson** and **Design Lesson** (AI slide editor — e.g. a Division/remainders lesson with teacher notes and lesson goals).
- **Start Demo** onboarding / empty states.
- **Sign Up / Sign In** screens.
- Many **mobile** versions of the above.
- In-progress **design annotations** (e.g. "Add teacher/bobldobl lessons, maybe none in results") — the product is still actively being iterated.

**Takeaway:** the built product already does lesson discovery, AI lesson/slide design, and timetable scheduling, across web + mobile.

---

## 5. Stack / hosting (stated, not yet verified)

- Repo: `Mhayw01/bobldobl-landing-page` (GitHub, private). **Not yet accessible** — my sandbox can only see the empty "Curriculum OS" folder. Drop the repo into that folder and I'll confirm the framework and reusable components.
- Hosting plan: **GitHub → Netlify**, DNS on **Squarespace**.

---

## 6. Open questions to confirm before we plan C-OS
1. For C-OS branding, is the **live purple/cyan/orange** system canonical (and the 2022 navy guide is superseded), or do you want to pull anything back from the navy guide?
2. Is the editorial **serif** for emotional headlines something to keep as part of the brand?
3. Anything in the current product (Figma) that's being dropped or is out of scope for C-OS?
4. Is `bobldobl-landing-page` the only repo, or is there a separate app repo?

*Nothing about C-OS positioning, messaging, sections, or CTAs is decided yet — that's the next step, once you're happy this captures what exists.*
