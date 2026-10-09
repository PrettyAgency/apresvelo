# Design brief — Après Vélo "Tasmania recovery" release
Two page templates for apresvelo.com (Shopify). Agency: prepared September 2026.

## The client
Après Vélo — premium Australian guided cycling tour operator (with a legacy cycling-apparel line). Tours are 5–7 days, A$2,995–$12,000, ~12–15 riders per departure, led by ride captain **Beardy McBeard** (Marcus Enno), one of cycling's best-known photographers. Tone: knowledgeable, warm, a little wry — "ride hard, then the après begins." Never corporate, never bro-y.

## Audience
Australian road/gravel cyclists, roughly 45–65, affluent, researching a considered ~$3k+ purchase over weeks. Many browse on iPad/mobile. Trust signals matter: real reviews, real photography, a phone number, clear prices and dates.

## The job (both pages)
Primary conversion: a **tour enquiry/booking request** via ONE form per page (segmented toggle: "I'm ready to book" / "I have questions"). Secondary: brochure download ($200-off offer). No newsletter prominence. Every form completion redirects to a thank-you page (fires analytics events — keep the flow, don't design inline "success" states for the live build).

## Design system
- **Palette:** bone `#f2efe8` (background), slate `#181c1e`, eucalypt green `#1f3d33`, dolerite grey `#5c6670`, brand red `#cf0a2c` — red is for CTAs and small accents ONLY. Card surface `#faf8f3`, hairline `#ddd8cc`.
- **Type:** Fraunces (display, weights 400–600) + Archivo (body/UI). Sentence case headings. No all-caps eyebrow labels.
- **Photography-led.** Beardy McBeard's imagery is the brand's unfair advantage — big, full-bleed, minimal overlay. All prices, dates, stats and buttons must be REAL TEXT, never text baked into images (the current site does this; it's an SEO and accessibility fault we're fixing).
- **Signature element:** an SVG ride elevation profile accompanying itineraries — cyclists read elevation like a language.
- Interactions: itinerary day accordion, FAQ accordion, sticky booking bar (appears after the hero: tour name, dates, from-price, rider limit, CTA). Motion minimal — accordions and the sticky bar only.
- Responsive to mobile; visible focus states; WCAG-friendly contrast on the bone background.

---

## TEMPLATE 1 — Tasmania hub page (the page that must RANK)
URL: /pages/tasmania-cycling-tours · This page targets: "tasmania cycling tours", "tasmanian cycling tours", "cycling tours tasmania", "bike tours tasmania", "cycling holidays tasmania".
H1: **Tasmania cycling tours**. Title tag: "Tasmania Cycling Tours 2026–27 | Road & Gravel | Après Vélo".

Section order:
1. **Hero** — full-bleed Tassie landscape, H1 + one-line promise, CTA "Find your tour" (anchor to tour cards).
2. **Tour cards (the answer, up top)** — all 5 Tasmania tours as rich cards: name, dates, days, difficulty (x/5), from-price, road/gravel tag, one-line character ("the purist's week", "gravel coast to coast"…), link to tour page. This section answers "which one is right for me?"
3. **Comparison strip** — small table: tour × days × difficulty × surface × price × next departure.
4. **Why Tasmania / why Après Vélo** — 300–400 words of genuine destination copy (Wellington, East Coast, Central Highlands gravel, spring/autumn seasons) + Beardy as local. Supports 800–1,200 total words on-page.
5. **Guest reviews** — pooled from all Tassie tours, 4–6 quotes with star treatment.
6. **Destination FAQs** (accordion, FAQPage schema): best time of year, road vs gravel choice, fitness needed, bike hire, non-riding partners, getting to Hobart/Launceston.
7. **Gallery strip** — 4–6 images.
8. **Enquiry section** — single form (toggle) + brochure offer + phone.
9. Footer cross-links: Gravel tours hub, all tours.

## TEMPLATE 2 — Tour pillar page (the page that CONVERTS)
Reference prototype supplied (Tour de Tasmania). This template repeats for all ~13 tours.
Targets the TOUR NAME + long-tail only (e.g. "tour de tasmania", "hobart cycling tour", "mt wellington cycling tour"). **Do NOT use "Tasmanian cycling tours" in this page's title/H1** — that term belongs to the hub; it appears here only as the breadcrumb/link anchor pointing at the hub.
Title shape: "Tour de Tasmania | 5-Day Hobart Cycling Tour | Après Vélo".

Section order:
1. Breadcrumb ("Tasmania cycling tours / Tour de Tasmania") · full-bleed hero · H1 tour name · one-paragraph lede · CTAs (Request a booking / See the five days).
2. **Facts strip** (eucalypt band): days, km, climbing m, difficulty, departure dates, from-price — real text.
3. Sticky in-page section nav: Overview · Itinerary · What's included · Ride captain · Reviews · FAQs · Gallery.
4. **Overview** — 2–3 paragraphs, ride + après balance, one supporting image.
5. **Itinerary** — elevation profile SVG + day-by-day accordion (day, title, km/elevation chips, 2–3 sentence description).
6. **What's included / not included** — two honest columns + non-riding-partner note (15% off, support-vehicle seats).
7. **Ride captain** — dark slate band, Beardy bio + photo.
8. **Guest reviews** — 3+ quotes specific to this tour (Review schema).
9. **FAQs** — 6–8 tour-specific questions on-page (FAQPage schema). These absorb the old /pages/faq/* sub-pages.
10. **Gallery** — 4 images.
11. **Enquiry section** (eucalypt band) — single toggle form, brochure offer, gift voucher link, phone number. Microcopy: "No payment now. One follow-up from a human, no spam."
12. **Other Tasmania tours** — 3 cross-link cards (exact-anchor link back to hub included).

## Content per tour (Tour de Tasmania values for the reference build)
5 days · Hobart to Hobart · 378 km · 7,600 m climbing · difficulty 4/5 · 26–31 Oct 2026 · from A$2,995 twin share. Days: (1) Cruisy Hobart roll-out 35km/720m + welcome dinner; (2) Cygnet challenge 125km/2,000m gravel coast road; (3) Pipeline Track 88km/1,800m, MONA afternoon, dinner included; (4) Mt Wellington loop 50km/1,313m — 17.7km at 7%; (5) Vineyard ride 80km/1,800m, Strade-Bianche-style white gravel finale, farewell long lunch; (6) transfers out.

## Hard constraints (SEO recovery — do not trade away in design)
- FAQs, reviews and gallery live ON these pages, not on separate URLs.
- One form per page. Book Now is a page CTA, not a nav destination.
- All copy as real HTML text; images carry no informational text.
- Mega-menu context: site nav is being collapsed to ~14 links; these templates must not depend on deep menu links to sub-pages.
- Internal links: tour pages link UP to the hub with anchor "Tasmania cycling tours"; hub links DOWN once to each tour.

## Out of scope
Checkout/payment, the fashion store, blog templates, the actual Wufoo/forms replacement (form is designed here, wired by dev).
