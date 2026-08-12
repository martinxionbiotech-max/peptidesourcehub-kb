---
title: Quality Control Framework — PeptideSourceHub
description: Multi-layer quality control framework covering in-process, release, and pre-shipment testing gates with full analytical methodology and documentation standards.
schema_type: TechArticle
---

# Quality Control Framework

## Quality Philosophy

PeptideSourceHub operates under a **three-gate quality system** that subjects every production batch to analytical verification at multiple stages. This multi-layer approach ensures that quality is not merely tested at the end — it is built into every step of the manufacturing process. Our facility has maintained this framework since 2009, with a production record exceeding 2 million vials.

Our QC system is aligned with:

- **ISO 9001:2015** Quality Management Systems
- **ICH Q7** GMP for Active Pharmaceutical Ingredients
- **USP <1503>** Peptide Quality Attributes

## Three-Gate Quality System

```
┌─────────────────────────────────────────────────────────────┐
│                     MANUFACTURING FLOW                       │
│                                                              │
│  Raw Materials → Synthesis → Purification → Packaging       │
│        │             │            │            │             │
│        ▼             ▼            ▼            ▼             │
│    [Gate 1]      [Gate 1]     [Gate 2]     [Gate 3]        │
│  In-Process   In-Process    Release     Pre-Shipment        │
│  Inspection   Monitoring    Testing     Verification        │
└─────────────────────────────────────────────────────────────┘
```

### Gate 1: In-Process Controls

| Stage | Control Point | Method | Acceptance Criteria |
|-------|--------------|--------|---------------------|
| **Raw Material Receipt** | Amino acid identity & purity | HPLC, TLC | ≥99% individual amino acid purity; identity confirmed |
| **Raw Material Receipt** | Resin and reagent quality | Supplier COA review | Meets specification per approved supplier list |
| **Solid-Phase Synthesis** | Coupling efficiency monitoring | Kaiser/ninhydrin test, conductivity | ≥99% coupling efficiency per cycle |
| **Cleavage & Deprotection** | Crude peptide identity | HPLC screening, MS | Target peak present; major impurities identified |

### Gate 2: Release Testing

All products must pass Gate 2 before advancing to final packaging:

| Test | Method | Reference Standard | Acceptance Criteria |
|------|--------|--------------------|---------------------|
| **Purity** | RP-HPLC (C18, ACN/water/0.1% TFA gradient) | USP <621>, Ph.Eur. 2.2.46 | ≥99.0% main peak area |
| **Identity (MW)** | ESI-MS | — | Mass within ±1.0 Da of theoretical [M+H]<sup>+</sup> |
| **Peptide Content** | Amino acid analysis or nitrogen content | USP <1051> | ≥85% (typical: 85–92%) |
| **Residual TFA** | Ion chromatography | — | ≤0.1% (w/w) |
| **Appearance** | Visual inspection | — | White to off-white lyophilized powder |
| **Solubility** | Gravimetric in recommended solvent | — | ≥1 mg/mL in specified solvent |

### Gate 3: Pre-Shipment Verification

Before any batch is released for shipment, Gate 3 confirms:

| Check | Scope |
|-------|-------|
| **Batch Documentation Audit** | COA, MS spectra, HPLC chromatogram reviewed and approved |
| **Label Verification** | Product name, batch number, quantity, storage conditions correct |
| **Packaging Integrity** | Vacuum-sealed vials, desiccant present, tamper-evident seals intact |
| **Storage Conditions** | Temperature log verified (-20°C ± 5°C) throughout storage period |
| **Documentation Package** | All quality documents collated and verified for completeness |

## Analytical Instrumentation

Our QC laboratory is equipped with the following primary analytical instruments:

| Instrument | Model Range | Application |
|------------|-------------|-------------|
| **Analytical HPLC** | Agilent 1260 Infinity II series | Purity determination, impurity profiling |
| **Preparative HPLC** | Agilent / Shimadzu preparative systems | Purification at gram scale |
| **Mass Spectrometer** | ESI-MS (single quadrupole) | Molecular weight confirmation |
| **MS/MS** | Triple quadrupole (select products) | Sequence verification by fragmentation |
| **Lyophilizer** | Labconco / Christ freeze-dryers | Final product preparation |
| **Analytical Balance** | Mettler Toledo (0.01 mg readability) | Weighing and content determination |
| **Ion Chromatograph** | Metrohm | Residual counter-ion analysis (TFA, acetate) |

## QC Personnel & Training

Our quality team is structured for independence and accountability:

| Role | Responsibility |
|------|---------------|
| **QC Director** | System oversight, OOS investigations, batch release authorization |
| **QC Analysts** | Routine HPLC, MS, and content analysis per SOP |
| **QA Manager** | GMP compliance, SOP management, deviation/CAPA handling |
| **Documentation Specialist** | COA issuance, batch record review, archive management |

All analytical staff undergo documented training on each SOP, with periodic requalification. Training records are maintained as part of the ISO 9001 QMS documentation.

## In-Depth Quality Guides

→ **[Certificate of Analysis & Purity Analysis](coa-purity-analysis.md)** — How to read, verify, and challenge a COA  
→ **[HPLC Chromatography](hplc-chromatography.md)** — Methodology, peak interpretation, and impurity identification  
→ **[Mass Spectrometry](mass-spectrometry.md)** — ESI-MS, MALDI-TOF, MS/MS, and spectrum interpretation  
→ **[Batch Traceability](batch-traceability.md)** — Lot numbering, traceability chain, and audit trails  
→ **[Documentation Package](documentation-package.md)** — Standard and extended documentation deliverables  

---

← [Back to Knowledge Base Home](../index.md) | [COA & Purity Analysis →](coa-purity-analysis.md)
