## PyFlowline workflow

### Overview

PyFlowline generates the conceptual river networks based on two major inputs:

1. vector-based river flowlines
2. mesh

### USGS National Hydrography Dataset river flowline processing

In this study, we used the United States Geologic Survey National Hydrography Dataset (NHD) flowlines.
The raw NHD flowline dataset contains more than 10, 000 flowlines and cannot be used by our study.

The following operations are used to pre-processing the raw NHD flowlines. 

1. The stream order is used to remove small rivers (In QGIS).
2. The filtered flowlines are converted to the GeoJSON format (In QGIS).

### Install the PyFlowline package

Install the Pyflowline package using Conda (recommended):

    conda install -c conda-forge pyflowline

### Data preparation

1. Configure the path in the JSON files under the `example` folder.
2. Set up model parameters, e.g., mesh resolution.

### Run simulation

Run the simulations using the `run_susquehanna.py` script using your preferred Python environment.

Correct errors if there are issues in the path configuration.

### Visualization

Two types of output are available under the outpur folder
1. JSON files, contain information of mesh and flowline topological relationship;
2. GeoJSON files, contain conceptual flowlines in the `GIS` format. These files can be visualized directly using QGIS.

