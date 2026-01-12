# ACTB_Primer_Design
notes regarding NGS analysis - jan 26 
Author : Harshita 

# TITLE 
Primer Design and Specificity Analysis for Human ACTB Gene using Primer-BLAST

# AIM 
To design gene-specific PCR primers for the human ACTB gene and validate their specificity using NCBI Primer-BLAST.

# Tools Used
NCBI Gene database
NCBI Primer-BLAST
ACTB mRNA sequence (NM_001101.5)

# Procedure
ACTB gene sequence was retrieved from NCBI Gene database. (https://www.ncbi.nlm.nih.gov/gene/)
Primer design was performed using Primer-BLAST with product size set to 80–200 bp and Tm ~60 °C.
Primer specificity was checked against the human genome (taxid:9606).
Primer pair with optimal parameters and single predicted product was selected.

# Result 
Forward Primer: CCTTCCTTCCTGGGCATGG
Reverse Primer: CTGTGTTGGCGTACAGGTCT
Amplicon size: 103 bp

# Conclusion 
The designed primers showed optimal characteristics and high specificity, making them suitable for PCR and NGS applications.

# FIGURE SHOWING THE PRIMER PAIRS
1.

<img width="1778" height="487" alt="Screenshot 2026-01-12 161656" src="https://github.com/user-attachments/assets/3cdc607e-c694-49e5-942a-47d1e3f06fe5" />

2.

<img width="1771" height="906" alt="Screenshot 2026-01-12 161713" src="https://github.com/user-attachments/assets/62ef5f13-4a8a-4c52-9577-793d3065f735" />

3.

<img width="1760" height="833" alt="Screenshot 2026-01-12 161730" src="https://github.com/user-attachments/assets/f96581c7-eb10-466b-b16c-ae029bb7a6fc" />


# 1. On-Target Matches
Does the primer pair match the target gene with 100% identity?
The selected primer pair showed a 100% sequence identity match to the intended target gene ACTB (NM_001101.5). Primer-BLAST predicted a single specific PCR product of 103 bp corresponding to the ACTB gene, confirming accurate on-target amplification.

# 2. Off-Target (Non-Specific) Hits
a) potential targets : Primer-BLAST analysis against the Homo sapiens genome (taxid:9606) revealed only one predicted amplification product corresponding to the ACTB gene. No additional products were detected on unintended genomic regions. 
b) Critical Check : No binding of both forward and reverse primers was observed within 2,000 bp of each other on any unintended chromosome or pseudogene. Therefore, the risk of non-specific amplification is minimal.
c) rule of thumb 
rule : Non-specific product is risky if both primers bind within 2,000 bp with ≤2–3 mismatches at 3′ end.
analysis : According to the rule of thumb, non-specific amplification is unlikely, as Primer-BLAST did not identify any unintended genomic regions where both primers bind within 2,000 bp with fewer than 2–3 mismatches at the 3′ end. 

# 3. Primer Quality Assessment 
a) GC Content (40–60%)
Primer	GC %
Forward	63.16%
Reverse	55.00%
The GC content of the primers falls within or close to the recommended range (40–60%), ensuring stable primer-template binding without excessive secondary structure formation.
b) GC Clamp (3′ end stability)
Forward 3′ end: G
Reverse 3′ end: T (with nearby GC bases)
The primers contain a GC clamp at the 3′ end, providing stable binding at the extension site and improving amplification efficiency.
c) Self-Complementarity (Primer Dimers)
| Parameter            | Value |
| -------------------- | ----- |
| Self complementarity | 4.0   |
| 3′ complementarity   | 2.0   |
Both primers exhibit low self-complementarity and low 3′ complementarity scores, indicating a low risk of hairpin or primer-dimer formation.
conclusion : Overall analysis of the Primer-BLAST results indicates that the selected ACTB primer pair demonstrates high on-target specificity, no significant off-target binding, acceptable GC content, a stable GC clamp, and low self-complementarity. Therefore, the primers are of high quality and suitable for specific PCR amplification and NGS target enrichment.

# Deliverables – ACTB Primer Design 
1. Forward Primer Sequence (5′ → 3′): CCTTCCTTCCTGGGCATGG
2. Reverse Primer Sequence (5′ → 3′): CTGTGTTGGCGTACAGGTCT
3. | Parameter                | Forward Primer | Reverse Primer |
| ------------------------ | -------------- | -------------- |
| Length                   | 19 bp          | 20 bp          |
| Melting Temperature (Tm) | 60.08 °C       | 59.97 °C       |
| GC Content               | 63.16%         | 55.00%         |
4. Expected Product Size: 103 bp 
5. Specificity Statement: The primer pair is specific to the human ACTB gene and produces a single amplification product of 103 bp. Primer-BLAST analysis against the human genome (taxid:9606) showed no significant off-target amplification. 
