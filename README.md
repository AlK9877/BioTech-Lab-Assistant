# 🧬 BioTech Lab Assistant | دستیار آزمایشگاه بیوتکنولوژی

**Live app:** https://alk9877.github.io/BioTech-Lab-Assistant/

BioTech Lab Assistant is a small, client-side educational web application for routine biotechnology calculations and basic DNA/RNA sequence review. It was developed after completing the **Web App Design for Biotechnologists with AI** course, with AI-assisted development used during the coding and refinement process.

> **Important:** This is an educational and planning tool. Laboratory reagent volumes, PCR conditions, ECL ratios, and other experimental settings must be checked against the specific kit instructions and laboratory protocol before use.

## Main modules

### 1. PCR Master Mix Calculator
- Calculates per-reaction and bulk volumes.
- Includes a configurable excess margin for pipetting loss.
- Uses an **example PCR composition**, not a universal PCR recipe.
- Requires a whole-number reaction count.

### 2. Western Blot ECL Substrate Calculator
- Estimates working solution from membrane surface area.
- Includes mini-gel, midi-gel, and custom membrane sizes.
- Includes 1:1 and 40:1 reagent-ratio presets.
- Ratio presets are clearly marked as values that must be verified against the kit instructions.
- Requires a whole-number membrane count.

### 3. Dilution & Molarity Converter
- Solves `C1V1 = C2V2` for routine stock dilutions.
- Supports M, mM, µM, and nM.
- Supports L, mL, and µL.
- Calculates required solute mass from concentration, volume, and molecular weight.

### 4. DNA/RNA Sequence Tool
- Accepts a raw sequence or **one FASTA record at a time**.
- Detects DNA versus RNA and keeps RNA as RNA instead of converting `U` to `T`.
- Rejects mixed `T/U` input.
- Calculates sequence length and canonical-base GC and AT/AU percentages.
- Produces the correct DNA or RNA reverse complement.
- Provides frame-1 protein translation.
- Supports IUPAC ambiguity codes for sequence handling and reverse complement.
- Shows **N/A** for basic Tm and MW estimates when the input is RNA or contains ambiguity codes.
- Labels Tm as an **estimated** value.

### 5. Lab Sheet Export
- Word document (`.docx`)
- Excel-compatible HTML file (`.xls`)
- CSV (`.csv`)
- Plain text (`.txt`)

The `.xls` option is an Excel-compatible HTML table saved with an `.xls` extension; it is not a native binary Excel workbook.

### 6. Languages
- English
- فارسی (RTL)
- Deutsch

## Technical structure

The application is a **single-file client-side web app** (`index.html`) with no backend or database. It uses CDN-hosted frontend dependencies, including Bootstrap, Bootstrap Icons, Google Fonts, and JSZip. Because of these CDN resources, a network connection is required for all styling and export features to load reliably unless the resources are already cached.

## Sequence calculation notes

The Tm result is a basic empirical estimate for canonical DNA oligos. Actual oligonucleotide Tm depends on reaction conditions such as Mg²⁺, salt, dNTP concentration, and oligo concentration. For experimental primer design, use a dedicated oligo-analysis tool and the conditions of your PCR system.

The ssDNA MW estimate uses base-specific nucleotide masses for an unmodified DNA oligo. Modified oligos, phosphorylated ends, RNA, and ambiguity codes require a more specific calculation.

## References used for calculation checks

- IDT OligoAnalyzer and oligonucleotide guidance: https://www.idtdna.com/pages/tools/oligoanalyzer
- IDT molecular-weight guidance: https://www.idtdna.com/pages/support/faqs/how-do-i-calculate-the-molecular-weight-of-an-oligo-
- Thermo Fisher DNA/RNA molecular-weight reference: https://www.thermofisher.com/fr/en/home/references/ambion-tech-support/rna-tools-and-calculators/dna-and-rna-molecular-weights-and-conversions.html

## Run locally

1. Download `index.html`.
2. Open it in a modern browser.
3. Keep an internet connection available so the CDN resources can load.

## Deploy with GitHub Pages

1. Upload `index.html` to the repository root.
2. Open **Settings → Pages**.
3. Select the `main` branch and root (`/`).
4. Save the Pages settings.

## About the project

This project was created as a practical learning project after participating in a course on web-app development for biotechnologists with AI. The goal was to combine basic web development with common biotechnology calculations and simple sequence-analysis tasks in one accessible interface.

**GitHub:** https://github.com/AlK9877
