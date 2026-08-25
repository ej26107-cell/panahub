# PanaHub Website — local copy

## What's here
- `PanaHub Website.dc.html` — the whole site (all 14 sections, bilingual, Pana AI, membership flow)
- `support.js` — required runtime; the page will not render without it
- `image-slot.js` — the drag-and-drop image placeholders
- `uploads/` — the hero video

## How to open it
Keep all four items in the same folder structure, then open
`PanaHub Website.dc.html` in Chrome, Edge, or Safari.

Everything runs locally — no server, no install, no internet needed
(external links to organizer sites obviously need a connection).

## What this is and isn't
This is the complete front-end design. It is not yet a deployable
web application. Missing for production:

1. **URLs / routing** — the 14 pages are one file switching state.
   There is no /florida, /events, etc. The SEO plan needs those.
2. **Database** — all listings, events, scholarships and businesses
   are hardcoded arrays. Submission forms don't save anywhere.
3. **Accounts** — the Google/Microsoft sign-in buttons are visual.
   No auth, no sessions, no saved favorites, no newsletter delivery.
4. **Pana AI** — keyword matching over the hardcoded data. Real AI
   needs a server-side API key (never in frontend code).

## For a developer
Hand them this file as the specification. Every screen, state, flow,
and both languages of copy are in it. The target stack from the
original brief: Next.js + Supabase (Postgres + Auth) on Vercel.
The data arrays near the bottom of the file map directly onto the
database tables that brief describes.
