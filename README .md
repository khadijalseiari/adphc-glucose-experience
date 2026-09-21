# Blood Glucose Experience — ADPHC

A bilingual (English / Arabic) public-health education application developed for the
**Abu Dhabi Public Health Centre (ADPHC)**.

The application uses two interactive, evidence-based activities to demonstrate how
**food order** and **post-meal walking** affect the blood glucose response.

---

## Live application

**[https://&lt;your-username&gt;.github.io/&lt;your-repo-name&gt;/](https://khadijalseiari.github.io/adphc-glucose-experience/)**

*(Replace the placeholders once GitHub Pages is enabled.)*

---

## About

| | |
|---|---|
| **Owner** | Abu Dhabi Public Health Centre (ADPHC) |
| **Purpose** | Public-health education |
| **Languages** | English and Arabic (full RTL support) |
| **Format** | Single standalone HTML file |
| **Size** | 3.81 MB (3,991,126 bytes) |
| **SHA-256** | `b9439876d05e418aec5447482d380fcfab943ab8a87c34f2f1e72f6ad3c5dfff` |

---

## Activities

### 1. Nutrition — food order
Scenario-based questions on the sequence in which foods are eaten, followed by an
animated comparison of the resulting glucose response curves, with supporting evidence
and source citations.

### 2. Physical Activity — post-meal walking
Scenario-based questions on walking after eating, followed by an animated
three-curve comparison with the published peak values marked.

---

## Technical characteristics

The application is a **single self-contained HTML file**:

- All HTML, CSS and JavaScript are inline
- All nine images are embedded as Base64 data URLs
  (1 logo + 2 homepage activity icons + 6 in-game illustrations)
- **Zero external dependencies** — no CDNs, no external fonts, stylesheets or scripts
- **Zero network requests** on load
- **Runs fully offline** — the file works by double-clicking it locally
- No data collection, no cookies, no local storage, no authentication, no tracking

The only external URLs in the file are the scientific citation hyperlinks in the
references section, which resolve only if a user deliberately clicks one.

---

## Usage

### Online
Open the GitHub Pages link above in any modern browser.

### Offline
Download `index.html` and open it directly in a browser. No installation,
no server and no internet connection is required. This is the recommended
method for live workshop delivery, as it removes any dependency on venue Wi-Fi.

### Browser support
Any current version of Chrome, Edge, Firefox or Safari, on desktop, tablet or mobile.

---

## Scientific integrity

This application presents peer-reviewed published findings. The following
constraints are deliberate and **must not be altered**:

- The **Nutrition graphs show relative comparisons only.** They intentionally do not
  display numeric glucose concentrations, because the source publications do not
  report measured values at every time point. Adding values would fabricate data.
- The on-screen text **"Relative comparison — not measured glucose concentrations"**
  must remain exactly as written, in both English and Arabic.
- The **Physical Activity** graph retains the published peak values and the original
  statistical note recording that the two walking conditions did not differ
  significantly from each other.
- No axis values, tick labels, interpolated points, smoothed curves or additional
  quantitative values may be introduced.
- No scientific claim, citation, statistical statement, population description or
  disclaimer may be added, removed or reworded.
- The data constants `PRE_C` and `UAE_C` are calibrated and must remain unchanged.

---

## Disclaimer

> For public-health education only. This tool does not predict your individual glucose
> response, diagnose diabetes or prediabetes, or replace medical advice.
> Individual glucose responses vary.

This disclaimer appears on every screen of the application and must not be removed,
relocated or altered.

---

## Sources

The application cites peer-reviewed research indexed on PubMed and published in
*Scientific Reports*. Full citations appear within the application's evidence and
references sections.

---

## Contributing

This is a finalised, approved public-health resource. Its content underwent multiple
scientific review cycles.

**Pull requests altering scientific content, data constants, graph rendering,
wording or disclaimers will not be accepted.**

For corrections, please contact ADPHC directly rather than submitting changes.

---

## Verifying file integrity

To confirm a copy is unmodified:

```bash
sha256sum index.html
```

```powershell
Get-FileHash .\index.html -Algorithm SHA256
```

Expected result:

```
b9439876d05e418aec5447482d380fcfab943ab8a87c34f2f1e72f6ad3c5dfff
```

Any other value means the file has been altered.

---

© Abu Dhabi Public Health Centre (ADPHC)
