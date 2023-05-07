# Supplementary data to RSOB-22-0369
Code and data associated with our study **"Caprin-1 binding to the critical stress granule protein G3BP1 is influenced by pH"** published in Open Biology with the ID code RSOB-22-0369.
An earlier version of our study has been posted on [BioRxiv](https://www.biorxiv.org/content/10.1101/2021.02.05.429362v1) on February 05, 2021.

The associated structure of NTF2 in complex with the Caprin-1 derived SLiM has been deposited on 2019-10-29 and released on 2021-05-12 with PDB code [6TA7](https://www.rcsb.org/structure/6TA7)

Here, we also thank the critical reviewers during the inital submission at Molecular Cell for suggesting 

- to re-analyze the imaging data to take into account the variable GFP-G3BP1 (and GFP-Caprin-1) expression
- to establish in vitro reconstituted condensate assays

Data used to generate the figures have also been depostited at [DRYAD](https://doi.org/10.5061/dryad.k98sf7mb8). 

---
Analysis and visualization scripts of the data are separated by method, and listed here. \
Note: the scripts are not annotated thoroughly. So you need to be familiar with R and the tidyverse.\
Plots were saved as postscript files, and edited into publication-quality figures using Adobe Illustrator. The legend to the pre-figures in the markdown document contain information for which figure they were used in the manuscript.\
The bookdown document was created based on [bookdown](https://bookdown.org/yihui/bookdown/), and [rtemps](https://github.com/bblodfon/rtemps).

Please reach out to me if you spot errors, have probles with the scripts/data, or want to develop the scripts into something more useful for the community etc. 

---
## ITC
related to Figures 2 and 4.

Data were obtained using an ITC200 calorimeter (GE Healthcare). Data and binding parameters were pre- analyzed using the MicroCal PeakITC software (Malvern). 
Final analysis and global fits were performed using NITPIC and Sedphat (Brautigam et al., 2016; Scheuermann and Brautigam, 2015).

Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_ITC

---
## nanoDSF 
related to Figure 4.

Data were obtained using Prometheus (Nanotemper) and pre-analyzed using supplier's software. Data were exported for further analysis and visualization.

Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_nanoDSF_IP

---
## BLI 
related to Figure 2.

Measurements were performed on an Octet RED instrument (ForteBio). Raw data were pre-processed by subtracting the reference from the sample surfaces and applying a Savitzky-Golay filter as implemented in the Octet RED analysis software.

Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_BLI

---
## Cellular and reconstituted condensate assays 
Images were captured using a four-megapixel sCMOS digital camera with the manufacturer’s software MetaXpress, and raw TIF files were analyzed using CellProfiler (CP), ImageJ and Rstudio  (McQuin et al., 2018; Schindelin et al., 2012; Wickham, 2017, 2016; Wickham and Grolemund, 2017). Note: original images _w3 were offset from w2 by 4 pixels which was corrected using Fiji using batch processing - the corresponding macro file was deposited on DRYAD.  
Output tables were analysed in R.

### High-throughput cellular imaging datasets 
related to Figures 5 and 7.

**DRYAD data related to Figure 5 (G3BP1 mutants)** 
- Cellprofiler pipeline
  - *pipelines_G3BP1.zip*  
- Imaging datasets in ZIP folders 
  -  *img_plate2171.zip* 
  -  *img_plate2185.zip*
  -  *img_plate21691.zip*
- LLPS images and Excel summary in LLPS_GFP-Caprin-1.zip
- Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_condensates_GFP-G3BP1

**DRYAD data related to Figure 7 (Caprin-1 chimera)** 
 - Cellprofiler pipeline 
    - *pipelines_Caprin1.zip* / Note: uncertain about 1740 pipeline. there are two saved pipelines which are both uploaded.
 - Imaging datasets in ZIP folders 
    - *img_plate1734.zip*
    - *img_plate1735.zip* 
    - *img_plate1737.zip*
 - LLPS images and Excel summary in LLPS_GFP-G3BP1.zip
 - Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_condensates_GFP-Caprin1

---
## Raw images/western blots
related to Figures 2, 4, 5, 6, 7.

The images/blots shown as Figures in the main manuscript and the supplement have been deposited as ZIP file at DRYAD.
The image files are organized in folders/subfolders according to Figure number.

