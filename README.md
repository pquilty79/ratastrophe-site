# Ratastrophe website

Static product information, support, and privacy website for Ratastrophe, for the Ratastrophe app. Follows the structure of the developer’s Presents of Mind site, with Ratastrophe branding, existing app artwork, and information checked against the native app source.

## App Store URLs

- Marketing: https://pquilty79.github.io/ratastrophe-site/
- Support: https://pquilty79.github.io/ratastrophe-site/support.html
- Privacy policy: https://pquilty79.github.io/ratastrophe-site/privacy.html

Support email: **supportchesstimewars@gmail.com**, the shared support mailbox already published on the developer’s example website. Ratastrophe email links use an app-specific subject.

## Publishing

GitHub Pages serves **main → /docs**, using **Deploy from a branch**. No build system, JavaScript runtime, external font, analytics, contact-form service, or package installation is needed by the website. `docs/.nojekyll` keeps publishing static. The repository contains the public website only; native app source is separate.

For local preview, run `python3 -m http.server 4173 --directory docs` and open http://127.0.0.1:4173/.

## App Store review references

Checked November 9, 2026:

- [Apple’s Support URL definition](https://developer.apple.com/help/app-store-connect/reference/app-information/platform-version-information/): the support website must provide actual contact information for app issues, feedback, and feature requests.
- [App Review Guideline 1.5](https://developer.apple.com/app-store/review/guidelines/#developer-information): the app and its Support URL must provide an easy way to contact customer service.
- [App Review Guideline 5.1.1](https://developer.apple.com/app-store/review/guidelines/#data-collection-and-storage): the privacy policy must explain data handling, use, retention/deletion, and choices; its link is also required in App Store Connect and inside the app.

The website supplies public contact and privacy pages. Publishing it does not itself configure App Store Connect, add links inside the native app, verify the live in-app purchase product, or guarantee App Review approval. Those are separate release tasks.

## Maintenance

The privacy text reflects the current app: local campaigns/achievements, StoreKit purchases, locally generated fictional sponsor messages, and no third-party analytics/advertising SDK. Update it before introducing cloud saves, real advertising networks, analytics, accounts, or other new data flows. Keep the support inbox monitored and revise instructions when controls change.

The icon is copied from the existing Ratastrophe app asset catalog, without alteration. No new artwork was generated for this site.

## Validation

On November 9, 2026, the four HTML pages passed responsive browser checks at 320, 390, 768, and 1440 pixels: **16 page/viewport combinations**, with no horizontal overflow or missing images. Eight automated accessibility scans at phone and desktop widths found **zero WCAG A/AA violations** in the rules tested. Keyboard-operated FAQs and the skip link, reduced-motion styling, and larger body text were also checked. Automated scans are not a complete manual accessibility audit.

Static checks validated all **37 local link/anchor references**, unique IDs, the XML sitemap, public customer-service contact information, and the icon’s unchanged provenance. Browser checks followed each distinct internal link and checked its target. The published website has no script, iframe, form, external font, or analytics dependency. Visual review covered desktop presentation and the phone contact panel.

Local QA evidence is retained outside the published site at `/tmp/ratastrophe-site-qa/`, including `report.json` and screenshots. These development checks do not modify the native app or its saved games.
