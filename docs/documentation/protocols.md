# Protocols
## Golden Gate Cloning
Golden Gate constructs were assembled using the EcoFlex MoClo kit (Addgene kit #1000000080) doi.org/10.1021/acssynbio.6b00031. This kit comes with level 0,1, and 2 backbones (see publication for more details).

1. Add the following to a PCR tube (use BsaI for level 1 and BsmBI for level 2 assemblies):
 
│ Reagent │ Amount │
│ --- │ --- │
│ Backbone DNA │ 50 ng│ 
│ Insert DNA │ 100 ng │
│ T4 ligase buffer│ 1 μl │
│ T4 ligase │ 0.5 μl │
│ BsaI / BsmBI │ 0.5 μl │
│ ddH2O │to 10 μl │


Incubate in the thermocycler using the following protocol:
Level 1 / BsaI
Step
Cycles (x)
Temperature (ºC)
Time
Digestion and ligation
15-30
37
5 min
Annealing
16
10 min
Final digestion and T4 ligase inactivation
1
50
5 min
Enzyme inactivation
1 
80
5 min



Level 2 / BsmBI

Step
Cycles (x)
Temperature (ºC)
Time
Initial digestion
1
42
1 h
Digestion and ligation
99
42
5 min
Annealing
16
1 min
Final digestion
1
42
1 h
Enzyme inactivation
1 
80
15 min


Note: Try to use smaller vectors containing fewer inserts as reduced protein expression demands may exhibit higher transformation efficiency due to the reduced size and lower metabolic load on the cells.

## Gibson Assembly
PCR of all inserts & backbones to create appropriate overhangs, 
DpnI Digest: add 0.5 uL of DpnI to 25 uL PCR reaction, incubation 15 min at 37°C ( to remove the template DNA)
Gel extraction of the correct PCR products: Follow the protocol of the NucleoSpin Gel and PCR Clean-up kit (Macherey-Nagel)
Mix 50–100 ng of vector DNA with a molar 2:1 or 1:1 ratio of each insert (see table below) 
Add water and NEBuilider HiFi DNA Assembly Master Mix as indicated below


2-3 Fragment Assembly
4-6 Fragment Assembly
molar DNA ratio (vector:insert)
1:2
1:1
total amounts of DNA fragments
0.03-0.2 pmol
0.2-0.5 pmol
NEBuilider HiFi DNA Assembly Master Mix
2.5 μl
2.5 μl
ddH2O
fill up to 5 μl
fill up to 5 μl


Incubate samples in a thermocycler at 50°C for 60 minutes 
Store samples on ice or at –20°C for subsequent transformation



## Transformation
To test our genetically engineered constructs, we transformed them into bacteria. For single plasmid transformation, E. coli cells were made chemically competent using the Mix & Go E. coli Transformation Kit & Buffer Set (Zymo Research), following the manufacturer's protocol.

Thaw competent DH5a on ice
Add 1 μl of plasmid DNA or 5 uL of assembly reaction to 20-50 μl of competent cells
Flick the tube to mix
Incubate mixture on ice for 30 minutes
Heat shock at the bacteria at 42 °C for 30 s
Place on ice for 5 minutes
Pipette 200 µl of room temperature LB into the mixture
Incubate at 37°C for 60 minutes while shaking at 750 rpm
Warm selection plates to 37 °C in the incubator
Spin down bacteria and resuspend in 50 μl LB
Spread 50-100 μl of cells on LB agar plates containing the antibiotics for selection.
When multiple antibiotics are used, use 0.6x of the standard working concentration for each antibiotic.
Incubate overnight at 37 °C

For co-transformations with two accessory plasmids:
Thaw competent S2060 cells on ice
pre-mix 200 ng of the two accessory plasmids in an equimolar ratio
Add 50 μl of competent cells
Continue at step 3 above
Due to the metabolic burden caused by DNA replication and protein expression, co-transformants might grow at a markedly reduced rate.

## Phage production
The production of our phages started by assembling a plasmid containing all phage genes. Our selection plasmid, containing either SIAH1/2 or unspecific enzymes but lacking essential genes for phage replication was combined with splitC (Addgene #138523) and splitD (Addgene #138521) plasmids using SapI Golden Gate assembly
Day 1: Golden Gate assembly
Assemble a plasmid containing all phage genes: the selection plasmid, splitC (Addgene #138523) and splitD (Addgene #138521) by mixing the following components in a PCR tube

T4 DNA ligase buffer (10x)
2 μl
SapI
1 μl
T4 DNA ligase
1 μl
selection plasmid
200 ng
SplitC
100 ng
SplitD
100 ng
ddH2O
to 20 μl 


Incubate in the thermocycler overnight with the following program:

Step
Cycles (x)
Temperature (ºC)
Time
Digestion and ligation
99
37
5 min
Annealing
18
5 min
Final digestion 
1
37
1 h
Enzyme inactivation
1 
80
15 min


Day 2: Transformation
Transform the assembly reaction as explained above
Thaw competent S2060 cells on ice
Add 2 µl of the ligation reaction into 50 μl of competent S2208 cells
Flick the tube to mix
Incubate mixture on ice for 30 minutes
Heat shock at the bacteria at 42 °C for 30 s
Place on ice for 5 minutes
Pipette 200 µl of room temperature LB into the mixture
Incubate at 37°C while shaking at 750 rpm until bacteria reach saturation
Warm selection plates to 37 °C in the incubator
Spin down bacteria and resuspend in 50 μl LB
Spread 50-100 μl of cells on LB agar plates (which antibiotic)?
Incubate overnight at 37 °C
Day 3: Plaque Assay to determine phage titer
Note: it makes sense to do 2 plaque assays: the first one to see if phages are produced and what their pfu is. Pick one phage of the first plaque assay to get monoclonal phages and repeat the plaque assay again
Spin down 2 mL (9000 g, 1 min)
Transfer supernatant to a new tube and sterilise with a 0.22 µm filter
Send purified phages for Sanger sequencing with the primer oLS670
Determine the phage titer with a plaque assay as described below
Phages can be stored in the fridge for multiple months. If titer gets to low, re-grow in S2208 bacteria again

## Determination of phage titer by plaque assay
Spin down your samples at 8’000 xg for 2 min to remove bacteria and other contaminants
Transfer supernatant to a new tube. Phages can be stored at 4ºC for further use (note that phage titer will gradually decrease over time)
Dilute a saturated S2208 culture and grow it to an OD600 of 0.5
Pour 15 mL LB agar without antibiotics in a Petri dish and let solidify
Once solidified, mix 2 mL of LB and 2 mL of hot LB agar, add 1 mL of the S2208 culture, vortex quickly, and pour on top of the solidified LB agar. Let solidify for at least 30 min
Meanwhile, prepare a 10-fold serial dilution of your phage sample (100 to 10-7). Remember to include a phage with a known pfu/mL as a positive control
Add 4 µL of each dilution onto the top agar. Let the plate sit for 15-30 min before transferring it to the incubator, making sure that the drops do not merge
Incubate plate overnight (16-20 h) at 37ºC
The tier of the phage sample can be determined by the following formula: 

titer (in pfu/mL) = (# of plaques) x (dilution factor) x 100 

## Determination of phage titer by qPCR
Spin down your samples at 8’000 xg for 2 min to remove bacteria and other contaminants
Transfer supernatant to a new tube. Phages can be stored at 4ºC for further use (note that phage titer will gradually decrease over time)
Prepare the qPCR reaction mix as follows (see Supplementary XX for oLS-1662 and oLS-1663):

Reagent
µL/well
FirePol Polymerase
3
oLS-1662 100 uM
0.05
oLS-1663 100 uM
0.05
Water
9.9


In a qPCR 384-well plate, add 13 µL of qPCR reaction mix to each well, followed by 2 µL of the supernatant of each sample. Perform triplicate measurements for better results
Cover the plate with an adhesive seal and briefly spin down the plate 
Insert the plate in the qPCR machine (here, we used the LightCycler 480 II from Roche) and program the following settings: 

Step
Cycles (x)
Temperature (ºC)
Time
Pre-incubation
1
95
12 min
Denaturation
45
95
15 s
Annealing
53
30 s
Elongation
72
10 s


Set the excitation wavelength to 465 nm and the detection wavelength to 510 nm and start the protocol
Analyse readout with the software analysis tool “Absolute Quantification/Second Derivative Maximum”
Threshold cycle (CT) values, which indicate the cycle number at which the fluorescence from the amplifying DNA exceeded a predefined threshold, can be converted to PFU/mL using previously constructed standard curved. qPCR results with CT > 30 can be considered as absence of phages

## Site-directed mutagenesis for substrate degron modification
Prepare a reaction mix in a PCR tube as indicated here (see Report for the corresponding primers):

Reagent
25 µL reaction
5X Q5 Reaction Buffer
5 µL
10 mM dNTPs
0.5 µL
10 µM Forward Primer
1.25 µL
10 µM Reverse Primer
1.25 µL
pES1076 template
100 ng
Q5 High-Fidelity DNA Polymerase
0.25 µL
Nuclease-Free Water
to 25 µL


Gently mix the reaction and collect all liquid to the bottom of the tube by briefly spinning it, if necessary
Set the thermocycler for the following program:

Step
Cycles (x)
Temperature (ºC)
Time
Initial Denaturation
1
98
30 s
Denaturation

30
98
5 s
Annealing
50-72*
20 s
Elongation
72
20 s/kb
Final Elongation
1 
72
2 min

*calculate annealing temperature for your pair of primers with the NEB Tm Calculator

Treat 1 µL of the PCR reaction with 5 µL of KLD buffer, 1 µL of the KLD Enzyme Mix, and top it with 3 µL of water
Incubate at room temperature for 5 min
Transform 2 µL of the KLD reaction into 20 µL of competent cells and plate directly in LB agar with the appropriate antibiotics without recovery

## Phage propagation assay 
Transform S2060 cells with the AP(s) of interest (see Transformation)
Dilute a saturated overnight culture of bacteria 1,000-fold into LB media supplemented with the appropriate antibiotics and grow at 37ºC to OD600 0.5
Aliquote 1 mL of culture into a deep-well plate and infect with phages at a starting titer of 106 pfu/mL. Seal the plate with a breathable membrane.
Incubate the plate overnight (16-20 h) at 37ºC
Determine the phage titer by performing a plaque assay (see Determination of phage titer by plaque assay). To calculate fold propagation, divide the final phage titer by the starting titer

## Phage-assisted non-continuous evolution (PANCE) to generate a library of Selection Plasmids (SP)
To drift your selection plasmid, you will use a S2060 strain transformed with DP6 plasmid (see Transformation)
Dilute a saturated overnight bacteria culture in 50 mL LB with appropriate antibiotics and 100 mM glucose, and grow it to an OD600 of 0.5
Add arabinose to a final concentration of 40 mM. This will induce the expression of the mutagenesis machinery.
Immediately after, infect your culture with phages containing the SP you want to drift to a final concentration of 104 pfu/mL
Incubate the flask at 37ºC, shaking at 250 rpm, overnight (16-20 h)
The following day, determine the phage titer using qPCR (see Determination of phage titer by qPCR)
Initiate the next round of drift by repeating steps 2 to 6. Infect the fresh culture with the phages that propagated overnight and whose titer you determined by qPCR
