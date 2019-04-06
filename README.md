## Overview
This repo was an experiment in creating a spatially partitioned data structure
for use with the Datashader project. See https://github.com/pyviz/datashader/issues/678
for more background.

It was integrated into Datashader in [pyviz/datashader#702](https://github.com/pyviz/datashader/pull/702) and [pyviz/datashader#702](https://github.com/pyviz/datashader/pull/706)

![](notebooks/osm-one-billion.gif)

## nbviewer Notebooks
 1. [Spatial partitioning of Dask DataFrames using Hilbert curves](https://nbviewer.jupyter.org/github/jonmmease/hilbert_frame/blob/master/notebooks/1-HilbertCurvePartitioningOverview.ipynb)
 2. [Hilbert-curve spatial data structure performance on 300 million point census dataset](https://nbviewer.jupyter.org/github/jonmmease/hilbert_frame/blob/master/notebooks/2-HilbertCurvePartitioningCensusExample.ipynb)
 3. [Faster interactive exploration of 1 billion points](https://nbviewer.jupyter.org/github/jonmmease/hilbert_frame/blob/master/notebooks/3-HilbertCurveOneBillionInteractive.ipynb)

## Credits
The hilbert curve implementation is a 2D specialization and numba optimization of the excellent work
by @galtay in https://github.com/galtay/hilbert_curve
