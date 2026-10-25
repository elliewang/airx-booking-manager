# AirX Control — Airline Booking & Operations Management

A responsive **static** airline-company administration portal with an integrated **rule-based staff chatbot**, built with vanilla HTML, CSS, and JavaScript. Deploy to GitHub Pages with no build steps, API keys, or backend.

## Features
- Airline staff dashboard with sample operational KPIs and recent reservations
- Reservation management: create, search, edit, cancel, filter by status
- Flight schedule with editable status (Scheduled, On Time, Boarding, Delayed, etc.)
- Passenger manifest showing lead passenger contacts and associated bookings
- Analytics for reservation statuses and illustrative seat utilization
- Chat assistant that summarizes flight schedules, delayed flights, booking totals, and finds AX booking references
- Browser `localStorage` persistence and a Reset demo data control
- Responsive navigation for desktop and mobile

## Live deployment on GitHub Pages

1. Create a GitHub repository, for example `airx-airline-ops`.
2. Upload **the contents of this directory** to the repository root. Make sure `index.html`, `styles.css`, and `app.js` are in the root (not nested inside another folder).
3. Go to **Settings → Pages → Build and deployment**.
4. Choose **Deploy from a branch**, select branch **main**, and folder **/(root)**, then click **Save**.
5. After deployment your site URL will be `https://YOUR_USERNAME.github.io/airx-airline-ops/`.

You can also open `index.html` locally. Everything works without a server; the Google Fonts import is optional and falls back to local fonts if offline.

## How to use

- Open **Reservations** to create, edit, cancel, and search demo reservations.
- Open **Flight Operations** and change a flight's status from the last table column.
- Open **Passengers** to view a simple manifest of non-cancelled lead passengers.
- Open the **Ask AirX AI** chat launcher. Try: `Show today's flights`, `Find booking AX1042`, `How many confirmed bookings?`, or `Show delayed flights`.
- Use **Reset demo data** in the sidebar to restore the initial sample dataset.

## Important demo limitations

This application is **not** connected to any real airline GDS, PSS, ticketing, payment, passenger identification, or operational data source. The chatbot is **rule-based** (not powered by an LLM), and all sample records and edits are stored in each visitor's own browser using `localStorage`. Data is not shared between devices or users and is not secure for real passenger information. All passenger names and emails are fictional. Do **not** enter real customer data. Flight capacity/booking figures are illustrative and independent of the small reservation sample list. Production airline management requires authentication, role-based access, server-side data storage, auditing, data security, and live airline integrations.

## Files

- `index.html` — portal layout, reservation form, chatbot UI
- `styles.css` — desktop/mobile styling
- `app.js` — sample data, CRUD operations, rendering, chatbot logic
- `.nojekyll` — GitHub Pages compatibility

## License
MIT (see `LICENSE`).
