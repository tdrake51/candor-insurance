# Candor Insurance Brokerage Inc — Segment Landing Pages

Static landing pages for Candor Insurance Brokerage Inc. Each page serves a
specific audience segment and embeds a shared intake form. No build step,
no dependencies — plain HTML and CSS.

---

## Pages

| File | Audience |
|------|----------|
| `landlord-insurance-readiness.html` | Landlords & rental property owners |
| `rental-portfolio-review.html` | Investors with multiple properties |
| `fix-and-rent-investor.html` | Fix-and-rent / vacant / builder's risk |
| `temporary-displacement-housing.html` | Mid-term & displacement housing providers |
| `supportive-recovery-housing.html` | Supportive & recovery housing operators |
| `behavioral-health-human-services.html` | Behavioral health & human services agencies |
| `candor-styles.css` | Shared stylesheet — **required** by all six pages |

> All six pages link to `candor-styles.css`. Keep every file in the same
> folder or the pages will load without styling.

---

## What each page does

- Presents Candor's readiness-and-referral model for that audience
- Embeds a shared Google Form for intake
- Provides click-to-email and click-to-call contact
- Tags every inquiry with the originating page for attribution

---

## Setup

Two values are already wired into the page scripts:

- **Google Form URL** — the shared intake form
- **Source Code field ID** — the hidden question each page stamps automatically

Each page silently fills a "Source Code" question on the shared form, so every
submission lands in the linked responses spreadsheet already labeled by page.

### One item still on placeholder

- **Phone number.** Pages currently dial `718-831-2066`. To route calls through
  a tracking number, update `var PHONE_DIAL` near the bottom of each page.

---

## Publishing with GitHub Pages

1. Push all seven files to the repository root.
2. **Settings → Pages**, set the source to the `main` branch, folder `/ (root)`, and Save.
3. Wait a few minutes for the site to build.
4. Pages are served over HTTPS at
   `https://<username>.github.io/<repo>/<file>.html`.

### Note on visibility

A free GitHub Pages repository is **public** — anyone can read these files.
That's fine for marketing pages. Do **not** add private notes, credentials,
internal strategy, or backend configuration to this repository.

---

## Testing the tracking

1. Open each published page.
2. Submit one test entry through the embedded form.
3. Confirm the **Source Code** column in the responses spreadsheet shows the
   correct code for that page.

If the Source Code arrives blank, verify the form's "Source Code" question is a
**Short answer** field (multiple-choice or dropdown questions reject prefilled
values that aren't exact listed options).

---

## Compliance

Candor Insurance Brokerage Inc is a licensed insurance brokerage. All coverage
advice, quoting, and policy placement are provided by licensed insurance
professionals. Content in these pages is general in nature and does not
constitute an offer of insurance, a quote, or a guarantee of coverage.
Availability of programs and coverages varies by state and is subject to
carrier underwriting.

---

*Internal reference. Contact: Candor Insurance Brokerage Inc · sglanz@candorins.com · candorins.com*
