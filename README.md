# RSOB-22-0369
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

Feel free to contact me if you spot errors, want to develop the scripts into something more useful for the community etc. 

### ITC
Data were obtained using an ITC200 calorimeter (GE Healthcare). Data and binding parameters were pre- analyzed using the MicroCal PeakITC software (Malvern). 
Final analysis and global fits were performed using NITPIC and Sedphat (Brautigam et al., 2016; Scheuermann and Brautigam, 2015).

Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_ITC

### nanoDSF 
Data were obtained using Prometheus (Nanotemper) and pre-analyzed using supplier's software. Data were exported for further analysis and visualization.
Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_nanoDSF_IP

### BLI 
Measurements were performed on an Octet RED instrument (ForteBio). Raw data were pre-processed by subtracting the reference from the sample surfaces and applying a Savitzky-Golay filter as implemented in the Octet RED analysis software.

Link to analysis/visualisation script: https://github.com/derpaule/RSOB-22-0369_BLI

### Cellular and reconstituted condensate assays 
Images were captured using a four-megapixel sCMOS digital camera with the manufacturer’s software MetaXpress, and raw TIF files were analyzed using CellProfiler (CP), ImageJ and Rstudio  (McQuin et al., 2018; Schindelin et al., 2012; Wickham, 2017, 2016; Wickham and Grolemund, 2017). 
Output tables were analysed in R.

- **High-throughput imaging datasets** are stored locally at Karolinska Institutet (each about 300 GB in size) . Please contact Gerald.McInerney@ki.se if you need access to the raw images. Note that images _w3 were offset from w2 images by 4pixels which was corrected using Fiji using batch processing - the macro file was deposited on DRYAD. If covered by Karolinksa, the data may be uploaded on DRYAD at a later stage.
- **G3BP mutants** Cellprofiler pipelines uploaded as pipelines_G3BP1.zip to DRYAD.
- **Caprin-1/chimera** Cellprofiler pipelines uploaded as pipelines_Caprin1.zip to DRYAD.

### Raw images/western blots
The images/blots shown as Figures in the main manuscript and the supplement have been deposited as ZIP file at DRYAD.
The image files are organized in folders/subfolders according to Figure number.

