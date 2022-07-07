---
title: "guide-pool-microinjections"
---

Date : 2022-06-16

Author : V Chong-Morrison

# CRISPR guide pool preparation for microinjections

## Introduction
This protocol has been tested on pools of up to 15 different guides cloned into my U6 vector for zebrafish (3.5kb, Amp resistance, Addgene #119069).

Adapted from Addgene's [Pooled Library Amplification protocol](https://www.addgene.org/protocols/pooled-library-amplification/)

## Materials and Equipment
- Commercial competent cells. Electrocompetent, or Stellar (Takara/ClonTech) chemo-competent - 100 µl per pool.
- Suitable antibiotic agar plates - TWO plates per pool. *Note: Ensure the agar is not too thick*.
- Standard reagents and consumables for bacterial work
- Refrigerated centrifuge with fixed-angle rotor for 5/50 ml tubes up to 12,000 rpm/18,500g
- Bacterial scrapers
- Mini/Midiprep kit (Qiagen, or suitable alternative)
- Qubit™ dsDNA HS Assay Kit (Q32851, ThermoFisher)
- Taq polymerase master mix (NEB, or suitable alternative)
- Suitable primers for PCR

## Procedure

### Pre-flight and Day 1

1. Clone and miniprep U6 guides.
2. Nanodrop to determine concentration.
3. Book refrigerated centrifuge and rotor.
4. Combine an equal amount of every U6 guide in the desired pool to obtain at least 40 ng/µl final concentration. This usually requires at least 200 ng per guide. Mix thoroughly by tapping vigorously, pulse spin.
5. Check concentration of pool on Nanodrop.
6. If necessary, dilute the pool with nuclease-free water in a fresh micro-centrifuge tube to obtain 400-500 ng of DNA in 10 µl.
   
   *E.g. 200 ng each of 15 guides were pooled together and the final volume was 65 µl, so we expect the pool’s concentration to be 46.2 ng/µl. 10 µl of this would be 462 ng of DNA - good to proceed without dilution.*

7. Pre-warm SOC medium.
8. Transform 10 µl of pooled DNA into 100 µl competent cells using standard protocol, adding 1 ml pre-warmed SOC at the end.
9. Shake for 1 hour at 37C.
10. Place agar plates in the incubator to pre-warm.
11. After shaking, perform 1:100 dilution of the cells - add 10 µl of the transformation to 990 µl pre-warmed SOC in a fresh micro-centrifuge tube.
12. Plate 100 µl of this dilution onto a prewarmed dish.
13. Transfer remainder of the undiluted transformation into a micro-centrifuge tube and spin at 4000g for 10 minutes at RT.
14. Remove 800 µl SOC until ~200 µl left. Gently resuspend the pellet.
15. Plate everything (~200 µl) onto second prewarmed dish.
16. Incubate plates overnight at 37C.
17. Place LB (plain, antibiotic not required) in the fridge to chill overnight.

### Day 2

1. Count single colonies on the 1:100 dish and work out the Total Colony Yield.

    **Total Colony Yield = count x 100 ÷ 0.1**
    
    **Total Colony Yield should be at least 1000X greater than number of guides in the pool.**
    
    *E.g. At least 15 single colonies counted on the 1:100 plate for 1000x coverage of a library of 15 plasmids.*

2. Typically, there is an excess of the required number of single colonies on the 1:100 dish, and too many colonies to count on the undiluted dish.
3. Chill 50 ml Falcon tubes (ensure they are rated for high centrifuge speeds!) on ice - one per non-diluted plate/pool.
4. Ensure sterile scrapers and cold LB are ready.
5. Dispense 12 ml cold LB onto the non-diluted plate.
6. Scrape the bacteria into the cold LB, using a gentle pushing motion. Take care not to split or gouge agar during the scraping process.
7. Using a 10 ml serological pipette, carefully collect the cold LB/bacteria slurry into a 50 ml tube on ice.
8. Repeat steps 2-4 so that agar is clear and all bacteria have been removed. This should produce ~25 ml cold LB/bacteria slurry per non-diluted plate/pool.
9. In most cases, Minipreps are sufficient. Take 5 ml of this slurry and process according to standard protocol to purify DNA.
10. Centrifuge remaining ~20 ml slurry at 4000g for 10 minutes at 4°C to pellet bacteria. Remove supernatant and freeze cell pellets as backup.
11. Alternatively, if processing the entire slurry or the backup pellet (resuspend with fresh cold LB), proceed with Midiprep to purify DNA. Elute DNA in 0.5 to 1 ml of Elution Buffer.
12. Quantify DNA (diluted 1:20) by Qubit (not Nanodrop, for accuracy needed for microinjections).

    *Typical yield is 300 - 500 ng/µl for 1 ml eluted DNA (Midiprep) or ~1 µg/µl for 50 ul eluted DNA (Miniprep)*

### Day 3

1. Check that each guide is present in the purified pool using PCR:

    - Prepare 2X PCR master mixes for each guide using forward primer (targeting the universal backbone) and reverse primer (specific to each guide).
    - One reaction experimental i.e. purified pool, one reaction negative control i.e. water.
    - Use 1 ng of the purified pool in 25 µl Taq polymerase reactions, for 30 cycles. If desired, use limited-cycle PCR (e.g. < 20 cycles) to roughly assess representation of each guide via gel band intensity.
    - Check results on a gel.

2. PCR conditions I have tested:

    - Forward primer targeting beginning of U6a promoter (`ATCCCTCGActcgagtttacgtaTTTCTCCAGCCTCGGTCATTCAG`) and Reverse spacer oligo (used in previous
BsmBI guide cloning) producing ~450 bp amplicon.
    - OneTaq® Hot Start 2X Master Mix with Standard Buffer (M0484, New England Biolabs)
    - Primer concentration: 0.5 µl of 10 µM each
    - Annealing temperature: 56C
    - Extension time: 35 secs

Run 5 ul of reaction on 1% gel.
