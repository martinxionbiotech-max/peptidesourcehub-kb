---
title: HPLC Chromatography for Peptide Analysis — PeptideSourceHub
description: Technical guide to high-performance liquid chromatography for peptide purity analysis. Covers reverse-phase methodology, peak interpretation, impurity types, and supplier evaluation.
---

# HPLC Chromatography for Peptide Analysis

## What HPLC Measures

High-Performance Liquid Chromatography (HPLC) is the primary analytical technique for determining peptide purity. It works by separating components of a mixture based on their differential interaction with a stationary phase (the column) and a mobile phase (the solvent system). The detector output — a chromatogram — plots absorbance (signal intensity) against retention time.

For peptides, HPLC answers two key questions:

1. **How many components** are present in the sample? (number of peaks)
2. **What is the relative abundance** of each component? (peak area percentages)

At PeptideSourceHub, every production batch undergoes both analytical HPLC (for purity determination) and preparative HPLC (for purification at scale).

## Reverse-Phase HPLC Methodology

### Principle of Separation

Reverse-phase HPLC separates peptides based on **hydrophobicity**. The stationary phase (C18 alkyl chains bonded to silica) is hydrophobic, while the mobile phase is polar (water-based). Peptides with more hydrophobic residues (Leu, Ile, Val, Phe, Trp) interact more strongly with the stationary phase and elute later (higher retention time). Hydrophilic peptides elute earlier.

### Standard Method at PeptideSourceHub

| Parameter | Specification |
|-----------|--------------|
| **Column** | C18, 4.6 mm × 150 mm or 4.6 mm × 250 mm |
| **Particle Size** | 5 µm (analytical); 3 µm or 3.5 µm for higher resolution |
| **Pore Size** | 100 Å or 300 Å (300 Å preferred for peptides >2 kDa) |
| **Mobile Phase A** | Water + 0.1% (v/v) Trifluoroacetic Acid (TFA) |
| **Mobile Phase B** | Acetonitrile + 0.1% (v/v) TFA |
| **Gradient** | Typically 5% B to 95% B over 20–30 minutes |
| **Flow Rate** | 1.0 mL/min (4.6 mm ID column) |
| **Column Temperature** | 25°C or 40°C (method-dependent) |
| **Injection Volume** | 5–20 µL |
| **Detection Wavelength** | 214 nm or 220 nm (primary); 254 nm (secondary) |
| **Sample Concentration** | ~1.0 mg/mL in water or mobile phase |

### Role of Trifluoroacetic Acid (TFA)

TFA serves as an **ion-pairing agent** in the mobile phase:

- At low pH (~2), TFA protonates basic residues (Lys, Arg, His, N-terminus) and pairs with them
- This suppresses ionic interactions with residual silanol groups on the silica
- Result: sharper peaks, better resolution, and improved reproducibility

Without TFA (or an alternative ion-pairing agent), peptides with basic residues exhibit peak tailing and poor resolution.

### Why Acetonitrile (ACN)?

Acetonitrile is the organic modifier of choice for peptide HPLC because:

- **Low UV cutoff** (190 nm) — does not interfere with peptide bond detection at 214/220 nm
- **Low viscosity** — reduces column backpressure
- **High elution strength** — effectively displaces peptides from the C18 stationary phase

Methanol is an alternative but has higher UV absorbance at low wavelengths and higher viscosity, making ACN the preferred organic modifier for peptide analysis.

## Detection Wavelength Selection

The peptide bond (amide chromophore) absorbs strongly at approximately 190–220 nm. Detection at 214 nm or 220 nm is the standard for peptide analysis because:

1. Every peptide residue contains a peptide bond — universal detection
2. Impurities that are peptide-based (deletion sequences, truncated peptides) are detected with similar sensitivity
3. Sensitivity is high: typical LOD (limit of detection) ~0.01–0.05% of main peak

### Multi-Wavelength Detection Strategy

| Wavelength | Chromophore Detected | Sensitivity | Coverage |
|------------|---------------------|-------------|----------|
| **214 nm** | Peptide bond (amide) | High | All peptides and peptide-based impurities |
| **220 nm** | Peptide bond (amide) | High | Similar to 214 nm; slightly less TFA baseline interference |
| **254 nm** | Aromatic rings (Trp, Tyr, Phe) | Moderate | Only aromatic-containing species |
| **280 nm** | Trp, Tyr | Low–moderate | Selective for Trp/Tyr-containing species |

At PeptideSourceHub, purity is reported at **214 nm or 220 nm** (primary). If 254 nm is used as the sole detection wavelength, non-aromatic impurities may be missed — this is considered a significant analytical gap.

> **Supplier evaluation tip:** If a supplier reports purity at 280 nm only, ask for the 214/220 nm chromatogram. A 280 nm-only method will systematically under-report impurities in peptides lacking aromatic residues.

## Interpreting Peak Area Percentages

### The Area Normalization Method

Peptide purity by HPLC is almost universally reported as area percent:

$$\\text{Purity}_{\\text{Area\\%}} = \\frac{A_{\\text{main}}}{\\sum A_i} \\times 100$$

Where *A*<sub>main</sub> is the area of the target peptide peak and ∑*A<sub>i</sub>* is the sum of all integrated peak areas (excluding solvent front and system peaks).

### Assumptions and Limitations

The area normalization method assumes **equal response factors** for all components. This assumption is:

| Assumption | Validity |
|------------|----------|
| Peptide-based impurities (deletion sequences, truncations) have similar extinction coefficients at 214/220 nm | ✅ Generally valid — same amide backbone |
| Non-peptide impurities (solvents, salts) have similar UV response | ⚠️ May not be valid — these may not absorb at all at 214 nm |
| Modified peptides (oxidation, deamidation) have similar response | ✅ Generally valid for common modifications |
| Aggregates are detected equivalently | ❌ Aggregates may not elute from the column |

This limitation is why PeptideSourceHub supplements HPLC with mass spectrometry and, for critical applications, peptide content determination by amino acid analysis — providing orthogonal verification that HPLC data is not misleading.

### Typical Chromatogram Profile at ≥99% Purity

A typical ≥99% pure peptide chromatogram shows:

| Feature | Expected Observation |
|---------|---------------------|
| Main peak area | ≥99.0% of total integrated area |
| Number of impurity peaks | 1–3 (rarely more at this purity level) |
| Largest single impurity | Typically <0.5% |
| Main peak symmetry (USP tailing factor) | 0.8–1.3 |
| Baseline noise | <0.1 mAU |
| Solvent/void peak | Small peak at RT ~1–3 min (expected) |

## Common Impurity Types

Understanding what impurities appear in a peptide chromatogram — and why — is essential for evaluating purification quality.

### Synthesis-Related Impurities

| Impurity Type | Description | HPLC Behavior | Typical Abundance |
|--------------|-------------|---------------|:---:|
| **Deletion sequences** | Peptides missing one or more residues from incomplete coupling | Earlier elution (less hydrophobic) or co-elution | <0.5% per deletion |
| **Truncation products** | Terminated sequences from incomplete deprotection or capping failure | Variable; often earlier elution | <0.3% |
| **Diastereomers** | Racemized residues from coupling activation | Near co-elution with target (challenging to separate) | <0.1% (per racemized residue) |
| **Insertion sequences** | Double couplings | Later elution (more hydrophobic) | <0.1% |
| **Incomplete deprotection** | Residual protecting groups | Variable; aromatic protecting groups absorb strongly at 254 nm | <0.2% |

### Degradation-Related Impurities

| Impurity Type | Description | HPLC Behavior | Typical Abundance |
|--------------|-------------|---------------|:---:|
| **Oxidation products** | Oxidized Met (sulfoxide/sulfone), oxidized Cys, oxidized Trp | Earlier elution (more polar) | <0.5% |
| **Deamidation** | Asn/Gln conversion to Asp/Glu | Slightly earlier elution at acidic pH | <0.2% |
| **Aggregates** | Non-covalent dimers/oligomers | Later elution or may not elute (column-bound) | <0.1% (detectable) |
| **Aspartimide formation** | Asp-Gly/Asp-Ser sequences | Slightly different RT; may appear as double peak | <0.1% |
| **β-Elimination** | Disulfide-bonded Cys degradation at alkaline pH | Additional peaks | <0.2% |

### Processing-Related Impurities

| Impurity Type | Description | Detection |
|--------------|-------------|-----------|
| **Residual TFA** | From mobile phase; remains as counter-ion | Not detected by UV at 214 nm (no chromophore) |
| **Residual scavengers** | EDT, thioanisole from cleavage cocktail | Detectable at 254 nm if aromatic |
| **Column bleed** | Stationary phase degradation products | Baseline drift, ghost peaks |

## System Suitability

Before any analytical HPLC run is accepted for purity reporting, the PeptideSourceHub QC laboratory verifies system suitability:

| Parameter | Acceptance Criteria | Purpose |
|-----------|---------------------|---------|
| **Blank injection** | No peaks >0.05% of typical main peak area | Confirms system is clean (no carryover, ghost peaks) |
| **Retention time reproducibility** | RSD ≤1% (n=3 injections) | Confirms pump and column stability |
| **Peak area reproducibility** | RSD ≤2% (n=3 injections) | Confirms injection precision |
| **Theoretical plates (N)** | ≥5,000 for main peak (4.6 mm × 150 mm column) | Confirms column efficiency |
| **USP tailing factor (T)** | 0.8–1.5 for main peak | Confirms acceptable peak shape |
| **Resolution (Rs)** | ≥1.5 between closest critical pair | Confirms adequate separation |

### USP Tailing Factor

The tailing factor quantifies peak asymmetry:

$$T = \\frac{W_{0.05}}{2f}$$

Where *W*<sub>0.05</sub> is the peak width at 5% of peak height, and *f* is the distance from the peak front to the apex at 5% height.

| Tailing Factor | Interpretation |
|:---:|---|
| **0.9–1.1** | Excellent — symmetrical peak, good column performance |
| **1.1–1.3** | Acceptable — slight tailing, common for basic peptides |
| **1.3–1.5** | Borderline — moderate tailing; may affect integration accuracy |
| **>1.5** | Unacceptable — significant tailing; column or method issue |
| **<0.8** | Fronting — unusual for peptides; check injection solvent |

### Theoretical Plates (Column Efficiency)

Theoretical plates are calculated from the peak:

$$N = 16 \\left(\\frac{t_R}{W}\\right)^2$$

Where *t<sub>R</sub>* is retention time and *W* is the baseline peak width. Higher plate counts indicate sharper, narrower peaks and better resolution.

| Column Type | Typical N (150 mm) |
|-------------|:---:|
| 5 µm C18 | 5,000–10,000 |
| 3.5 µm C18 | 8,000–15,000 |
| 3 µm C18 | 10,000–18,000 |
| Sub-2 µm (UHPLC) | 15,000–30,000 |

## Purification Methodology

PeptideSourceHub uses preparative HPLC for purification at scale, following the same basic principles as analytical HPLC:

| Parameter | Analytical HPLC | Preparative HPLC |
|-----------|:---:|:---:|
| **Purpose** | Purity measurement | Purification (fractionation) |
| **Column ID** | 4.6 mm | 21.2 mm, 30 mm, or 50 mm |
| **Flow Rate** | 1.0 mL/min | 20–80 mL/min |
| **Sample Load** | 5–20 µg | 50–500 mg |
| **Detection** | UV at 214/220 nm | UV at 214/220 nm with fraction collector |

Crude peptide (~70–90% purity depending on sequence) is dissolved, loaded onto the preparative column, and eluted with the same ACN/water/TFA gradient system. Fractions containing the target peptide (identified by retention time) are pooled, analyzed by analytical HPLC, and — if ≥99% purity — advanced to lyophilization.

For products requiring >99.5% purity, a second preparative HPLC step with a modified gradient (shallower slope in the target elution region) may be employed to resolve closely eluting impurities.

## Questions to Ask Your Supplier About HPLC

| Question | What the Answer Reveals |
|----------|------------------------|
| "What column and dimensions are used for purity testing?" | Resolution capability; 4.6 mm × 150 mm or 250 mm is standard |
| "What particle size and pore size?" | 5 µm is standard; 300 Å pore recommended for peptides >2 kDa |
| "What is the mobile phase composition?" | TFA/ACN system is standard; alternative systems (formic acid, ammonium acetate) may affect selectivity |
| "What gradient program is used?" | Steep gradients reduce resolution; 20–30 min gradients are typical for analytical HPLC |
| "At what wavelength(s) is purity reported?" | 214/220 nm should be primary; single-wavelength at 280 nm is insufficient |
| "Can you provide the blank injection chromatogram?" | Reveals system contamination, carryover |
| "What is the system suitability criteria?" | Demonstrates method validation |
| "Is purity reported by area normalization or external standard?" | Area normalization is standard for peptides; external standard calibration is unusual for purity |
| "How many injections per sample?" | At minimum, duplicate injections; single injection is insufficient |
| "What is your integration parameter for peak threshold?" | Too high a threshold may miss small impurities |
| "Can you provide the raw data file?" | Allows independent verification; PDF reports can be edited |

---

← [COA & Purity Analysis](coa-purity-analysis.md) | [Mass Spectrometry →](mass-spectrometry.md)
