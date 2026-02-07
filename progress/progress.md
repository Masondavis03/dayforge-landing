# DayForge Landing Page - Progress

## Project
- **Repo:** [Masondavis03/dayforge-landing](https://github.com/Masondavis03/dayforge-landing)
- **Live URL:** [dayforge.org](https://dayforge.org)
- **Stack:** Static HTML/CSS/JS, Supabase (waitlist), Vercel (hosting), Cloudflare (DNS)

---

## Completed

### Phase 1 - Initial Landing Page (2026-02-05)
- Single-file static site (`index.html`) with dark theme
- Hero section: "Your day, forged by AI."
- 3 feature cards: Voice-First Scheduling, Document-Aware, Private by Design
- Email waitlist form connected to Supabase `waitlist` table
- Deployed to Vercel with custom domain `dayforge.org` via Cloudflare DNS

### Phase 2 - Full Redesign (2026-02-05)
- **Typography:** Sora (headings) + Lexend (body) replacing Outfit + DM Sans
- **Particle system:** Interactive canvas with mouse-reactive particles and connection lines
- **Grain overlay:** Subtle noise texture for depth
- **Nav:** Scroll-aware navbar with blur backdrop, nav links (Features, How It Works), CTA button
- **Hero (redesigned):**
  - Two-column layout: text left, calendar mockup right
  - Animated calendar with February 2026 grid, color-coded events (Team Standup, Deep Work Block, Project Review)
  - Floating badges: "AI Scheduling", voice waveform "Listening...", "Smart Conflict Detection"
  - 3D perspective tilt on calendar with hover flatten
- **How It Works section (new):**
  - 3-step flow: Speak or Drop > AI Forges Your Day > Live Your Day
  - Numbered step circles with connecting line, scroll reveal animations
- **Features section (expanded):**
  - 5 cards in 2-column grid with 1 full-width "Voice-First Scheduling" card featuring animated waveform visualizer
  - New cards: Smart Rescheduling, Campus Ready (Canvas LMS sync)
  - Radial gradient hover effects on cards
- **Waitlist section (redesigned):**
  - Unified input + button inside a single bordered container with focus glow
  - Trust signals: "No spam, ever", "Early access priority", "Free at launch"
  - Supabase integration: POST to `/rest/v1/waitlist`, handles 201/409/errors with try/catch
- **Footer:** Two-column with copyright left, Privacy/Terms/Contact links right
- **Animations:** Scroll reveal (IntersectionObserver), hero fade-in sequence, floating elements, waveform bars, shimmer on logo
- **Responsive:** Breakpoints at 900px and 500px for tablet/mobile

### Phase 3 - Premium Editorial Redesign (2026-02-07)
- **Inspiration:** LION Specialty (lionspecialty.com) — cinematic, editorial, scroll-driven storytelling
- **Typography:** Instrument Serif (display/headings) + General Sans (body) — premium editorial pairing
- **Layout:** Narrative flow: Hero → Problem → Solution → Demo → Stats → Features → Waitlist
- **Hero (redesigned):**
  - Centered layout with massive serif headline "Your day, forged by AI."
  - Italic gradient accent on "forged"
  - Dual CTA: "Join the Waitlist" + "Try It Live"
  - Animated scroll indicator at bottom
- **Problem section (new):**
  - 6 numbered pain points in 3-column border grid (LION-style)
  - Large serif problem numbers (01–06) with accent opacity
  - Subtle gradient hover on each cell
  - Topics: manual scheduling, context-blind, documents siloed, privacy, rigidity, students forgotten
- **Solution statement (new):**
  - Full-width centered "That's why we built DayForge." with gradient italic
- **Interactive Demo section (new):**
  - Split panel: voice command buttons (left) + calendar timeline view (right)
  - 4 demo scenarios: schedule standup, block deep work, import deadlines, reschedule afternoon
  - Animated event cards slide into timeline slots on click
  - Live "DayForge: Done." voice response bar with pulsing indicator
  - macOS-style window dots (red/yellow/green)
- **Stats section (new):**
  - 4 big metrics: 3×, 100%, Zero, 24/7
  - Gradient serif text, bordered top/bottom
- **Features (redesigned):**
  - Two-column: sticky description left + accordion right
  - 5 accordion items with rotating +/× icon
  - Voice-First, Document-Aware, Private by Design, Smart Rescheduling, Canvas LMS
- **Waitlist (redesigned):**
  - Radial glow background effect
  - Serif headline "Be the first to forge your day."
  - Supabase integration with 201/409/error handling
- **Meta/SEO:** OG tags, Twitter card, favicon (⚡ emoji SVG)
- **Particles:** Refined — 60 max count, connecting lines at 130px, mouse repulsion
- **Film grain:** SVG noise overlay at 2.5% opacity

---

## Infrastructure
| Component | Service | Details |
|-----------|---------|---------|
| Hosting | Vercel | Auto-deploy from GitHub `master` branch |
| DNS | Cloudflare | Custom domain `dayforge.org` |
| Waitlist DB | Supabase | Project `wkycsdqejmhswlpzxmez`, table `waitlist` |
| Source | GitHub | `Masondavis03/dayforge-landing` |

---

## TODO / Next Steps
- [ ] Wire Supabase anon key (replace `YOUR_ANON_KEY_HERE` placeholder)
- [ ] Privacy Policy and Terms of Service pages
- [ ] Analytics (Vercel Analytics or Plausible)
- [ ] A/B test hero copy and CTA variations
- [ ] Add waitlist count display ("Join 500+ others")
- [ ] Mobile hamburger menu for nav links
- [ ] Performance audit (Lighthouse)
- [ ] OG image for social sharing previews
