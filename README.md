# Rahul weds Priyanka — wedding website

A single-page Madhubani (Kachni line-art) wedding website. It needs no server, database or coding to run.

```
index.html              ← the whole website
assets/invitation.mp4   ← the invitation film
assets/itinerary-card.jpg
assets/music.mp3        ← background music (plays after "Open the invitation")
assets/og-cover.jpg     ← picture shown when the link is shared on WhatsApp
assets/video-poster.jpg
fonts/                  ← Hindi and English fonts
```

## 1. Fill in your details (2 minutes)

Open `index.html` in any text editor (on a phone, the GitHub website's editor works too) and find the **SETTINGS** block near the top:

| Setting | What to put |
|---|---|
| `rsvpNumber` | The WhatsApp number that should receive RSVPs: country code and number, digits only, e.g. `919876543210` |
| `contacts` | Names and phone numbers to show under the RSVP form. Leave the `X`s and that contact stays hidden |
| `maps` | Where the "Directions" / "Navigate" buttons lead (home: the Shiv Mandir on Road No. 14A as a landmark, with a note that the house is just behind it; reception: Madhuram Marriage Hall) |
| `mapEmbed` | The embedded maps (already set). To change: Google Maps → **Share** → **Embed a map** → copy only the `src="..."` link |
| `photos` | Optional. Upload photos into `assets/photos/` and list them, e.g. `["assets/photos/1.jpg", "assets/photos/2.jpg"]` |

## 2. Put it online (free)

### Option A — GitHub Pages
1. Sign in at github.com → **New repository** → name it e.g. `rahul-weds-priyanka` → **Public** → Create.
2. **Add file → Upload files** → drag in *everything inside this folder* (index.html, assets, fonts, README.md) → **Commit changes**.
3. **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → **Save**.
4. After a minute your site is live at `https://YOUR-USERNAME.github.io/rahul-weds-priyanka/`.

### Option B — Netlify Drop (quickest, no account needed to try)
Go to **app.netlify.com/drop** and drag this whole folder onto the page. You get a link instantly; create a free account to keep it and rename it (e.g. `rahul-weds-priyanka.netlify.app`).

### Optional — your own address
A domain like `rahulwedspriyanka.in` costs a few hundred rupees a year and can be pointed at either option above.

## 3. Make the WhatsApp preview appear

Once you have the final address, open `index.html` and replace both `YOUR-SITE-ADDRESS` lines near the top, e.g.

```
https://YOUR-USERNAME.github.io/rahul-weds-priyanka/assets/og-cover.jpg
https://YOUR-USERNAME.github.io/rahul-weds-priyanka/
```

Then the link shows the Madhubani "Rahul & Priyanka" banner in WhatsApp chats.

## Notes
- **Music:** "Roslyn" (Rishab Rikhiram Sharma) is a copyrighted song. Private sharing is usually fine, but on a public repository GitHub can remove it after a copyright complaint. To be safe, swap `assets/music.mp3` for a royalty-free track (same filename) or delete it; the page works without it.
- **Countdown:** counts to the wedding day (25 Nov, 2:00 PM IST), then automatically to the next event. Finished events get a "सम्पन्न · DONE" stamp.
- **Calendar:** each event has "Add to calendar" (Google); the red button downloads all five events with reminders for any phone calendar.
