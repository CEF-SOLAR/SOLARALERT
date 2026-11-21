# AlertaSolar — Revision History

**Author / Project Director:** Carlos Eduardo Francheri — Geologist · Independent SCADA developer specializing in solar photovoltaic energy  
**Purpose:** A concise, human-readable release log in the tradition of classic software revision files. Entries appear newest first; every released build retains its full versioned filename.  
**Downloads:** [GitHub Releases](https://github.com/CEF-SOLAR/SOLARALERT/releases) · [Project README](README.md)

> This log begins with the currently reviewed 5.48 build. Earlier versions are not reconstructed without verified records or a source comparison. Do not treat a feature verified in one build as proof that it was first introduced in that build.

---

## 5.48 — 2026-11-21

**Distribution:** `AlertaSolar_V5_EN_5.48.html`  
**Language:** English  
**Record:** First entry in the public revision log; reviewed against the HTML 5.48 source.

**DOCUMENTED AND CONFIRMED IN THIS BUILD**
- The operational local heuristic `R_Local` is bounded to **[0, 1]**; the unsaturated `R_local,raw` remains available for diagnostics.
- Scientific HUDs distinguish the raw product from the bounded operational index.

**VERIFIED BY STATIC SOURCE REVIEW**
- Chart 6 references the bounded local index and exposes raw diagnostic information in its historical tooltip.
- Operational index levels and relevant alert paths reference the bounded value.

**SCIENTIFIC STATUS:** `I_Global` and `R_Local` are dimensionless, experimental heuristic indicators, not measured GIC (A) or induced electric fields (V/km). Observational calibration is still required.

**Verification scope:** Static inspection of the supplied HTML 5.48; not an end-to-end live-operational test. With no older source file for a direct diff, these are documented characteristics of 5.48, **not a claim that every feature originated in this release**.

---

## Entry template for the next published version

<!-- Copy this block ABOVE the preceding version, replace the placeholders, and remove the HTML comment delimiters.
## X.XX — YYYY-MM-DD

**Distribution:** `AlertaSolar_VX_EN_X.XX.html`

**ADDED**
- ...

**CHANGED**
- ...

**FIXED**
- ...

**NOTES**
- ...
-->
