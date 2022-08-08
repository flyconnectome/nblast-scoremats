# NBLAST score matrices

NBLAST is an algorithm to quantify morphological similarity between neurons. Its second
version (Costa et al., 2016) uses a 2D scoring matrix to determine whether two points 
(or rather the distance between them and the dot product of their vectors) are indicative 
of two neurons belonging to the same type or not. 

The original scoring matrix was generated using neurons from the FlyCircuit project - 
i.e. _Drosophila_ neurons skeletonized from confocal stacks co-registered to a template brain. 
Despite being created for fly neurons and from light-level data it works surprisingly well
for other types of data (e.g. EM-derived skeletons) and organisms. That said: there is 
probably mileage in generating specialised scoring functions for certain applications. 

This repository collects alternative scoring matrices that you can plug into e.g. the
Python implementation in `navis` or the R implementation in `nat`.

Contributions welcome!

## Scoring matrices 

### FlyCircuit 
`scoremats/fcwb.csv` is the original scoring matrix made from light-level data of _Drosophila_ co-registered to the same template space.

### hemibrain
`scoremats/hemibrain.csv` was generated from _Drosophila_ neurons from the Janelia hemibrain connectome.

## How to use

TODO

## How to generate your own

TODO
