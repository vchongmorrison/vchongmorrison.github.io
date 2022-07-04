---
title: "atacseq-FACS"
---

Date : 2022-07-04

Author : V Chong-Morrison

# Preparation of ATAC-seq libraries from FACS samples

## Introduction
This protocol has been tested on 14,000 (see note) FAC-sorted cells (BD Fusion).

*Note: As guidance only, unlikely to be an accurate number which is typical for most sorters - based on experience the no. of events for most sorters overestimate ~50% of 'true' cell number.*

## Materials
- Pipette tips, low-binding/retention grade, for cell work
- Micro-centrifuge tubes, normal retention i.e. not low-binding, for buffers and reagents
- DNA LoBind® tubes, 1.5 ml (0030108051, Eppendorf)
- Tabletop micro-centrifuge, cooled to 4C
- Heatblock, set to 37C
- Thermal cycler
- Magnetic rack for microcentrifuge tubes
- 1X PBS
- 1M Tris-HCl pH 7.4
- 5M NaCl
- 1M MgCl2
- 10% NP40 a.k.a. Igepal CA-630
- EtOH, molecular biology grade
- TE buffer, molecular biology grade
- Any suitable PCR purification kit e.g. NEB Monarch, Qiagen PCR Purification MinElute, Zymo Research DNA Clean & Concentrator-5
- TapeStation D1000 reagents, normal or high sensitivity (or Bioanalyzer equivalent) (5067-5582 and 5067-5583, Agilent)
- Tagment DNA TDE1 Enzyme and Buffer Kit (20034197 or 20034198, Illumina)
- NEBNext® Q5® Hot Start HiFi PCR Master Mix (or suitable alternative) (M0543, New England Biolabs)
- AMPure XP for PCR Purification (A63880, Beckman-Coulter)
- Nextera or Buenrostro et al. primers (see Appendix below)

## Procedure

### Pre-flight

Ensure ATAC reagents are prepared. Place PBS, NaCl, MgCl2, NP40 and EtOH on ice to cool.

### Prep

1. Prepare Cell Lysis Buffer on ice.

   **Cell Lysis Buffer**

   | Component | Volume/amount | Final conc. |
   | :---------- |:----------:| ----------:|
   | 1M Tris-HCl pH 7.5   | 10 µl      | 10 mM |
   | 5M NaCl        | 2 µl      | 10 mM |
   | 1M MgCl2   | 3 µl      | 3 mM |
   | 10% NP40      | 1 µl | 0.1% |
   | Nuclease-free water      | up to 1 ml | - |
   ||||
    
2. FACS population-of-interest into normal retention tubes containing 100 µl filtered Hank's.

### Steps - Tn5 transposition

1. Set heat-block to 37C. Cool tabletop micro-centrifuge down to 4C.
2. If desired and there is sufficient material, split collected cells equally to obtain two replicates.
3. Pellet collected cells at 500 g/rcf at 4C for 5 minutes in cooled tabletop micro-centrifuge.
4. Carefully remove Hank's without disturbing the cell pellet (can be challenging to see).
5. Add 50 µl cold 1X PBS by pipetting gently against the opposite wall where the cell pellet would be.
6. Centrifuge 500 g/rcf at 4C for 5 minutes in cooled tabletop micro-centrifuge.
7. Carefully remove PBS and add 50 µl cold Cell Lysis Buffer.
8. Gently pipette 3-5 times to resuspend the cell pellet.
9. Centrifuge 500 g/rcf at 4C for 10 minutes in cooled tabletop micro-centrifuge.
10. Carefully remove supernatant and set the nuclei pellet on ice.
11. Proceed immediately to Tn5 transposition.
    
    **Tn5 transposition**
    
    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | Nuclease free water   | 9 µl | - |
    | 2X TD Buffer      | 10 µl | 1X |
    | TDE1 Enzyme   |  1 µl | - |
    | Total      | 20 µl | - |
    ||||
    
13. Pipette up and down to mix, then transfer reactions into fresh DNA LoBind® tubes.
14. Incubate at 37C for 30 minutes.
15. STOP transposition by purifying the reactions using a suitable PCR purification kit, eluting the transposed DNA in 10 µl of buffer.
16. Store purified DNA in -20C or proceed with PCR amplification to generate ATACseq libraries.

### Steps - PCR amplification and indexing of libraries

1. In PCR tubes, combine the following.

   **PCR amplification, indexing**

   | Component | Volume/amount | Final conc. |
   | :---------- |:----------:| ----------:|
   | Purified DNA | 10 µl | - |
   | Nuclease free water | 10 µl | - |
   | Universal primer, 10 µM   |  2.5 µl | 0.5 µM |
   | Index primer, 10 µM      | 2.5 µl | 0.5 µM |
   | NEBNext® Q5® Hot Start HiFi PCR Master Mix      | 25 µl | 1X |
   | Total      | 50 µl | - |
   ||||

2. Run the following cycling programme (adjust accordingly if substituting polymerase). Adjust number of cycles if using lower/higher number of cells.

   **Thermal cycling**

   | Temperature | Time | Cycles |
   | :---------- |:----------:| ----------:|
   | 72C | 5 mins | - |
   | 98C | 30 secs | - |
   | 98C |  10 secs | 13 |
   | 65C | 75 secs | 13 |
   | 65C | 5 mins | - |
   | 10C | Hold | - |
   ||||
        
### Steps - Purification of amplified libraries

1. Equilibrate AMPure beads to RT (e.g. while PCR is running) and prepare 80% EtOH (500 µl per library).
2. Vortex beads thoroughly to resuspend.
3. In a DNA LoBind® tube, combine 50 µl of resuspended beads with the 50 µl PCR reaction.
4. Pipette up and down smoothly until well-mixed.
5. Incubate at RT for 5 mins.
6. Pulse spin and place on magnetic rack for 5 minutes until the solution is clear.
7. Carefully remove and discard the supernatant without touching the beads (with DNA bound to them).
8. With the tubes still on the magnetic rack, gently add 200 µl of 80% EtOH against the opposite wall to the beads.
9. Leave for 30 secs then gently remove EtOH.
10. Repeat steps 8-9.
11. With the tube still on the magnetic rack, air dry the beads with lids open for maximum 10 minutes. *Tip: Observe the drying process, beads will go from wet to ‘shiny’ to ‘cracked river bed’.  Do NOT allow to dry to ‘cracked river bed’. Aim for ‘not shiny, dry’.*
12. Remove tube from the magnetic rack, and elute DNA by adding 20 µl 0.1X TE buffer to the beads.
13. Pipette up and down gently until beads are thoroughly resuspended in the TE buffer.
14. Pulse spin, then place on magnetic rack for 5 minutes until the solution is clear.
15. Carefully remove the supernatant into a fresh DNA LoBind® tube - this is your final ATACseq library.
16. Store in -20C.

### Steps - Library QC, quantification and NGS.

1. Assess the success of the experiment using Agilent TapeStation D1000 (regular or high sensitivity) or Bioanalyzer equivalent. Transposition is deemed successful if a periodic set of peaks (~150bp, 300 bp, 450 bp…) can be detected indicative of mono-, di-, tri-… nucleosomes.
2. For accurate quantification of libraries prior to NGS, quantify using a suitable qPCR-based library quantification kit for Illumina (e.g. KAPA Biosystems, NEB) by testing 1:2000, 1:5000 and 1:10,000 dilutions of the library and taking the mean concentration as final result.
3. Sequence the libraries to obtain paired-end reads at least 50 bp in length (e.g. 2x75bp).

### Appendix

Sequences from Buenrostro et al. 2013 can be ordered as oligos from usual provider (more economical) - they correspond to Illumina Nextera primers up to N712 (Ad2.1 = N701, Ad2.2 = N702…..Ad2.12 = N712) only. 

Refer to **Supplementary Table 1: Oligo designs. A list of ATAC-seq oligos used for PCR** from:

*[Buenrostro, J., Giresi, P., Zaba, L. et al. Transposition of native chromatin for fast and sensitive epigenomic profiling of open chromatin, DNA-binding proteins and nucleosome position. Nat Methods 10, 1213–1218 (2013)](https://doi.org/10.1038/nmeth.2688)*
