# Installing LSDTopotools in Ubuntu 24.04.1 LTS in 2025
- python=3.10
- conda install conda-forge::lsdtopotools - using https://anaconda.org/conda-forge/lsdtopotools
- pip install lsdviztools
  * Direct usage caused installation problems due to GDAL not being installed due to some version clash of GDAL with other libraries.
  * So installed lsdviztools from source (Git repo)
  * Download from https://github.com/LSDtopotools/lsdviztools.git
  * From the downloaded folder in the conda environment, use - `python setup.py install` to install lsdviztools.
  * GDAL installed using - `conda install conda-forge::gdal` from https://anaconda.org/conda-forge/gdal
  * Other dependencies of lsdviztools such as `fiona`, `rasterio`, `Cartopy`, etc are installed using conda forge.
- lsdtopo3.yml is .yml file contains information about channels and packages (with version) to install. 
