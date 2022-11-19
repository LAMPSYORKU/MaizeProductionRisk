# MaizeProductionRisk
This repository is used to store raw data, calculated data, programs and software package list for the paper "Climate change poses significant risks to maize production over the Great Lakes region"

## 1. Work environment setting 
### 1.1 Download and install anoconda3 packages for 64-bit Windows with Python 3.8
### 1.2 conda create --name climada_env
### 1.3 conda activate climada_env
#### 1.3.1 conda install numpy
#### 1.3.2 conda install padas
#### 1.3.3 conda install matplotlib
#### 1.3.4 conda install cartopy
#### 1.3.5 conda install xarray
#### 1.3.6 pip install -e climada_python [https://climada-python.readthedocs.io/en/stable/guide/Guide_Installation.html]
#### 1.3.7 pip install -e climada_petals [https://climada-python.readthedocs.io/en/stable/guide/Guide_Installation.html]
#### 1.3.8 conda install -c anaconda jupyter

## 2.Download data
### mkdir climada_work
### cd climada_work
### copy Historical_RCP26_RCP60_file_list.txt (in the raw_data directory) to climada_work/
### wget -ci Historical_RCP26_RCP60_file_list.txt to download all historical simulation and future projection data to current work directory
### dircetly download land use data and spam production data

## Analyze data with python program following the guidance of climada_petals

