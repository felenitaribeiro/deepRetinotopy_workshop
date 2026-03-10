# deepRetinotopy Workshop

Workshop materials for predicting retinotopic maps from cortical anatomy using [deepRetinotopy](https://github.com/felenitaribeiro/deepRetinotopy_TheToolbox), a geometric deep learning toolbox for retinotopic mapping.

## Overview

This workshop walks participants through using deepRetinotopy to predict polar angle and eccentricity maps of the human visual cortex from FreeSurfer-derived anatomical surfaces -- no functional MRI data required.

## Notebooks

### Part 1: Predicting retinotopic organisation
Two notebooks are provided depending on whether participants bring their own data:

- **`1_deepretinotopy_wo-data.ipynb`** -- Downloads example data from the [NYU Retinotopy Dataset](https://openneuro.org/datasets/ds003787) (via DataLad) and runs the full pipeline: data setup, single-subject and multi-subject processing, and interactive visualization.
- **`1_deepretinotopy_w-data.ipynb`** -- For participants with their own FreeSurfer outputs. Covers loading custom data, running predictions, and visualizing results.

## Platform

These notebooks are designed to run on [Neurodesk](https://www.neurodesk.org/), an open platform that provides a reproducible environment for neuroimaging analysis with pre-installed tools. The easiest way to get started is through [Neurodesk Play](https://play.neurodesk.org/), a cloud-based JupyterLab instance that requires no local installation -- just open it in your browser and you're ready to go.

All required neuroimaging software (FreeSurfer, deepRetinotopy) is available via Neurodesk's `module` system, so there is no need to manage installations or dependencies manually.

## Requirements

- A [Neurodesk Play](https://play.neurodesk.org/) session (or a local [Neurodesk](https://www.neurodesk.org/docs/getting-started/neurodesktop/) installation)
- FreeSurfer directory with minimal surface files per subject (`lh/rh.white`, `lh/rh.pial`, `lh/rh.sphere.reg`)
- HCP `fs_LR-deformed_to-fsaverage` template surfaces (downloaded within the notebooks)

## Reference

Ribeiro, F. L. et al. (2025). Predicting functional topography of the human visual cortex from cortical anatomy at scale. [bioRxiv](https://www.biorxiv.org/content/10.1101/2025.11.27.690210v2)