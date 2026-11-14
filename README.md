# Protected on Paper — Free Colorado Assistance Checker (v5.3)

A free, standalone Colorado assistance-reference calculator built as one `index.html` file. It runs in the visitor's browser with no paid hosting, database, app download, subscription, or outside JavaScript libraries.

**Status:** The standalone calculator is publicly served at https://streamlinedsystemsolutions.github.io/protected-on-paper-calculator/ on free GitHub Pages. The latest keyboard-accessibility patch deployed successfully. This does not mean all benefits data, devices, accessibility needs, and external provider links have passed full hard-launch QA.

## Enable GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/(root)**, then **Save**.
4. Wait for GitHub to show its own **Visit site** link, then open the exact HTTPS address displayed there.
5. Test the calculator on a real mobile phone and computer before linking it from Protected on Paper. Return to the main WordPress site using **Back to Protected on Paper**.

A GitHub Free account supports Pages with a public repository. No custom domain, paid GitHub plan, or WordPress upgrade is required.

## Important boundaries

- The calculator is an **educational estimate**, not an eligibility approval, legal opinion, guarantee of program funding, or application.
- ZIP-code guidance does not establish city limits or exact service boundaries. Users must verify county and municipality as well as current program eligibility.
- Medical expense illustrations are not universal rent determinations. For Section 8 calculations, confirm the applicable policy, effective date, hardship/transition eligibility, expenses, and the agency's worksheet.
- User-entered values are processed within the browser. GitHub as the website host may collect standard access logs.
- **Do not** add personal housing records, pay stubs, passwords, private email, real client information, health records or API secrets to this public repository.
- The `index.html` currently has a staging `noindex,nofollow` directive; remove only after a complete public-release review.
- Passing a local Chromium check does not replace a real GitHub Pages HTTPS, Android/iOS, Firefox, Safari, keyboard, and screen-reader test.
- The primary Protected on Paper WordPress site remains private until separate hard-launch approval.

Official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Accessibility and data-integrity checkpoint — November 13, 2026

- Accessibility patch: commit `6b356a6ecb76b14fa88b35823f6ba704632fba1f` (plain-English three-step introduction, keyboard focus restoration after closing the screening dialog, dialog description for screen readers, and truthful GitHub hosting/privacy wording). All original embedded benefit data and mathematical formulas were preserved.
- Verified the linked GitHub Pages deployment completed successfully: https://github.com/streamlinedsystemsolutions/protected-on-paper-calculator/actions/runs/43551326481
- 48/48 **local** Chromium interaction regression checks passed at 320, 390, 768, and 1280px: modal opening/closing, Escape, keyboard focus, ZIP/county/income validation, results focus, 5%/$845 and 10%/$890 illustrative rent samples, no script errors, no outbound data requests, and no horizontal overflow. These are local browser tests, not separate iOS/Safari/Firefox or screen-reader certification.
- Structural data QA: 64 unique counties and matching county-contact entries, 642 five-digit ZIP entries with no unknown counties, 62 local-program records with HTTPS URLs and unique IDs, 2,652 rule entries with valid sources and nonnegative numeric values. ZIP coverage, official current benefit limits, agency eligibility, dates and funding availability still require independent source checks.
- This calculator remains an educational starting point. Do not treat a matching amount, medical threshold selection, county hint, or resource listing as an approval or currently open application. The main WordPress website remains private while its separate hard-launch QA is unfinished.

## Public calculator safety and comprehension update — November 13, 2026

- Committed calculator patch [8c8579ae5](https://github.com/streamlinedsystemsolutions/protected-on-paper-calculator/commit/8c8579ae542c8099adbc3f304606cabe68d89ea7). [GitHub Pages deployment succeeded](https://github.com/streamlinedsystemsolutions/protected-on-paper-calculator/actions/runs/43558654660).
- Explained medical-expense eligibility for elderly/disabled families and separate disability work-related expenses; anchored to [24 CFR § 5.611](https://www.law.cornell.edu/cfr/text/24/5.611).
- Clarified that 5% and 7.5% are conditional phase-in/hardship thresholds, not rates a tenant can choose; preserved the prior 5% **example default** and unchanged calculator formulas. The 3% rate is historical; 7% is a nonofficial hypothetical comparison; 10% is the standard HOTMA threshold absent eligible relief.
- Added collapsible five-step math explanation and an accessible copyable email request for the housing agency's income, deductions, medical-threshold policy, effective dates and hearing rights. If clipboard permission is blocked, the sample is selected so the user can copy it manually.
- Added plain public 211 Colorado alternate resource route while the main Protected on Paper WordPress site remains private; the source page says links to that private site may request login.
- Moved keyboard focus to the first invalid rent input, rather than requiring the reader to find which field failed.
- Local mirrored-source Chromium checks: **72/72 passed** across 320, 390, 768, 1280px, including sample 5% ($845) and 10% ($890) outputs, copy interaction with a deterministic clipboard stub, error/focus behavior, no horizontal overflow, no JavaScript exceptions or unsolicited network requests. Two inline JavaScript blocks passed `node --check`.
- GitHub content readback verified the embedded 741k-character JSON rule-data block is identical before and after the patch. This is not an independent legal accuracy certification.
- **Remaining:** Real Safari/iOS and Firefox testing, actual screen reader and keyboard usability with people needing accommodations, real clipboard permission on live HTTPS (the local test used a stub), verifying current provider links and incomplete ZIP/jurisdiction data, and all private WordPress launch gates. The browser sandbox disallowed direct live navigation, although a separate public HTTP scanner reached the live site. Site staging `noindex,nofollow` remains intentionally active.
