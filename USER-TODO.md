# User TODO — before shipping Boinkle's store listings

1. ~~Replace the contact email.~~ **Done** — `support@stockintel.app` is set in all three pages
   (`docs/index.html`, `docs/terms.html`, `docs/support.html`).

2. **Push to the public repo and enable Pages:**
   - Push this repo to `https://github.com/stockintelai45-blip/match-drop-legal` (public).
   - In GitHub: Settings > Pages > Source = branch `main`, folder `/docs`.
   - Resulting URLs:
     - Privacy: `https://stockintelai45-blip.github.io/match-drop-legal/`
     - Terms: `https://stockintelai45-blip.github.io/match-drop-legal/terms.html`
     - Support: `https://stockintelai45-blip.github.io/match-drop-legal/support.html`

3. **Wire the URLs into the stores:**
   - App Store Connect: set Privacy Policy URL (privacy page) and Support URL (support page).
   - Google Play Console: set Privacy Policy URL and (optionally) a support/contact URL.
   - Keep App Privacy / Data Safety answers consistent with this policy: declare AdMob's data
     collection (device identifiers, IP/approximate location, ad interaction data), and on-device
     -only storage of best score / level progress / settings (no account).

4. **Have the text reviewed by a qualified lawyer.** `docs/terms.html` is explicitly marked as a
   template (see the HTML comment at the top of the file) — get it checked before relying on it,
   and ideally have the privacy policy checked too given the GDPR/AdMob content.
