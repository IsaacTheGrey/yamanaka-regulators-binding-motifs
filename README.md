# yamanaka-regulators-binding-motifs
This project scans genomic regions for known DNA motifs (with optional mismatches) and visualizes the results.

## Usage
### 🛠 Environment Setup

Reccomended to use **Mamba** (a faster Conda replacement).

#### 1. Install Mamba (if needed)
```bash
conda install -n base -c conda-forge mamba
mamba create -n motifscan
mamba activate motifscan
mamba install -c conda-forge jupyterlab matplotlib pandas pyfaidx
```

### 📁 Inputs
- A reference genome in FASTA format to put in the folder /references
- A list of target regions in the script (`gene`, `chrom`, `center`, `window`)
- A list of motifs to scan (consensus sequences)

### 📂 Outputs

All results will be written to the motif_plots/ folder:

    *.tsv: tabular motif hit reports
    *.png: per-gene motif hit plots (Visualization colors: blue = forward strand, red = reverse strand)




## Example case

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


