---
title: "Mass Spectrometry Verification — PeptideSourceHub"
description: "Technical guide to mass spectrometry for peptide molecular weight confirmation. ESI-MS, MALDI-TOF comparison, spectrum interpretation, and MS/MS sequence verification."
---

# Mass Spectrometry for Peptide Verification

## Why Mass Spectrometry Matters

High-Performance Liquid Chromatography (HPLC) answers "how pure?" — but it does not answer "what is it?" A sample can display a single sharp peak at 99.5% purity and still be the wrong peptide. Mass spectrometry (MS) provides definitive molecular weight confirmation, ensuring the peptide's identity matches expectations.

At PeptideSourceHub, **every production batch undergoes both HPLC and MS analysis** before QC documentation is finalized. This dual verification is standard practice for research-grade peptide manufacturing.

## ESI-MS: The Standard for Peptide Analysis

Electrospray Ionization Mass Spectrometry (ESI-MS) is the most commonly used MS technique for peptide analysis. It operates by:

1. **Ionization**: The peptide solution is sprayed through a charged capillary, producing multiply-charged ions ([M+nH]ⁿ⁺)
2. **Mass Analysis**: Ions are separated by mass-to-charge ratio (m/z) in a quadrupole or time-of-flight (TOF) analyzer
3. **Deconvolution**: Software converts the charge-state envelope into a single zero-charge mass spectrum showing the molecular weight

### Expected Output

| Peptide MW Range | Typical Charge States | Expected Accuracy |
|---|---|---|
| 300–1,000 Da | +1, +2 | ±0.5 Da |
| 1,000–5,000 Da | +2, +3, +4 | ±1.0 Da |
| 5,000–25,000 Da | +4 to +15 | ±1.5 Da |

## Method Comparison: ESI vs MALDI-TOF

| Parameter | ESI-MS | MALDI-TOF |
|---|---|---|
| **Ionization** | Liquid-phase, electrospray | Solid-phase, laser desorption |
| **Typical Charge** | Multiply charged ions | Singly charged ions |
| **Mass Range** | Best for <30 kDa | Best for >10 kDa |
| **Sensitivity** | Excellent (fmol range) | Excellent (amol range) |
| **Common Use** | Routine peptide MW confirmation | High-throughput screening |
| **At PSH** | Every batch | On request for large peptides |

PeptideSourceHub uses ESI-MS as the standard release method for all catalog products. MALDI-TOF is available upon request for higher molecular weight products (e.g., HGH, ~22,125 Da).

## Interpreting a Mass Spectrum

### Key Features to Identify

1. **Parent Ion Peak**: The deconvoluted [M+H]⁺ peak — should match theoretical monoisotopic MW ± acceptable tolerance
2. **Adduct Peaks**: [M+Na]⁺ (+22 Da), [M+K]⁺ (+38 Da) — common in sodium/potassium-containing buffers
3. **Dimer Peaks**: [2M+H]⁺ at 2× MW — indicates aggregation at higher concentrations
4. **Fragment Peaks**: Low m/z signals — may indicate in-source fragmentation

### Common Adducts in Peptide Mass Spectra

| Ion | Mass Shift | Origin |
|---|---|---|
| [M+H]⁺ | +1.0078 Da | Primary ion — this is what you confirm against theoretical MW |
| [M+Na]⁺ | +22.9898 Da | Sodium from glassware, buffers, or solvents |
| [M+K]⁺ | +38.9637 Da | Potassium from buffers |
| [M+NH₄]⁺ | +18.0344 Da | Ammonium from buffers |
| [M+2Na-H]⁺ | +44.9718 Da | High sodium environment |

A clean mass spectrum shows the [M+H]⁺ peak dominating, with [M+Na]⁺ at ≤10% relative abundance. Excessive sodium adduction suggests incomplete desalting during workup.

## MS/MS: Sequence Verification

For high-value peptides or complex sequences, MS/MS (tandem mass spectrometry) provides sequence confirmation:

1. **Selection**: The parent ion is isolated in the first mass analyzer
2. **Fragmentation**: Collision-Induced Dissociation (CID) breaks the peptide at amide bonds
3. **Analysis**: The fragment ions (b-ions and y-ions) are analyzed, producing a sequence ladder

MS/MS is particularly valuable for:
- Verifying sequences over 20 amino acids
- Confirming modified residues (acetylation, amidation, fatty acid conjugation)
- Detecting deletion sequences at single-amino-acid resolution

## Questions to Ask Suppliers About Their MS Method

| Question | Why It Matters |
|---|---|
| What MS instrument and ionization method do you use? | ESI vs MALDI — different mass ranges and accuracy profiles |
| What is your mass accuracy specification? | Research-grade should be ±1.0 Da or better |
| Do you run MS on every batch, or only periodically? | Batch-specific MS is a key quality indicator |
| Can you provide the actual mass spectrum, not just the MW value? | Enables independent verification of peak identity |
| Do you also monitor for common impurities by MS? | Shows whether the supplier actively screens for incorrect sequences |
| Is MS/MS available for sequence verification? | Essential for complex peptides, modified sequences, or high-value orders |

## Related Resources

- [HPLC Chromatography Guide](hplc-chromatography.md)
- [COA & Purity Analysis](coa-purity-analysis.md)
- [Quality Control Framework](index.md)
- [Product Specifications](../specs/)
