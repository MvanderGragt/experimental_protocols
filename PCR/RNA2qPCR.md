# From RNA to Q-PCR

## RNA isolation
•	make sure to have at least 3 biological replicates<br/>• isolate clean total RNA (kit or phenol), there should be no degradation

## DNase treatment of isolated RNA (TURBO DNase kit Ambion)
•	RNA in 45 µl H2O dd<br/>
•	add 5 µl 10x buffer and 0,5 µl DNase<br/>
•	20’ 37°C<br/>
•	add 5 µl DNase inactivation reagent<br/>
•	3’ RT with occasional mixing<br/>
•	1,5 ‘ max speed spin<br/>
•	pipette off RNA into clean tube without disturbing the pellet<br/>
•	nanodrop and/or put on gel to check integrity and quantify carefully<br/>

## cDNA synthesis (Revert Aid kit Fermentas)
•	include NAC and NTC (see below)<br/>
•	0,5-2 µg total RNA<br/>
•	add 1 µl oligo(dT)18<br/>
•	up to 13 µl with H2O dd<br/>
•	5’ 70°C, chill on melting ice<br/>
•	add 4 µl 5x buffer<br/>
•	add 2 µl 10 mM dNTPs<br/>
•	add 0,25-1 µl RT transcriptase (amount depending on total RNA input)<br/>
•	add 0,75-0 µl H2O dd (adds up to 1 µl with RT transcriptase)<br/>
•	60’ 42°C<br/>
•	10’ 70°C, chill on melting ice<br/>
•	when used 1 µg you count with RNA equivalent concentration of 50 ng µl-1<br/> 

## Preparation Q-PCR
•	check all cDNA samples with normal PCR (check: primer dimers, gDNA, cDNA integrity)<br/>
•	dilute to equivalent of 10 ng RNA for all samples<br/>
•	to calculate primer efficiencies take cDNA sample expected to have the highest expression and make dilution range: 1x-4x-16x-64x-256x (1x = 10 ng)<br/>
•	make non amplification control (NAC): RT reaction without RT enzyme; test cDNA for gDNA contamination<br/>
•	make no target control (NTC): do RT reaction with a water sample; test for contamination and primer dimers<br/>
•	make H2O control: water sample for each primer pair on each plate; test primer dimers<br/> 
•	dilute primers from stock (filter-tips!) to 10 µM working stocks<br/>

## Q-PCR
•	work on ice, not in strong daylight, work fast<br/>
•	see excel sheet for pipetting scheme<br/>
•	make MasterMix: 	5x EvaGreen Mix / ROX / water<br/>
•	make PrimerMix: 	dilute primers to 300 nM and add pairs together<br/>
•	mix cDNA with MM: mix 1 - mix n<br/>
•	aliquot mix 1-n over each PM<br/>
•	disperse into 2 or 3 wells (=technical replicates)<br/>
•	add NAC and NTC controls on the plate<br/>
•	add dilution range for each primer pair on the plate<br/>

## Machine
•	switch on and check the if the holder is right for strip or plate<br/>
•	start computer,  open 7500 system software<br/>
•	file / new / absolute quantification / next<br/>
•	select detector (make sure it is one with SYBR reporter)<br/>
•	next / 96-well scheme is shown; possible to fill in sample names<br/>
•	close / go to instrument tab<br/>
•	deselect 9600 emulation<br/>
•	volume 10 µl<br/>
..1: 2’ 50°C<br/>
..2: 15’ 95°C<br/>
..3: 15’’ 95°C, 1’ 60°C, 45 cycles<br/>
•	add dissociation stage<br/>
•	save as, save in your folder as sds<br/>
•	put samples in machine, close, press start and wait until run starts<br/>
•	result / amplification /<br/> 
•	select Rn vs cycle and set baseline (where all curves are flat)<br/>
•	deltaRn vs cycle and set manual Ct to point where *a) all curves still linear b) nicely parallel to each other c) having largest distance from each other*<br/>
•	press analyse<br/>
•	export your data to file and also to memory-stick: file / export / results / cvs<br/>

## Quality Checks
•	check raw data for strange amplification curves: both in Rn vs cycle and deltaRn vs cycle<br/> 
•	curves should be parallel in log-linear phase, certain samples might have abnormal amplification efficiency<br/>
•	check dissociation curves (Tdissociation should be equal in all reactions)<br/>
•	check NTC or water control for primer dimers and contaminations<br/>
•	if product in NTC, check if its Tm is different from target reaction Tm. If Tm is not very different: its Ct should be at least 5 higher than of the target reaction<br/>
•	check NAC control for amplification of gDNA. If Tm of NAC fragment is different, check that NAC fragment is not present in target reactions. If Tm is not very different, Ct value should be at least 5 higher than of the target reaction<br/>
•	primer specificity: only one clear curve should be present in the dissociation analysis<br/>
•	check primer efficiencies in dilution series; should be around 2 (double each cycle). Plot the log of cDNA concentration against the Ct value. (see excel calculation sheet)<br/>

## Calculations
•	Open in CSV-file and save it as EXCEL<br/>
•	Determine the primer efficiency (see calculation sheet)<br/>
•	Take average Ct of technical replicates<br/>
•	Calculate the RQ (relative quantification: =1/(2,0 ^ Ct)<br/>
•	Calculate the NE (normalised expression: = RQtarget/RQnorm<br/>
•	You can present the NE but when doing statistics, perform a back-transformation first<br/>

