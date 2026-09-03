# Canadian Waters — Safari Prototype (v2)

Open `index.html` in a web browser. For iPhone testing, upload this folder to
any static web host and open its HTTPS address in Safari.

What's new in this version:
- A real lake map (irregular shoreline, two islands, marked fishing hotspots)
  that you drive a boat around using the on-screen stick (or drag on desktop).
- Live casting: tap CAST, then drag anywhere on the water to aim — direction
  and drag distance set the cast's angle and power. Release to cast.
- A visible lure lands with a splash and ripples while you wait for a strike.
- When a fish bites you get a short window to tap SET THE HOOK before it
  gets away.
- The fight is now shown on screen: the fish itself swims near the lure,
  darting and jumping as you alternate REEL IN and LET IT RUN, and visibly
  gets pulled toward the boat as its stamina drops.
- Fishing hotspots (weed edge, rocky point, drop-off, sunken timber) bias
  which species bites and how fast, and are flagged when you drive near them.
- A third species, Walleye, joins Smallmouth Bass and Northern Pike.

Gameplay loop:
1. Drive the boat with the stick — look for a flagged hotspot.
2. Choose a lure.
3. Tap CAST, then drag to aim and release.
4. Watch the lure; when it strikes, tap SET THE HOOK in time.
5. Alternate REEL IN and LET IT RUN to land the fish.
6. Cast again or go back to driving. Build your Trophy Book.

The prototype is still intentionally self-contained: no server, account, or
external libraries are required — everything (including the lake map) is
generated in-browser on load.

Known limits / good next steps for further refinement:
- Boat currently can't run aground into the two islands in a "fun" way (it
  just stops) — could add a bump/damage sound or slow drift instead.
- Only one lake is generated; a level-select or "drive to a new lake" trip
  system would extend replay value.
- No persistence yet — money/XP/trophies reset on page reload.
- Weather/time-of-day currently only display a clock; could actually affect
  bite rates.
