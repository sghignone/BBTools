# BBTools
[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/4220)

BBTools is a suite of fast, multithreaded bioinformatics tools designed for analysis of DNA and RNA sequence data.

## RQCFilter2
RQCFilter2 is a revised version of RQCFilter that uses a common path for all dependencies.
The dependencies are available at http://portal.nersc.gov/dna/microbial/assembly/bushnell/RQCFilterData.tar

Performs quality-trimming, artifact removal, linker-trimming, adapter trimming, and spike-in removal using BBDuk.
Performs human/cat/dog/mouse/microbe removal using BBMap.
It requires 40 GB RAM for mousecatdoghuman, but only 1GB or so without them.

Usage:  rqcfilter2.sh in=<input file> path=<output directory> rqcfilterdata=<path to RQCFilterData directory>

