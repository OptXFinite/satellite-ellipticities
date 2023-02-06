# satellie-ellipticities
A suite of analyses on the spatial distribution of satellite galaxies around their hosts using obersevational satellite data from the [SAGA survey](https://sagasurvey.org/) and simulated dark matter data from the [CosmoSim VSMDPL simulation](https://www.cosmosim.org/metadata/vsmdpl/)

## Features
- Compare the distribution of SAGA satellite system ellipticities measured to simulated dark matter subhalo ellipticities
- Plot features of host galaxy against ellipticity measurements
- Evaluate the prominence of each satellite or subhalo system with respect to a random distribution


## Dependencies
- Use of public SAGA data requires the installation of the [SAGA](https://github.com/sagasurvey/saga#installation) package
```
conda install git pip
pip install git+git://github.com/sagasurvey/saga.git
```
- VSMDPL data may be similarly downloaded via their website. This package assumes it is downloaded as a parquet
- all other python dependencies are listed in the requirements.txt file

to install a new conda environment called ``satellite-ellipticities`` with all dependencies, run the following inside the top directory
```
$ conda env create
$ conda activate satellite-ellipticities
```

or to install packages via pip:
```
$ pip install -r requirements.txt
```

## Env
- You need to supply the paths to your local copies of 4 data sets in a .env file which will be gitignored. A fifth environment variable, the SAGA_DB will be a remote path which need also be added to your .env file. 