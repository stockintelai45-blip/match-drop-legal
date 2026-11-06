# User TODO — before shipping Boinkle's store listings

1. **Replace the contact email.** Find/replace `YOUR-EMAIL-HERE` in all three pages:
   - `docs/index.html`
   - `docs/terms.html`
   - `docs/support.html`

2. **Have the text reviewed.** `docs/terms.html` is explicitly marked as a template (see the HTML
   comment at the top of the file) — get it checked by a qualified lawyer before relying on it,
   and ideally have the privacy policy checked too given the GDPR/AdMob content.

3. **Push to the public repo and enable Pages:**
   - Push this repo to `https://github.com/stockintelai45-blip/match-drop-legal` (public).
   - In GitHub: Settings > Pages > Source = branch `main`, folder `/docs`.
   - Resulting URLs:
     - Privacy: `https://stockintelai45-blip.github.io/match-drop-legal/`
     - Terms: `https://stockintelai45-blip.github.io/match-drop-legal/terms.html`
     - Support: `https://stockintelai45-blip.github.io/match-drop-legal/support.html`

4. **Wire the URLs into the stores:**
   - App Store Connect: set Privacy Policy URL (privacy page) and Support URL (support page).
   - Google Play Console: set Privacy Policy URL and (optionally) a support/contact URL.

5. **Keep App Privacy / Data Safety answers consistent with this policy:**
   - Declare AdMob's data collection (device identifiers, IP/approximate location, ad interaction
     data) in both App Store "App Privacy" and Play "Data Safety" forms.
   - Declare on-device-only storage of best score / level progress / settings (no account, no data
     linked to identity beyond what AdMob itself collects).
   - When in-app purchases ship, add RevenueCat + purchase data to both forms and update
     `docs/index.html`'s "In-app purchases" section from future tense to present tense if its
     wording needs it.
