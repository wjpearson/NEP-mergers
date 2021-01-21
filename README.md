Identifying mergers in the North Ecliptic Pole
=====================================

The repositry contains the code and trained models used to identify merging galaxies within the North Ecliptic Pole field.

The code runs with Python 3.6.9 using Tensorflow 2.3.1. Newer (or older) version of Python and Tensorfow may work but have not been tested. **requirements.txt** contains the modules and version that will work for the code.

If you use this code, please cite Pearson et al. 2021 (in prep). The paper also include the full details for the architecture and data used to train the networks.

Code Usage
----------

**HSC_SSP-merger-wrapped-images.ipynb** trains the convolutional network part of the full network on 128x128 pixel images.

**HSC_SSP-merger-wrapped-morphology-wAS.ipynb** trains the liner network part of the full network on the morphological parameters for the galaxies.

**HSC_SSP-merger-images-morphology-wAS.ipynb** trains the upper part of the full network. HSC_SSP-merger-wrapped-images.ipynb and HSC_SSP-merger-wrapped-morphology-wAS.ipynb need to be run before this script.

**HSC_SSP-merger-images-morphology-wAS-TEST.ipynb** tests the full network. HSC_SSP-merger-images-morphology-wAS.ipynb needs to be run before this script.

Pre-trained Models
------------------

**saved_image_model_HSC_SSP-sex**, **saved_morph_model_HSC_SSP_wAS-sex**, and **saved_model_HSC_SSP_wAS_128-sex-saved** contain the pre-trained models for the CNN, LN and full networks, respectivly.