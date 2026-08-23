# FROCKARA v2

Floral Indian frock commerce SPA with multi-page methodology.

## Core flows
- `/` homepage
- `/shop` collection
- `/product/<slug>` dedicated product page for every item
- `/themes` theme discovery
- `/sleeve-studio` sleeve-first discovery
- `/concierge` personal edit
- `/wishlist` saved pieces
- `/journal` editorial hub
- `/story` brand story + session panel

## Account + sessions
Google-ready sign-in modal. Current file includes a demo account adapter. Production must use Google Identity Services + backend token verification. Session events are recorded client-side in localStorage for prototype continuity.

## WhatsApp ordering
Product and cart actions create an order summary and open WhatsApp to `+91 83175 81308`. The message includes the order ID, product(s), size, quantity, total and payment/order instructions. Payment should be handled by an authenticated backend/PSP process; the SPA does not auto-transfer money.

## Order documents
Users can generate a downloadable text order summary. Production should generate a signed PDF/order document server-side and attach a secure order URL in WhatsApp.

## Production integrations
Replace demo Google account, analytics IDs, example canonical URL, demo assets, and front-end session storage with real auth, CRM/session service, inventory, order service, payment/UPI gateway, delivery, email/SMS/WhatsApp Business API, and server-generated documents.
