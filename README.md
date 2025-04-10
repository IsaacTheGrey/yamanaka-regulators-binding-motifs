# yamanaka-regulators-binding-motifs
Searching for binding motifs of regulators of Yamanaka factors

How to proceed:
1. Get the genomic loci of the yamanaka factors (10 kb before and after the gene)
2. make a bed file with the genomic loci
3. get the motifs of interest as PWM format or as a consensus 
4. run a script for the identification of these motifs

Yamanaka regulators: npm & srrt



srrt XLOC-0404390
MF-dependently expressed 12hpa 

srrt/ars2 binds sox2 enhancer region in mouse (10.1038/nature10712)

To do: 
predict srrt in alphafold, compare to mouse ars2
Check sox1b1 XLOC-064106 locus for ars2 binding motif
GTTAAGCAAATTAAATTTGATTCT






nucleophosmin/nucleoplasmin XLOC-051581
MF-dependently expressed 6hpa 

Npm binds 4G quadruplex region. 4G regulates myc expression (doi: 10.1074/jbc.M112.371013)
Npm interact swith myc protein (https://doi-org.uaccess.univie.ac.at/10.1073/pnas.0806879105)
Npm essential for myc nucleolar localisation (https://doi-org.uaccess.univie.ac.at/10.1038/onc.2012.227)

To do: 
predict npm in alphafold, c-terminus like human npm, binds 4G?
Check myc XLOC-004670 locus for 4G 


