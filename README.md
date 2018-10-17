# Adjusting for Confounding in Unsupervised Latent Representations of Images

This repository collects implementation details for the analyses reported in the paper [Adjusting for Confounding in Unsupervised Latent Representations of Images.](url)

# Contents

- [Dependencies](#dependencies)
- [Data](#data)
- [Background and Motivations](#background-and-motivations)
- [Training](#training)
- [Models](#models)

# Dependencies

`python 3.5.2`
`skimage 0.13.1`

`numpy 1.14.3`
`torch 0.4.0`

# Data 

We used the BBBC021v1 image set, which is a resource freely available to download through the Broad bioimage benchmark collection web server ([https://data.broadinstitute.org/bbbc/](https://data.broadinstitute.org/bbbc/)). These data capture phenotype changes of cancer cell lines exposed to a compendium of drugs. The imaging set was annotated as benchmark data to develop phenotypic profiling methods and, in particular, to validate their ability to predict the molecular mechanism of action (MOA) for a collection of compounds. Phenotypes were captured, across 10 weeks (batches), by labelling cells with DAPI, Tubulin, and Actin, thereby generating a triplet of single channel images (one per fluorescent marker) for each treatment.

For each image in the BBBC021v1 set, we detected cell nuclei using the algorithm difference of Gaussians on the DAPI channel. We cropped patches of <img src="https://latex.codecogs.com/svg.latex?\inline&space;128&space;\times&space;128" title="128 \times 128" /> pixels centred around each nucleus, and annotated <img src="https://latex.codecogs.com/svg.latex?\inline&space;128&space;\times&space;128&space;\times&space;3" title="128 \times 128 \times 3" /> images by concatenating patches from the DAPI, Tubulin, and Actin channels. Representative training images are displayed in Figure 1.

# Background and Motivations

# Training

# Models
