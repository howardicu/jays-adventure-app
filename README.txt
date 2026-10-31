Jay's Adventure App — prototype

What's included
- Biking, hiking and walking modes
- Map layer switch (OpenStreetMap terrain-style tiles / Esri satellite imagery)
- Browser GPS recording, speed, distance and elapsed time
- Save rides locally in the browser
- Animated route replay
- U.S.-only trail search by town, state, ZIP code, park or trailhead, with Mountain Bike, Hiking and Walking categories
- Named trail results with map pins and available route/difficulty tags, using OpenStreetMap Nominatim + Overpass
- Trail Photo Pins: take or choose a photo, capture current GPS coordinates, save it on this device, and show a camera pin on the map
- No built-in music integration; start any music app on the iPhone separately
- Local friend invite list (notes only; no invitations are sent)

Important limitations
This is an early web prototype, not a native iPhone/Apple Watch app.
- GPS and photo location require HTTPS and location permission. For best accuracy, take the photo at the spot you want to mark. The app gets a fresh GPS fix immediately after photo selection; the displayed accuracy is approximate.
- Photos and photo pins are stored locally in this browser on this device using IndexedDB. They are not uploaded or synced to the cloud. Deleting browser website data may delete them.
- Keep the app open while recording. Browser background GPS may pause or stop when the phone locks.
- Saved rides and friend notes are stored only on this device/browser.
- U.S. trail search is place-based: enter any U.S. location to search nearby mapped trails; it does not download every U.S. trail at once. Results depend on OpenStreetMap coverage and may omit unnamed trails.
- Trail results are mapped candidates, not verified open trails; difficulty, access, closures and current conditions may be missing. Confirm access and conditions with the land manager before riding or hiking.
- Music is played by the iPhone's own music app. Start playback there, then return to Jay's Adventure; the prototype does not control playback.
- Friend invitations, live group location, accounts, cloud sync, true offline maps, emergency services and Apple Watch integration are not implemented.
- Map/trail data needs internet access. Respect each provider's usage policies and attribution.

Test on iPhone
1. Host these files on an HTTPS static host.
2. Open the HTTPS address in Safari on iPhone.
3. Tap Share → Add to Home Screen.
4. Allow location and camera/photo access when prompted.
5. Use Take Photo while outdoors to save a GPS pin.

Trail Finder update: U.S. location searches now try multiple OpenStreetMap Overpass endpoints if the primary service is unavailable. Coverage and trail names depend on OpenStreetMap data.
