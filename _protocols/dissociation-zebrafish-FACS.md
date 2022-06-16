---
title: "dissociation-zebrafish-FACS"
---

Date : 2022-06-15

Author : V Chong-Morrison

# Dissociation of zebrafish larvae for FACS

## Introduction
This protocol has been tested on dissected heads/trunks and whole 30 hpf larvae to FAC-sort pineal cells (~40 cells per embryo, >80% viability) with a 100 µm
nozzle. For negative gating, ~20 whole wild type embryos is usually sufficient.

## Materials
- RNase-free pipette tips and micro-centrifuge tubes, low-binding/retention grade, for cell work
- RNase-free pipette tips and micro-centrifuge tubes, normal retention i.e. not low-binding, for buffers and reagents
- Glass serological pipettes
- 50 ml RNase-free Falcon tubes
- 40 µm cell strainers (22363547, FisherScientific)
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

1. Prepare Hank's solution (blocking isotonic solution for two samples - one experimental, one negative. Always have a negative sample for FACS gating!).

    **Hank's solution**

    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | 10X HBSS   | 1.2 ml      | 1X |
    | BSA        | 0.03 g      | 2.5 mg/ml |
    | 1M HEPES   | 120 µl      | 10 mM |
    | Water      | up to 12 ml | - |
    ||||

2. Filter-sterilise (0.22 µm) into a Falcon tube. This will now be used to make up the next two solutions (Dissociation and Dissociation STOP).
3. Prepare Dissociation solution (600 µl per sample of up to 50 whole embryos or 200 dissected heads/trunks ), in a normal Eppendorf tube is fine.

    **Dissociation solution**

    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | Papain           | 40 µl  | 0.02 U/µl |
    | ROCK inhibitor   | 0.6 µl | 10 µg/ml |
    | DNaseI           | 60 µl  | 1 mg/ml |
    | Hank's (filtered)| 500 µl | - |
    ||||

4. Prepare Dissociation STOP solution in one Falcon tube . Then, split it up so that there is 4 ml in a Falcon tube per sample).

    **Dissociation STOP solution**

    | Component | Volume/amount | Final conc. |
    | :---------- |:----------:| ----------:|
    | ROCK inhibitor   | 4 µl | 10 µg/ml |
    | DNaseI           | 400 µl  | 1 mg/ml |
    | Hank's (filtered)| 3596 µl | - |
    ||||

5a. **Bulk cell applications.** Prepare normal i.e. not low-binding micro-centrifuge tubes containing 200 µl Hank's solution + 0.2 µl ROCK inhibitor for cells collection. Place on ice. *Note : Can split into two tubes of 100 µl each, if collecting more than one tube of cells.*

5b. **Single cell applications.** Pipette input volume (e.g. 43 µl for 10X Genomics Single Cell 3’ v3.1) of nuclease-free water into a normal i.e. not low-binding micro-centrifuge tube. Pulse-spin, then mark the level with a fine marker. Remove all the water, then pipette 2 µl filtered Hank’s solution, ready for cells collection.

### Steps

1. If required, anaesthetise larvae and dissect tissues into glass dish placed on ice containing 1 to 2 ml filtered Hank's solution. Collect samples within 30 minutes to maximise viability.

    *Tip : Dissect 10 at a time in Petri dish, transfer with glass pipette and mark somewhere to help keep count.*

2. Set heat-block to 37C. Cool large centrifuge down to 4C.
3. Collect tissue into low-binding micro-centrifuge tube, and remove as much of Hank's solution as possible. Add Dissociation solution.
4. Incubate at 37C. Every 5 minutes, triturate sample 20 times in solution against the tube wall using a p200 low-binding tip.
5. Repeat step 4 until sample is dissociated i.e. no pieces of tissue left - this can take up to 20 minutes.
6. If not done already, prepare 50 ml Falcon tubes each containing 4 ml of Dissociation STOP solution for the required number of samples.
7. Stop dissociation reaction by collecting the dissociated sample into prepared Dissociation STOP solution.
8. For every sample, place a 40 µm cell strainer into a clean 50 ml Falcon tube.
9. Triturate sample gently (avoid bubbles!) against wall of Falcon tube ~10 times using a glass serological pipette.
10. Using the same glass serological pipette, collect the sample and pipette slowly onto the 40 µm cell strainer readily-placed onto its Falcon tube.
11. With cell strainers still attached, centrifuge at 500 g/rcf at 4C for 7 minutes.
12. Carefully lift the tubes out and discard cell strainer. Remove supernatant (slowly!) until approximately 500 µl is left - an estimate is fine.
13. Add 0.2 ul of 1:10 diluted eFluor 780 dye.
14. Resuspend the cell pellet gently using a fresh low-binding tip and transfer to a 5 ml polystyrene round tube. Place on ice and proceed with FACS (about 30 minutes to sort entire sample).
15. After FACS, pellet collected cells by at 500 g/rcf at 4C for 5 minutes in cooled tabletop micro-centrifuge.

    **Single Cell applications.** If volume of cells post-FACS does not exceed the level marked, step 15 can be skipped. Top-up the cell suspension with filtered Hank’s to the mark and proceed immediately with downstream processing.

16. Very carefully, remove the supernatant and proceed with downstream applications.

    **Single Cell applications.** If volume of cells post-FACS exceeds the level marked, remove supernatant to the mark. Gently resuspend the pelleted cells with a low-binding tip, place on ice, and proceed immediately with downstream processing.

### Appendix

#### Examples of downstream applications

- RNA extraction - resuspend pelleted cells in 100 µl Lysis Buffer (Ambion RNAqueous Micro-kit) and proceed with RNA extraction.
- ATAC-seq - protocol available separately (to be written up).

#### Evaluating dissociations

If desired, success of dissociations can be evaluated in trial runs using Trypan Blue viable cell counting with a haemocytometer. A quick Internet search will bring up several standard protocols. Here is an [example](https://www.thermofisher.com/uk/en/home/references/gibco-cell-culture-basics/cell-culture-protocols/trypan-blue-exclusion.html).

#### Protocol adjustments for different stages/tissue

The two main parameters that should be considered are physical dissociation (i.e. trituration every 5 minutes until no pieces left) and volume of Dissociation solution. This is a bit tricky for later stage/more robust and bigger tissue. Trituration may take longer but you do not want this to take too long i.e. ≥30 mins as opposed to ~20 mins, as viability will decrease significantly. To balance this, you need to scale up the Dissociation solution so that there is an excess (of papain)
e.g. using 1 mL instead of 600 µL. Alternatively, the Dissociation solution can remain at 600 µL but ensure the amount of tissue is roughly the same as the
protocol. The drawback to this approach is that the older the embryos, the fewer you can fit in - if the target population is not a rare cell type this may not be a
problem.

For younger embryos, the protocol remains the same. However, if younger than ~bud stage, a deyolking step may be needed prior to dissociation as excess
yolk may inhibit enzyme (papain) activity.
