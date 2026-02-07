# DayForge Landing Page

Landing page for [dayforge.org](https://dayforge.org) — an AI-powered calendar app launching Summer 2026.

## Design

Premium editorial aesthetic inspired by high-end agency sites. Scroll-driven storytelling with interactive demo, animated particles, and cinematic typography.

**Typography:** Instrument Serif + General Sans  
**Theme:** Dark (#08081a) with indigo accent (#6366f1)

## Stack

- Static HTML/CSS/JS (single file, no build tools)
- [Supabase](https://supabase.com) for waitlist email capture
- [Vercel](https://vercel.com) for hosting
- [Cloudflare](https://cloudflare.com) for DNS

## Development

Open `index.html` in a browser. No build step required.

## Deployment

Deployed via Vercel with custom domain `dayforge.org` managed through Cloudflare DNS.

### Setup

1. Replace `YOUR_ANON_KEY_HERE` in `index.html` with your Supabase anon key
2. Push to GitHub
3. Vercel auto-deploys from `master`

## Waitlist

Emails are stored in Supabase (`waitlist` table). The form handles:
- **201** → Success message
- **409** → Already registered
- **Error** → Retry prompt
