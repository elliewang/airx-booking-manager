# AirX — Static Airline Booking Management + Chatbot

A polished, fully static airline reservation management portfolio demo, designed for **GitHub Pages**.

## Features
- Responsive AirX homepage and live booking dashboard
- Search illustrative flight options by route, departure date, cabin and travelers
- Create demo reservations with confirmation codes
- List, search, edit, inspect and cancel demo reservations
- Browser-side travel assistant: search flights in plain English, jump to reservations, and explain booking changes
- LocalStorage persistence (per browser/device)

## Deploy to GitHub Pages
1. Create a new GitHub repository (for example `airx-booking-manager`).
2. Upload **index.html**, **styles.css**, **app.js**, **README.md**, and **.nojekyll** to the root of the repository (not inside another folder).
3. In GitHub, open **Settings → Pages**.
4. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, and Save.
5. Visit `https://YOUR_USERNAME.github.io/airx-booking-manager/` after deployment.

You can also open `index.html` locally by double-clicking it. No build, Node.js, Render, API keys or dependencies are required.

## Testing the site
1. Open Explore Flights; choose route and date; click Search flights.
2. Book a sample flight, entering a lead passenger name and email.
3. Go to My Bookings to see confirmation, edit details, change date, and cancel.
4. Click **Load sample bookings** to test management tools without booking first.
5. Open the chatbot and ask: `Find flights from Pittsburgh to Chicago tomorrow`, `Show my bookings`, `How do I change a booking?`

## Important limitations
This is a **demo**, not a real travel agency. All fares and flights are simulated. Reservations stay in the visitor's browser using localStorage, may be cleared by the visitor or browser, and do not synchronize between devices. The chatbot is a local keyword/rule-based assistant, **not** a connected LLM. Do not enter real personal/payment data. No payments, real inventory, authentication, email confirmation or airline ticket issuance are included.

## File structure
```
index.html     Main page and booking/chatbot UI
styles.css     Responsive website styling
app.js         Flights, bookings, local storage, chatbot behavior
.nojekyll      GitHub Pages compatibility
README.md      Instructions
```

## Upgrade path
For production: authenticated users, secure server-side booking database, airline inventory API integration, payment service, conversational model hosted on a secure backend, monitoring and audit logs.
