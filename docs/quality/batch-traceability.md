---
title: "Batch Traceability System — PeptideSourceHub"
description: "Technical documentation of the batch traceability system used in peptide manufacturing — lot numbering, audit trail, raw material mapping, and OEM batch number integration."
schema_type: TechArticle
---

# Batch Traceability System

## Overview

Batch traceability is the backbone of quality assurance in peptide manufacturing. A traceability system ensures that every vial can be mapped back to its complete production and testing history — from raw material lot numbers through synthesis, purification, QC testing, and final packaging.

At PeptideSourceHub, traceability is not an optional add-on. It is integrated into every production lot through:

- **Unique batch numbers** assigned at synthesis initiation
- **Documented material flows** at every processing step
- **QC data linkage** — HPLC chromatograms, MS spectra, and COA data keyed to batch number
- **OEM batch number mapping** for private-label customers

## Lot Numbering System

### Format: `PSH-[YY]-[SEQ]-[MONTH][CHECK]`

| Component | Example | Meaning |
|---|---|---|
| `PSH` | PSH | Peptide Source Hub identifier |
| `[YY]` | 26 | Production year (2026) |
| `[SEQ]` | 01837 | Sequential production number |
| `[MONTH]` | 08 | Production month (August) |
| `[CHECK]` | A | Check character (alphabetic) |

**Example**: `PSH-26-01837-08A` identifies batch 18,387 produced in August 2026, with integrity check character "A".

### Batch Number Assignment

- Assigned at **synthesis initiation** — not at packaging
- Printed on **COA, vial labels, kit box, and shipping documentation**
- **Never reused** — even for re-synthesis of the same peptide
- Stored in **immutable batch record database** with full production audit trail

## Traceability Chain

Every production lot follows a documented chain of custody through the manufacturing process:

```
Raw Materials → Synthesis → Purification → QC Testing → Packaging → Shipment
     │               │           │              │            │           │
     ▼               ▼           ▼              ▼            ▼           ▼
  Material      Synthesis   HPLC Run#      QC Batch#    Packaging    Shipping
  Lot #s        Batch#      Fraction#      COA ID       Lot#         Tracking#
```

### Stage-by-Stage Traceability

| Stage | What Is Recorded | Linked To |
|---|---|---|
| **Raw Materials** | Amino acid derivative lot #, resin lot #, solvent batch #, reagent certificates | Synthesis Batch # |
| **Synthesis** | Operator, date, equipment ID, synthesis scale, coupling efficiency data | Batch # |
| **Purification** | Preparative HPLC run #, column ID, fraction collection details, solvent batch # | Batch # |
| **Lyophilization** | Freeze-dryer ID, cycle parameters, duration, vacuum profile | Batch # |
| **QC Testing** | Analytical HPLC run #, MS acquisition ID, Karl Fischer run #, COA ID | Batch # |
| **Vial Filling** | Filling date, operator, equipment ID, in-process weight checks | Batch # |
| **Packaging** | Kit assembly date, packaging lot, label batch, serial number range | Batch # + Shipping Tracking # |
| **Shipment** | Carrier, tracking #, export documentation, commercial invoice # | Batch # + Order # |

## Documentation Audit Trail

### For Every Batch, the Following Records Are Maintained:

1. **Batch Manufacturing Record (BMR)** — Complete production history
2. **Analytical Data Package** — Raw HPLC chromatograms, MS spectra, any additional testing
3. **Certificate of Analysis (COA)** — Summarized quality data signed by QC reviewer
4. **Material Safety Data Sheet (MSDS)** — Safety and handling information
5. **Packaging Record** — Filling weights, vial counts, label verification
6. **Shipping Record** — Carrier, tracking number, export documents

### Record Retention

| Record Type | Retention Period |
|---|---|
| Batch Manufacturing Records | Minimum 5 years |
| QC Analytical Data | Minimum 5 years |
| COA Archive | Indefinite |
| Shipping Records | Minimum 3 years |

## OEM Batch Number Mapping

For OEM and private-label customers, PeptideSourceHub maintains a **dual-numbering system**:

| Layer | Number | Example |
|---|---|---|
| **Internal (PSH)** | PSH production batch number | `PSH-26-01837-08A` |
| **Customer-facing** | Brand's own lot number | `BRAND-A-2026-08` |

The OEM batch mapping provides:

- **Full traceability from customer label back to PSH manufacturing records**
- **Customer-facing batch numbers** that align with the buyer's own coding system
- **Quality documentation** referencing both internal and customer-facing batch numbers
- **Retrospective traceability** — if a customer reports an issue 12 months later, the batch can be traced back within minutes

## Traceability in Practice

When a researcher or procurement manager contacts PeptideSourceHub with a batch number:

1. **≤ 60 seconds**: Batch record located in database
2. **≤ 5 minutes**: Full manufacturing history and QC data retrieved
3. **≤ 1 business day**: Complete documentation package (BMR, COA, MS spectra, HPLC chromatograms) available for re-issue

This capability is not theoretical — it's operational. Every batch record is maintained in a searchable database with QC documentation archived in both electronic and physical formats.

## Related Resources

- [COA & Purity Analysis Guide](coa-purity-analysis.md)
- [Documentation Package](documentation-package.md)
- [Quality Control Framework](index.md)
- [GMP Guidelines](../regulatory/gmp-guidelines.md)
