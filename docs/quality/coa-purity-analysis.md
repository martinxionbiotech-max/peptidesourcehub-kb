---
title: Certificate of Analysis & Purity Analysis — PeptideSourceHub
description: Comprehensive guide to reading and verifying a Certificate of Analysis for research peptides. Covers all 10 COA fields, red flags, HPLC chromatogram interpretation, and peptide content vs purity.
---

# Certificate of Analysis & Purity Analysis

## What Is a Certificate of Analysis?

A Certificate of Analysis (COA) is the primary quality document for a research peptide. It provides the analytical evidence that a specific production batch meets the manufacturer's declared specifications. Every batch shipped by PeptideSourceHub is accompanied by a dated, batch-specific COA — never a template or generic document.

A properly issued COA serves three purposes:

1. **Verification** — Confirms that the batch was tested and passed acceptance criteria
2. **Traceability** — Links analytical data to a specific lot number and production date
3. **Comparability** — Enables laboratories to compare results across batches and suppliers

## The 10 Standard COA Fields

Every PeptideSourceHub COA contains the following fields. Understanding each field is essential for evaluating peptide quality and supplier competence.

### 1. Product Name & Catalog Number

```
Product Name: IGF-1 LR3 (Receptor Grade)
Catalog No.: PSH-1001
```

The product name should match the IUPAC or commonly accepted nomenclature. Catalog numbers enable unambiguous order reference. If the product name is ambiguous or uses non-standard naming, request clarification before ordering.

### 2. Batch / Lot Number

```
Batch No.: PSH-20260715-1001-A3
```

The lot number is the single most important identifier on the COA. It must be:

- **Unique** to the production batch
- **Traceable** through all manufacturing and QC records
- **Present** on both the vial label and the COA

PeptideSourceHub uses a structured lot numbering system — see [Batch Traceability](batch-traceability.md) for decoding details.

### 3. Manufacturing Date

```
MFG Date: 2026-07-15
```

The date the synthesis was initiated. This is the starting point for stability and shelf-life calculations. A recent manufacturing date (within 12 months) indicates fresher product.

### 4. Retest Date

```
Retest Date: 2028-07-15
```

Under proper storage conditions (-20°C, desiccated, protected from light), the peptide is expected to maintain specification until this date. After the retest date, the batch should be re-analyzed before use. A typical retest period is 24 months from manufacture date.

| Storage Condition | Expected Stability |
|-------------------|-------------------|
| -20°C ± 5°C, lyophilized, sealed | ≥24 months (to retest date) |
| -80°C, lyophilized, sealed | ≥36 months |
| 2–8°C, reconstituted | Use within 7–14 days (peptide-dependent) |
| Room temperature, reconstituted | Use within 24–48 hours |

### 5. Purity (HPLC)

```
Purity (HPLC): 99.47%
Method: RP-HPLC, C18 column, 214nm detection
```

Purity determined by reverse-phase HPLC is the most commonly reported quality metric. It represents the percentage of the main peak area relative to total integrated peak area in the chromatogram. Key points:

- **≥99.0% is the minimum standard** for PeptideSourceHub products
- Purity is reported to one or two decimal places — not rounded
- The method should specify the column type, mobile phase, and detection wavelength

> **Important:** HPLC purity does not equal peptide content. See the [Peptide Content vs Purity](#peptide-content-vs-purity) section below.

### 6. Molecular Weight (Mass Spectrometry)

```
Molecular Weight: 9117.5 Da
Mass Found (MS): 9117.8 Da ([M+H]+)
Deviation: +0.3 Da (±1.0 Da acceptable)
Method: ESI-MS
```

Mass spectrometric confirmation of molecular weight provides orthogonal identity verification. Required information on a credible COA:

- **Theoretical MW** — calculated from the peptide sequence
- **Observed mass** — the experimental result
- **Ion observed** — indicated as \[M+H\]<sup>+</sup>, \[M+Na\]<sup>+</sup>, or other adduct
- **Deviation** — the difference between theoretical and observed; typically < ±1.0 Da for peptides < 5 kDa

A mass deviation exceeding ±1.0 Da for peptides under 5 kDa warrants investigation. For larger peptides (>5 kDa), slightly larger deviations may be acceptable due to isotopic distribution effects.

### 7. Peptide Content

```
Peptide Content: 88.2%
Method: Amino Acid Analysis
```

Peptide content (also called net peptide content) quantifies the actual amount of peptide present in the lyophilized powder, accounting for:

- **Counter-ions** (TFA, acetate, chloride) from synthesis and purification
- **Residual water** not removed during lyophilization
- **Residual solvents** from manufacturing

The remaining mass (100% − peptide content) is predominantly counter-ion and water. This distinction has direct financial implications: at 88% peptide content, 1 mg of lyophilized powder contains 0.88 mg of actual peptide.

> **Common misunderstanding:** HPLC purity of 99% does not mean 99% of the powder weight is peptide. A peptide may be 99% pure by HPLC but only 85% peptide by weight due to TFA counter-ions and residual moisture.

### 8. Appearance

```
Appearance: White lyophilized powder
```

Visual description of the physical product. Typical acceptable descriptions:

| Appearance | Typical Indication |
|------------|-------------------|
| White lyophilized powder | Normal (most peptides) |
| Off-white lyophilized powder | Normal (some peptides with aromatic residues) |
| White to pale yellow powder | Acceptable for certain peptides |
| Yellow, brown, or discolored powder | Potential degradation — investigate |
| Gelatinous or sticky | Moisture ingress — do not use |
| Clumped or crystalline | Possible moisture exposure — re-analyze |

### 9. Solubility

```
Solubility: ≥1 mg/mL in 0.1% acetic acid
Recommended Solvent: 0.1% acetic acid (v/v) in sterile water
```

Solubility data guides proper reconstitution. The COA should specify:

- **Concentration** — at which solubility was confirmed
- **Solvent composition** — the exact formulation used
- **Observations** — clear solution, slight haze, particles

Solubility testing at PeptideSourceHub is performed gravimetrically: a known mass of peptide is dissolved in a measured volume of solvent, and complete dissolution is verified visually.

### 10. QC Approval & Issuance Date

```
QC Release: Approved by QC Director
Date: 2026-07-22
```

Identifies the authority responsible for batch release and the date of COA issuance. The COA should be signed or approved by a named individual or role, not a generic "QC Department."

## Red Flags: Identifying Low-Quality or Suspect COAs

When evaluating a supplier's COA, the following indicators warrant further investigation:

| Red Flag | Why It Matters |
|----------|---------------|
| **No batch/lot number** | Untraceable — no link to production records possible |
| **Template COA (same data across batches)** | Indicates batch-specific testing is not being performed |
| **COA dated more than 12 months before shipment** | Product may have degraded; testing may no longer be valid |
| **Purity below 99.0%** | Below PeptideSourceHub and industry best-practice standards |
| **No mass spectrometry data** | Identity is unverified; purity alone does not confirm the correct product |
| **Only one detection wavelength (e.g., 280 nm only)** | May miss impurities that absorb at other wavelengths; 214/220 nm is standard for peptide bonds |
| **Purity reported to 0 decimal places** | Suggests rounding; precision matters |
| **No MS ion species specified** | Cannot verify if the observed mass matches the expected adduct |
| **Generic "white powder" without method detail** | Lacks specificity; cannot assess degradation |
| **COA dated before the manufacturing date** | Impossible — indicates falsification |
| **No approval signature or release authority** | No accountability for batch release |
| **Peptide content not reported** | Critical financial and experimental parameter omitted |

## How to Read an HPLC Chromatogram

The HPLC chromatogram is the primary purity evidence on a COA. Understanding how to read it independently is a critical skill for peptide quality assessment.

### Key Elements of a Peptide HPLC Chromatogram

```
 Signal (mAU)
     │
 800 ┤                                    ┌───────────────┐
     │                                    │  Main Peak    │
 600 ┤                                    │  RT: 12.47    │
     │                                    │  Area: 99.47% │
 400 ┤                                    │               │
     │                                    │               │
 200 ┤  ┌─┐                               │               │
     │  │ │ Impurity 1                     │               │
   0 ┤──┴─┴───────────────────────────────┴───────────────┴───
     │  RT: 3.2            ┌─┐
     │  Area: 0.12%        │ │ Impurity 2
     │                     │ │ RT: 10.8
     │                     └─┘ Area: 0.41%
     ├─────────────────────────────────────────────────────────
     0        5        10       15       20       25
                        Time (min)
```

### What to Examine

| Element | What to Look For | What It Indicates |
|---------|-----------------|-------------------|
| **Main peak shape** | Symmetrical, Gaussian | Good column performance, single species eluting |
| **Main peak symmetry** | Tailing factor 0.8–1.3 | Within acceptable range. TF > 1.5 suggests column issues or peptide aggregation |
| **Number of impurities** | 1–3 minor peaks typical at >99% purity | More impurities suggest incomplete purification |
| **Impurity relative abundance** | Each impurity peak <0.5% area | Higher suggests purification issues |
| **Baseline** | Flat, no drift | Solvent quality, column equilibration |
| **Retention time (RT)** | Main peak at distinct RT, consistent across runs | Reproducibility; drifting RT suggests column or pump issues |
| **Void volume peak** | Small peak at ~RT 1–3 min | Unretained material (salts, very polar impurities) — normal if small |
| **Ghost peaks** | Peaks in blank injection | Contamination in system; invalidates run |
| **Integration marks** | Clearly marked start/end for each peak | Proper integration; manual override should be justified |

### Purity Calculation

Purity by area normalization is calculated as:

$$\\text{Purity (\\%)} = \\frac{\\text{Main Peak Area}}{\\text{Sum of All Peak Areas}} \\times 100$$

This is an **area percent** method. It assumes all components have similar extinction coefficients at the detection wavelength (214/220 nm for peptide bonds). This assumption is generally valid for peptide impurities (same backbone chromophore), but may be less accurate for non-peptide impurities.

### Detection Wavelengths

| Wavelength | What It Detects | Use Case |
|------------|----------------|----------|
| **214 nm / 220 nm** | Peptide bond (amide chromophore) | **Primary** — most peptides |
| **254 nm** | Aromatic side chains (Trp, Tyr, Phe) | Cross-check for aromatic impurities |
| **280 nm** | Trp, Tyr only | Selective detection; misses many impurities |

At PeptideSourceHub, the primary detection wavelength is **214 nm or 220 nm**, with 254 nm used as a secondary wavelength for products containing aromatic residues.

## Peptide Content vs Purity

One of the most common points of confusion in peptide quality assessment is the distinction between purity and peptide content. These are independent measurements that answer different questions.

| Parameter | Question Answered | Method |
|-----------|------------------|--------|
| **HPLC Purity** | "How much of the peptide present is the target peptide?" | RP-HPLC, area normalization |
| **Peptide Content** | "How much of this powder is actually peptide?" | Amino acid analysis, nitrogen determination |

### Why the Distinction Matters

Consider a hypothetical batch of IGF-1 LR3:

| Measurement | Result |
|-------------|--------|
| HPLC Purity | 99.5% |
| Peptide Content | 87% |

In 10 mg of this lyophilized powder:

- **Actual target peptide** = 10 mg × 87% × 99.5% = **8.66 mg**
- **Other peptide impurities** (deletion sequences, truncated peptides) = 10 mg × 87% × 0.5% = 0.04 mg
- **Non-peptide mass** (TFA counter-ion + residual water) = 10 mg × 13% = **1.30 mg**

If only purity is considered (99.5%), one might assume they received 9.95 mg of target peptide — an overestimate of 15%.

### Counter-Ion Contributions

The primary counter-ion in TFA-based peptide purification is trifluoroacetate (CF<sub>3</sub>COO<sup>−</sup>, MW 113.0). Each basic residue (Lys, Arg, His, and the N-terminus) can carry one TFA counter-ion. For a peptide with 5 basic residues:

- Peptide MW: 2000 Da
- Total TFA: 5 × 113.0 = 565.0 Da
- TFA mass contribution: ~22% of total

This explains why peptide content for TFA-salt peptides typically ranges from 78% to 92%.

### Acetate Salt Exchange

PeptideSourceHub can provide peptides in acetate salt form upon request. Acetate (CH<sub>3</sub>COO<sup>−</sup>, MW 59.0) is lighter than TFA, resulting in higher peptide content for the same peptide:

| Salt Form | Counter-Ion MW | Typical Peptide Content |
|-----------|:---:|:---:|
| Trifluoroacetate (TFA) | 113.0 | 78–92% |
| Acetate | 59.0 | 85–96% |
| Hydrochloride | 35.5 | 90–97% |

## Questions to Ask Your Peptide Supplier

When evaluating a new supplier or verifying an existing one, the following questions help assess analytical capability and quality system maturity:

### About the COA

1. "Is this a batch-specific COA, or a template?"
2. "Can you provide the raw HPLC chromatogram data file (not just the printed report)?"
3. "Do you test every batch, or only representative batches from a synthesis campaign?"

### About HPLC Methodology

4. "What column dimensions and particle size are used?"
5. "What is your mobile phase composition and gradient program?"
6. "At which wavelength(s) is purity reported?"
7. "What is your system suitability criteria? Can you provide the blank injection?"

### About Mass Spectrometry

8. "Which ionization method and instrument are used?"
9. "Can you provide the full mass spectrum (not just the deconvoluted mass)?"
10. "Do you perform MS/MS sequence verification, and if so, can you provide the fragmentation data?"

### About Batch Quality

11. "What is the actual peptide content of this batch (not just HPLC purity)?"
12. "What is the residual TFA or counter-ion level?"
13. "Can you provide stability data or forced degradation data for this peptide?"

### About Traceability

14. "How do you link this COA to specific raw material lots and synthesis records?"
15. "If I re-order the same product, will the COA data be different? (It should be — batch-to-batch variation is expected.)"

A supplier who cannot answer these questions, or who provides evasive responses, may lack the analytical capability implied by their COA.

---

← [Quality Control Hub](index.md) | [HPLC Chromatography →](hplc-chromatography.md)
