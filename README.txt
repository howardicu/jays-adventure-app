# Jay's Adventure App — prototype

## What's included
- Biking, hiking and walking modes
- Map layer switch (OpenStreetMap terrain-style tiles / Esri satellite imagery)
- Browser GPS recording, speed, distance and elapsed time
- Save rides locally in the browser
- Animated route replay
- Trail/path discovery search using OpenStreetMap Nominatim + Overpass
- Quick links to Spotify, Apple Music, Amazon Music, YouTube Music and Pandora
- Local friend invite list (notes only; no invitations are sent)

## Important limitations
This is an early web prototype, not a native iPhone/Apple Watch app.
- GPS requires HTTPS and permission; keep the page open while recording.
- Browser background GPS may pause or stop when the phone locks.
- Saved rides and friend notes are stored only on this device/browser.
- Trail search results are mapped path candidates, not verified open trails; difficulty, access and closures may be missing.
- Music buttons open each service; they do not provide embedded playback or subscription control.
- Friend invitations, live group location, accounts, cloud sync, true offline maps, emergency services and Apple Watch integration are not implemented.
- Map/trail data needs internet access. Respect each provider's usage policies and attribution.

## Test on iPhone
1. Host this folder on an HTTPS static host (for example, a private test deployment).
2. Open the HTTPS address in Safari on iPhone.
3. Tap Share → Add to Home Screen.
4. Allow location access when prompted.
5. Try the map and GPS recording outdoors in a safe area.

The app icon and manifest are included. A service worker is included for basic caching, but external map tiles and trail search still need a connection.


SPOTIFY PREMIUM PANEL
A Spotify Premium panel has been added to the live Explore screen with a connect button,
track display area, and previous/play-pause/next controls. These are currently prototype UI
controls only. They do not authenticate or control Spotify yet. A Spotify Developer app,
OAuth authorization (preferably Authorization Code with PKCE), approved redirect URI, and
a secure HTTPS-hosted deployment are required for a real integration. Never enter a Spotify
password into this prototype; sign-in must happen on Spotify's own authorization page.
