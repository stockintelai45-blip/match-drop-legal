# Decisions log — Boinkle legal pages

Autonomous run, 2026-11-06. Assumptions made without asking:

- Renamed app from "Match Drop" to "Boinkle" everywhere (previous pages were for a different,
  no-ads game called Match Drop; task specified Boinkle).
- Kept existing visual style (light blue gradient, rounded card, `--accent` orange pill,
  `"Fredoka",ui-rounded,"Nunito",system-ui,sans-serif` stack) rather than redesigning — task said
  "keep the existing styling, but restyle to match the game," and the existing CSS already matches
  the spec (light blue panel, rounded cards, Fredoka-like rounded font, system fallback).
- Governing law for Terms of Use: Sweden, per explicit instruction (placeholder, flagged in the
  HTML comment at the top of terms.html as needing lawyer review).
- Contact email: left as literal `YOUR-EMAIL-HERE` placeholder in all three pages, listed in
  USER-TODO.md.
- Supervisory authority named in the GDPR rights section: Swedish IMY, per explicit instruction.
- In-app purchases section is written in future/conditional tense ("if added", "may add") since
  purchases don't exist yet, per the brief ("optional in-app purchases added later").
- Restore Purchases FAQ entry explains there's nothing to restore yet, rather than omitting the
  question, since the brief asked for a placeholder.
- Footer nav added to all three pages linking to each other (index.html / terms.html /
  support.html), per instruction 4.
- No JavaScript added anywhere, per instruction 4.
- External links present: Google's privacy policy, Google's "how Google uses information" page,
  and Apple's standard EULA page. These are required references per the brief; they do not fire
  network requests on page load (they're plain `<a href>` elements, not scripts/fetches), so the
  "zero external requests" verification requirement (which concerns what the page itself loads)
  still passes — confirmed via Playwright network-request capture.
- Verification done with Playwright (chromium) at 390x844, file:// URLs, networkidle wait;
  confirmed 0 console errors, 0 external requests, all internal links (index.html/terms.html/
  support.html) present and mutually resolvable; screenshots saved to `verification/`.
