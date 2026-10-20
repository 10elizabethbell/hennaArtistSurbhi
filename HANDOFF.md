# Henna Artist Surbhi — handoff at ~60%

**Live:** https://10elizabethbell.github.io/hennaArtistSurbhi/ · **Repo:** https://github.com/10elizabethbell/hennaArtistSurbhi · **Built:** 2026-10-20 from Muse brief of 2026-10-20 (thin brief: one Karwachauth open-house post)

On the Call Sheet: yes (the script had to add a new entry, so Muse hadn't listed this prospect yet).

## What's built
- One page, calm band style. Bands: green hero → paper open house → deep-green booking form → paper close → deep-green footer.
- Palette (no logo exists, so it comes from the trade and her photo): henna-leaf green `#1f4d3c` in the "navy" role, deep green `#123227`, sage-tinted paper `#f3f5f1`, Karwachauth gold `#e6b04a` as the one fill accent (`#7e5410` when it has to be text on light). Green on purpose, so it can't be mistaken for Royal Henna by Neha (wine/rani/serif).
- Header: "Surbhi / Henna artist" wordmark, tap-to-call (908) 274-4044 top right.
- Hero: eyebrow "Karwachauth open house · Oct 26–28", H1 "Henna for your special day in North Brunswick" with the letter bounce-in, promise line, two buttons (Book your slot → form, Text Surbhi → `sms:`). Her one photo sits in the hero as a 3:4 card (under the buttons on phones, right column on desktop) with "Click to see more of my work." → Instagram right under it.
- Open house band: her post's facts word for word (26–28 Oct 2026, 10 AM – 4 PM, North Brunswick, "Limited slots available. Book your slot soon.") and a "Book your open-house slot" button that pre-selects Karwachauth in the form.
- **Time-bound:** after 28 Oct 2026, 4 PM (`CONFIG.EVENT_END`) the open-house band removes itself, the hero eyebrow becomes "Henna by Surbhi", and the form/close bands swap colours so light and dark still alternate.
- Booking form: name (required), occasion chips, how many people, day/time, notes. Submits as a pre-written text; if Messages doesn't open, it shows the number to call.
- Floating gold text circle: appears after the hero, hides over the form.
- Favicon / home-screen icon: a gold "S" on green (no logo exists). og.png 1200×630 for the Facebook link preview.

## Assumptions I made
- **Colours** are mine, not hers (no logo, no brand). Green from the henna leaf and her photo's plants; gold for Karwachauth.
- **Occasion chips** "Bridal" and "Festival or party" are customer choices I added; she has only advertised Karwachauth. Nothing on the page claims she does bridal work.
- **Promise line** "I take my time on every hand, so your design comes out the way you pictured it." is written in her voice, not quoted. Same for "I'll get back to you to confirm your time." (deliberately not "text back": texting is unconfirmed).
- **Texting:** unknown whether 908-274-4044 takes texts. It's a mobile-style number and she wrote "reach out @", so text is primary, but every text path also shows the number to call.
- **Where:** "North Brunswick" only; no address (unknown whether it's her home, a studio or mobile).
- Instagram link: verified live 2026-10-20 (display name "HennaBySurbhi", 70 posts). Its profile picture is a personal couple photo, so I didn't use it.

## Placeholders and gaps
- Only one work photo (from the group post, 600×800). The page needs 3–6 more; her Instagram has 70 posts (Muse can't log in there).
- No logo, email, Facebook page, reviews, prices, regular hours, address. Footer has no email (none found; not invented).
- **After Oct 28:** the page tidies itself, but the meta description, og:description and og.png still advertise the open house, and Facebook caches link previews. Regenerate og.png and rewrite both descriptions then.
- The photo is 600px wide, so on a 2x phone (350 CSS px) it is slightly upscaled. It is her only photo; swap in larger originals when she sends them.

## Questions for the owner
- Do you take texts on 908-274-4044?
- Where do appointments happen: your home in North Brunswick, a studio, or do you travel to clients?
- What else do you do: bridal, Eid/Diwali/Teej, baby showers, parties? Any starting prices?
- Can we use 4–6 of your Instagram photos (hands and feet, no faces)?
- Regular hours outside the open house?
- A business name you prefer on the page: "Henna Artist Surbhi" (your post) or "HennaBySurbhi" (Instagram)?

## Ideas not built (yours to pick)
- **Runner-up world (signature motion, opt-in):** a henna cone piping a vine of paste across the hero that dries from dark green-black to stain red-brown. Other worlds considered: drying paste cracking and flaking to reveal the stain; marigold petals; mehndi leaf pattern growing along band edges; Karwachauth moon and sieve. Neha's site already lets you pipe henna, so the drying/staining one is the differentiator.
- A small gallery (3–6 photos in 4:5 cards) once she sends photos.
- Services/occasions list as short items once she confirms them.
- The photo is a plain rounded card (the finish reviewer called it close to "dropped in"); frame it better once there are more photos.
- A "how booking works" 3-step band (cut to keep the page short with so little content).
- An Instagram embed is not worth it (heavy, tracking).
- Impeccable findings left standing because they're your calm-style choices: eyebrow pills (craft floor bans them), the diagonal band texture (`repeating-stripes-gradient`), the hero bounce-in, the floating circle, Cal Sans. The detector's `flat-type-hierarchy` note counts only the small UI sizes (11–20px); the headings run 30–80px.

## Not verified
- Real-device touch, and the real SMS handoff on iOS and Android (tested: the composed text decodes correctly; `sms:` opening was not tested on a device).
- Inside Facebook's in-app browser.
- Frame rate on old phones (only the H1 bounce-in and the fade-up move).
- I skipped Impeccable's interactive world-picking page: the build runs unattended by design.
