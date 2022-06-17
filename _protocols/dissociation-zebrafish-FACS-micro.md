---
title: "dissociation-zebrafish-FACS-micro"
---

Date : 2022-06-16

Author : V Chong-Morrison

# Dissociation of zebrafish larvae for FACS - micro version for bulk/plate-based single cell applications

## Introduction
This protocol has been tested on dissected neuroepithelium tissue (aiming for pineal organ) of 32-36 hpf larvae to FAC-sort GFP+ pineal cells with a 100 µm
nozzle. For negative gating, ~20 whole wild type embryos is usually sufficient.

## Materials
- RNase-free pipette tips and micro-centrifuge tubes, low-binding/retention grade, for cell work **Eppendorf Protein LoBind**
- RNase-free pipette tips and micro-centrifuge tubes, normal retention i.e. not low-binding, for buffers and reagents
- 40 µm cell strainers (**22363547, FisherScientific**change)
- 12x75 mm 5 ml polystyrene sterile round tubes with snap cap (734-0436, Falcon)
- DNaseI (10104159001, Sigma-Aldrich)
- Papain, 10 mg/ml i.e. 0.3 U/µl (10108014001, Sigma-Aldrich)
- ROCK inhibitor a.k.a. Y-27632 dihydrochloride (A3008, Generon UK)
- 10X HBSS, no calcium, no magnesium, no phenol red (14185052, ThermoFisher)
- Bovine Serum Albumin, heat shock fraction, protease free, essentially globulin free, pH 7, >=98% (A3059, Sigma-Aldrich)
- 1M HEPES solution (15630056, ThermoFisher)
- eBioscience Fixable Viability Dye eFluor 780 (65-0865-14, ThermoFisher)

## Procedure

### Pre-flight

Ensure following reagents are prepared in advance and stored appropriately.

- ROCK inhibitor; resuspend 10mg with 1 ml of DMSO to concentration of 10 mg/ml. Store in -20C.
- DNaseI; resuspend 50mg/100mg with 5 ml/10ml of nuclease-free water to final concentration of 10 mg/ml. Filter sterilise (0.22 µm) and store 1 ml aliquots at 4C for couple of days or -20C for long-term.
- eFluor 780 dye; dilute a small aliquot 1 in 10 with DMSO and store at -20C. Neat stock should be stored in -80C for long-term.
- Autoclave MilliQ DEPC water for making buffers and solutions, or use commercial UltraPure DNase/RNase-free distilled water.

### Prep

1. Prepare Hank's solution (blocking isotonic solution for one sample. Always have a negative sample for FACS gating!).

    **Hank's solution**

    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | 10X HBSS   | 1.2 ml      | 1X |
    | BSA        | 0.03 g      | 2.5 mg/ml |
    | 1M HEPES   | 120 µl      | 10 mM |
    | Water      | up to 12 ml | - |
    ||||

2. Filter-sterilise (0.22 µm) into a Falcon tube. This will now be used to make up the next two solutions (Dissociation and Dissociation STOP).
3. **Bulk cell applications.** Prepare normal i.e. not low-binding micro-centrifuge tubes containing 100 µl Hank's solution for cells collection. Place on ice.

### Steps

1. Set heat-block to 37C. Cool large centrifuge down to 4C.
2. If required, anaesthetise larvae and dissect tissues in an agar-bottomed Petri dish filled with ~10 mL filtered Hank's. 
3. Using a glass Pasteur pipette, collect tissue into low-binding micro-centrifuge tube pre-filled with 10 µl filtered Hank's and kept cool on ice.
4. Collect tissue within 30 minutes to maximise viability.
5. Top up to 250 µl with filtered Hank's.
6. Add 20 µl Papain, 0.3 µl ROCK Inhibitor and 30 µl DNaseI to commence dissociation.

    **Dissociation reaction**

    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | Papain           | 20 µl  | 0.02 U/µl |
    | ROCK inhibitor   | 0.3 µl | 10 µg/ml |
    | DNaseI           | 30 µl  | 1 mg/ml |
    | Hank's (filtered)| up to 300 µl | - |
    ||||

7. Incubate at 37C. Every 5 minutes, triturate sample 20 times in solution against the tube wall using a p200 low-binding tip. *Tip: Pre-coat the tip with filtered Hank's before triturating.*
8. Repeat step 4 until sample is dissociated i.e. no pieces of tissue left.
9. Stop dissociation by adding 600 µl filtered Hank's.
10. Place a 40 µm cell strainer into a fresh low-binding micro-centrifuge tube.
11. Pre-coat a P1000 tip with filtered Hank's before gently resuspending the cell suspension and transfer onto the cell strainer.
12. With cell strainer still attached, centrifuge at 500 g/rcf at 4C for 5 minutes.
11. Discard cell strainer and gently remove supernatant until approximately 500 µl remain.
12. Add 0.2 ul of 1:10 diluted eFluor 780 dye.
13. Resuspend the cell pellet gently using a fresh pre-coated low-binding tip and transfer to a 5 ml polystyrene round tube. 
14. Place on ice and proceed with FACS (about 30 minutes to sort entire sample).
15. **Bulk cell applications.** After FACS, pellet collected cells 500 g/rcf at 4C for 5 minutes in cooled tabletop micro-centrifuge.
16. **Bulk cell applications.** Very carefully, remove the supernatant and proceed with downstream applications.

### Appendix

#### Examples of downstream applications

- RNA extraction - resuspend pelleted cells in 100 µl Lysis Buffer (Ambion RNAqueous Micro-kit) and proceed with RNA extraction.
- ATAC-seq - protocol available separately (to be written up).

#### Evaluating dissociations

If desired, success of dissociations can be evaluated in trial runs using Trypan Blue viable cell counting with a haemocytometer. A quick Internet search will bring up several standard protocols. Here is an [example](https://www.thermofisher.com/uk/en/home/references/gibco-cell-culture-basics/cell-culture-protocols/trypan-blue-exclusion.html).

#### Protocol adjustments for different stages/tissue

Ensure the amount of tissue is roughly the same as the protocol. The drawback to this approach is that the older the embryos, the fewer you can fit in - if the target population is not a rare cell type this may not be a problem.

For younger embryos, the protocol remains the same. However, if younger than ~bud stage, a deyolking step may be needed prior to dissociation as excess
yolk may inhibit enzyme (papain) activity.