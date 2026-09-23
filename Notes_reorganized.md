## IBC Business App — Event Finder (Organized Notes)

### Project Overview
- Working title: IBC Business app (Event Finder)
- Purpose: help users discover local events and business promotions; enable businesses to post and promote events; allow ticket purchases via trusted third‑party providers or SDKs
- Platforms: iOS, Android, Web
- Target milestone: [end of 28th — confirm exact date]

### Users & Roles
- Attendee: browse, save/bookmark, RSVP, purchase tickets, view personal activity
- Business: create/manage events, view analytics, purchase subscriptions/promotions
- Admin / Moderator: approve listings, handle reports/refunds, manage content
- Guest (optional): browse public events without account

### Core MVP Features
- Event discovery: list view and map view
- Filters & search: tags, date, location radius, price, categories (parties, free activities, date ideas)
- Event detail page: title, description, images, date/time, address (with map link or embedded map), tags, organizer
- Accounts: attendee and business sign-up/login; admin/moderation accounts
- Create event: business / user can post an event (with optional moderation queue)
- Promote listing: one‑time purchase to feature/announce an event

### Ticketing & Payments
- Third‑party checkout recommended for ticket purchases (open in SFSafariViewController / Chrome Custom Tabs) and verify via provider API/webhook
- Option to integrate provider SDK/API (Eventbrite, Stripe, etc.) for tighter UX (medium effort)
- Avoid full card collection inside WebView for security/compliance unless using provider-recommended flows
- Payment providers to evaluate: Stripe, Square, Eventbrite, Ticketmaster

### Business Tools & Monetization
- Free basic postings for businesses
- Paid subscriptions for analytics and posting limits / premium features
- One‑time promoted/featured listing purchases
- Optional platform fee on ticket sales (decide revenue share)

### Social & Engagement Features
- Save/bookmark events, follow favorite businesses
- Activity feed / "For you" personalization
- Optional public chat or comments (moderation required)
- Share to social networks

### Extras / Gamification (optional)
- Local deals menu (e.g., "Rexburg deals")
- Simple mini-games (e.g., campus-themed Wordle) to boost engagement
- Seed parties or community events program

### Integrations & Tech Decisions (open)
- Mobile stack: [React Native / Flutter / Native iOS+Android] — choose
- Backend: [Firebase / Node + Postgres / Other] — choose
- Map provider: [Google Maps / Mapbox / Other] — choose
- Ticket/payment provider: [Stripe / Square / Eventbrite / Ticketmaster / Other] — choose

### Design & Assets
- Images and presentation assets needed for event pages and app store
- App theming: [no theming planned — confirm if needed]

### Legal, Compliance & App Store Notes
- Write Privacy Policy & Terms of Service
- Define refund policy for tickets and promoted posts
- App Store rules: ticketing for real‑world events generally allowed via external payments, but verify IAP requirements for any digital goods
- App store listing fee / notes: [$125 mentioned — clarify what this refers to]

### Analytics & Metrics to Track
- Events posted, events published, event views, RSVPs, ticket conversions, MAU, ARPU, business subscription churn

### Roadmap & Next Steps (prioritized)
1. Confirm tech stack + core providers (maps, payments, ticketing).
2. Define business subscription tiers and pricing.
3. Write 6–8 user stories for Attendee, Business, Admin.
4. Sketch 4 core screens: Home/List, Map, Event page, Create Event.
5. Implement minimal backend: auth, events CRUD, geo-search, purchase verification webhook.
6. Build mobile UI for browsing + create event flow.
7. Launch closed beta; collect feedback; iterate.

### Pricing & App Store
- Clarify the meaning of the noted "$125 for app in store" and any other costs (developer accounts, fees)

### Open Questions / Missing Decisions
- Exact launch date and milestones: [fill in]
- Chosen payment/ticket provider: [fill in]
- Mobile framework and backend choice: [fill in]
- Business subscription tiers, pricing, and revenue share: [fill in]
- Moderation workflow and SLA for approvals/reports: [fill in]
- Ticket display format: QR code, Wallet pass, or other: [fill in]
- Push notification strategy for reminders/promotions: [fill in]

### Notes / Misc
- Use clear terminology: "announce" vs "promote" vs "feature" for paid options
- Consider web-first pages for events to allow quick updates, then implement native views for better UX

---

