# Primer design for Stemloop PCR:
Two primers need to be designed for each unique miRNA. For the first phase, the Stemloop RT, a Stemloop RT primer 
needs to be made. This primer consists of the universal stemloop RT primer to which the 5’ 6 nt of the reverse complement DNA
sequence are added at the 3’.
For the end point PCR a universal reverse primer (GTGCAGGGTCCGAGGT, Tm 55.9&deg;C (OligoCalc)) is used. 
The forward primer needs to be miRNA specific. This consists of the miRNA sequence converted to DNA, 
of which 6 nt at the 3’-end are removed. At the 5’-end nts are added to increase the Tm equal to the Tm of the reverse primer.

![stemloopRT](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2225395/bin/1746-4811-3-12-1.jpg)<br/>
*Varkonyi-Gasic et al., 2007*<br/>

### Example:
#### miRNA159<br/>
UUUGGAUUGAAGGGAGCUCUA, RNA<br/>

#### End-point PCR
To make the forward primer (for end-point PCR) take the miRNA sequence and convert to DNA, take all except the last 6 nts.<br/>
TTTGGATTGAAGGGA**GCTCTA**, DNA<br/>

*forward primer:*<br/>
TTTGGATTGAAGGGA, Tm = 40.6&deg;C (calculated with OligoCalc, salt adjusted)<br/>
To make the temperature equal to that of the universal reverse primer (GTGCAGGGTCCGAGGT, Tm = 55.9&deg;C, some nts are added.<br/>

*forward primer (inc. extra nt):*<br/>
ggacTTTGGATTGAAGGGA, Tm = 55&deg;C<br/>

#### Stemloop-RT
To make the RT primer (used for reverse transcriptase) take the miRNA sequence, convert to DNA and than complement.
Add to the universal RT primer (TCGTATCCAGTGCAGGGTCCGAGGTATTCGCACTGGATACGAC) the last 6 nucleotides in reverse order (last nucleotide first, than 5th, 4th, 3rd, 2nd and first).

AAACCTAACTTCCCTCGAGAT, comp<br/>
**TAGAGC**TCCCTTCAATCCAAA, revcomp<br/>

*RT primer:*&nbsp;&nbsp;&nbsp;gtcgtatccagtgcagggtccgaggtattcgcactggatacgac**TAGAGC**

