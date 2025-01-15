# MLAD-C

The **M**ission**L**ab**A**irborne**D**ataset-**C**louds contains aerial images of clouds and associated labeled cloud masks from a flight experiment conducted on October 12, 2023, in the Upper Bavaria region of Germany.
The augmented dataset consists of 5488 RGB images captured from forward-looking perspective.
MLAD-C is designed to develop models for cloud segmentation. In our cloud detection approach, cloud segmentation functions as a pre-stage to cloud position estimation for sense & avoid purposes. 

MLAD-C is available for Download at [Zenodo](https://zenodo.org/records/14267123) (DOI:10.5281/zenodo.14267122).

More detailed information about MLAD-C and the developed cloud segmentation model can be found in our journal article:

[A Cloud Detection System for UAV Sense and Avoid: Analysis of a Monocular Approach in Simulation and Flight Tests](mdpi.com/2504-446X/9/1/55)

## Directory Structure

MLAD-C is provided in two formats:

1. augmented sensor recordings prepared for *YOLO-v8* framework to reproduce results of journal article
2. non-augmented sensor recordings in Full HD resolution

The directory structure is as follows:

- augmented_mladc
    - train
        - images
        - labels
        - masks
    - val
        - images
        - labels
        - masks
    - mladc.yaml

- full_hd_mladc
    - images
    - masks

## Cite

If you use MLAD-C in your research please cite the following publication: 

```
@Article{drones9010055,
AUTHOR = {Dudek, Adrian and Stütz, Peter},
TITLE = {A Cloud Detection System for UAV Sense and Avoid: Analysis of a Monocular Approach in Simulation and Flight Tests},
JOURNAL = {Drones},
VOLUME = {9},
YEAR = {2025},
NUMBER = {1},
ARTICLE-NUMBER = {55},
URL = {https://www.mdpi.com/2504-446X/9/1/55},
ISSN = {2504-446X},
ABSTRACT = {In order to contribute to the operation of unmanned aerial vehicles (UAVs) according to visual flight rules (VFR), this article proposes a monocular approach for cloud detection using an electro-optical sensor. Cloud avoidance is motivated by several factors, including improving visibility for collision prevention and reducing the risks of icing and turbulence. The described workflow is based on parallelized detection, tracking and triangulation of features with prior segmentation of clouds in the image. As output, the system generates a cloud occupancy grid of the aircraft’s vicinity, which can be used for cloud avoidance calculations afterwards. The proposed methodology was tested in simulation and flight experiments. With the aim of developing cloud segmentation methods, datasets were created, one of which was made publicly available and features 5488 labeled, augmented cloud images from a real flight experiment. The trained segmentation models based on the YOLOv8 framework are able to separate clouds from the background even under challenging environmental conditions. For a performance analysis of the subsequent cloud position estimation stage, calculated and actual cloud positions are compared and feature evaluation metrics are applied. The investigations demonstrate the functionality of the approach, even if challenges become apparent under real flight conditions.},
DOI = {10.3390/drones9010055}
}
```

## Funding

The research project MissionLab is funded by dtec.bw – Digitalization and Technology Research Center of the Bundeswehr which we gratefully acknowledge. dtec.bw is funded by the European Union – NextGenerationEU.
