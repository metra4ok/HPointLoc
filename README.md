# HPointLoc
Framework for visual place recognition and localization. This project is a complete implementation of paper "HPointLoc: open dataset and framework for indoor visual localizationbased on synthetic RGB-D images"

This repository provides a novel framework **PNTR** for work with novel indoor dataset - **HPointLoc**, specially designed for exploring capabilities for detection and loop closure in Simultaneous Localization and Mapping (SLAM).

Our paper on deep learning-based visual place recognition contains detailed information about these datasets:
> BibteX:
> HPointLoc: open dataset and framework for indoor visual localizationbased on synthetic RGB-D images*

## Quick start to evaluate PNTR pipeline

```bash
git clone --recurse-submodules https://github.com/cds-mipt/HPointLoc
conda env create -f environment.yml
python pipelines/pipeline_evaluate.py --dataset_root /path/to/dataset --image-retrieval 'patchnetvlad' --keypoints-matching 'superpoint_superglue' --optimizer-cloud 'teaser' -f  
```

