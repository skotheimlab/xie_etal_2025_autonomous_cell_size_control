# The G1/S transition in mammalian stem cells in vivo is autonomously regulated by cell size
Image analysis and statistical modeling tools for cell and microenvironment analysis of skin stem cell growth and cell cycle progression in vivo.

Tested on Python 3.9 on MacOS. More detailed instructions are in ./2024_analysis/instructions.txt. Requirements are listed in ./2024_analysis/requirements.txt

## Contents:

### semiauto_tracking_segmentation:
- Scripts for semi-automated movie assembly and collation of semi-automated single cell tracking in 3D

Expected input data: raw images, segmentation masks of nuclear shapes in 3D, and single cell tracking from MaMuT tracking tables

### assemble_movie:
- Semi-automated registration and assembly of movies from longitudinal snapshots semiauto_tracking_segmentation: collate segmentation and sparse single cell tracking
- Cell and microenvironment quantifications: Scripts for quantifying and collating cell and cell-neighborhood geometries using densely annotated 3D cell and nuclear segmentations

Expected input data: raw images, segmentation masks of cell and nuclear shapes in 3D

### annotate_tissue_dense:
- Annotate cell and microenvironment features tissue_dynamics_model
- Statistical models predicting cell cycle dynamics from cell or microenvironment features
