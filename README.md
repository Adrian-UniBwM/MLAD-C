# MLAD-C

The **M**ission**L**ab**A**irborne**D**ataset-**C**louds contains aerial images of clouds and associated labeled cloud masks from a flight experiment conducted on October 12, 2023, in the Upper Bavaria region of Germany.
The augmented dataset consists of 5488 RGB images captured from forward-looking perspective.
MLAD-C is designed to develop models for cloud segmentation. In our cloud detection approach, cloud segmentation functions as a pre-stage to cloud position estimation for sense & avoid purposes. 

MLAD-C is available for Download at [Zenodo](https://zenodo.org/records/14267123) (DOI:10.5281/zenodo.14267122).

More detailed information about MLAD-C and the developed cloud segmentation model can be found in our journal article: **TBD**

<!-- [A Cloud Detection System for UAV Sense and Avoid: Analysis of a Monocular Approach in Simulation and Flight Tests](https://github.com/Adrian-UniBwM/MLAD-C) -->

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

If you use MLAD-C in your research please cite the following publication: **TBD**

```
@article{dudekCloudDetectionSystemTBD,
  title = {A {{Cloud Detection System}} for {{UAV Sense}} and {{Avoid}}: {{Analysis}} of a {{Monocular Approach}} in {{Simulation}} and {{Flight Tests}}},
  author = {Dudek, Adrian and St{\"u}tz, Peter},
  year = {TBD},
  journal = {TBD},
  volume = {TBD},
  number = {TBD},
  pages = {TBD},
  doi = {TBD},
  abstract = {TBD}
}
```

## Funding

The research project MissionLab is funded by dtec.bw – Digitalization and Technology Research Center of
the Bundeswehr which we gratefully acknowledge. dtec.bw is funded by the European Union –
NextGenerationEU.