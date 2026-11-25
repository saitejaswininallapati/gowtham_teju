# Gowtham & Tejaswini — Wedding Invitation

A single-page, mobile-first invitation in English and Telugu. This version includes the Wedding (Muhurtham) only. No build step: upload this folder as it is to any static host.

## What's in the folder

| Path | Purpose |
|---|---|
| `index.html` | The whole site (styles and scripts included) |
| `song.mp3` | Background music, starts when a guest taps "Open Invitation" |
| `images/` | Cover, first page, event slides, monogram, share preview and icons |
| `videos/` | Looping event clips for Mehendi, Haldi and Wedding, plus still frames |
| `calendar/` | "Add to calendar" files for iPhone (Android uses Google Calendar links) |

## Publish

Any of these work; all are free for a site this size.

- **Netlify Drop:** go to app.netlify.com/drop and drag this folder onto the page.
- **Vercel:** `npx vercel` inside this folder, or import it from GitHub.
- **GitHub Pages:** push the folder to a repository and enable Pages.

## Before sharing with guests

1. **Share preview (WhatsApp, iMessage):** in `index.html`, change
   `<meta property="og:image" content="images/og-image.jpg"/>` to the full address,
   for example `https://your-site.netlify.app/images/og-image.jpg`. Messaging apps only show the picture when the address is complete.
2. **RSVP:** responses go to the Google Apps Script address in `RSVP_URL` inside `index.html`. Send one test response and check it reaches the Google Sheet.
3. **Calendar end times** are estimates: Wedding until 12:00 PM. Edit `calendar/*.ics` and the `CAL` list in `index.html` to change them.

## Changing details

Event dates, venues and dress codes appear in the event cards (`#events`), the venue section (`#venue`), the event slides script, and the calendar files. The Telugu text sits next to the English in the same places.

## Media credits and licences

- Wedding (jeelakarra bellam) clip: from the reference invitation project, used with permission. The Wedding clip is slowed and played forward and back for a smooth loop.
- Decor photos in the Wedding slides: Pexels licence (free to use, no credit needed).
- Wedding slides 2 and 3 (hand-holding photo, couple portrait): from the original invitation, sharpened with Real-ESRGAN.
- Older artwork was sharpened with Real-ESRGAN.
