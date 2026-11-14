# Operational Templates

**Open, reusable templates for operational readiness — connecting personnel readiness, equipment availability, and outstanding work into views supervisors can act on.**

**Live:** https://chavobutassi.github.io/operational-templates/
**Author:** Claudio Julián Butassi — Data Analytics

---

## Purpose

Organizations that protect facilities and coordinate field teams — private security
providers, water & wastewater operators, transportation and facility maintenance
contractors — all face the same information question: *which people are available and
qualified, which equipment is ready, and what work is still outstanding?*

This repository publishes **open templates** that answer that question in a consistent,
documented way. Each template ships with standard fields, documented indicators, and
built-in validation, so any organization can examine and adapt it **without commissioning
a new system**. All examples use **demonstration data only** — no real individuals or
organizations.

This is the knowledge-sharing component of my proposed U.S. endeavor: making reusable
data structures, indicator definitions, and validation procedures freely available, paired
with a working reference implementation.

## Templates

| Template | What it does | Status |
|---|---|---|
| **Operational Readiness Template** | Personnel-readiness register + equipment/work-order view + indicator dictionary + validation checklist, all in one self-contained page | ✅ published |
| Asset / work-order data structure | Standalone data model + dictionary for equipment and maintenance records | planned |
| Indicator dictionary | Reusable indicator definitions (coverage, expirations, availability, overdue work) | planned |
| Validation checklist | Portable data-validation rule set with examples | planned |

## How to use

Every template is a **single, self-contained HTML file** — no build step, no server, no
external dependencies. Open `docs/index.html` in any browser, or view it live on GitHub
Pages. To adapt it, replace the demonstration data block with your own authorized records;
the data model and indicator definitions are documented inside the page.

## Design principles

- **Demonstration data only** — nothing in this repository contains real personnel,
  equipment, or organization records.
- **Indicators are defined, not assumed** — each metric ships with its definition, source
  field, and update frequency.
- **Validation is visible** — records are checked before they feed any indicator, and every
  exception is surfaced rather than silently dropped.
- **Decisions stay with the organization** — the templates organize and present
  information; operational decisions and technical assessments remain with the
  responsible personnel.

## Related projects

- [vaca-muerta-analytics](https://github.com/chavobutassi/vaca-muerta-analytics) — production analytics + asset-register and IFC data validation (public data).
- [permian-analytics](https://github.com/chavobutassi/permian-analytics) — automated analytics on U.S. critical-infrastructure (energy) data.

---

*Built by [Claudio Butassi](https://github.com/chavobutassi) — data analyst. Templates are free to adapt with attribution; all example data is synthetic.*
