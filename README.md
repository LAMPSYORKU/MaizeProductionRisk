# MaizeProductionRisk
This repository is used to store raw data, calculated data, programs and software package list for the paper "Climate change poses significant risks to maize production over the Great Lakes region"

## 1. Work environment setting 
### 1.1 Download and install anoconda3 packages for 64-bit Windows with Python 3.8
#### <pre>conda create --name climada_env</pre>
#### <pre>conda activate climada_env</pre>
#### <pre>conda install numpy</pre>
#### <pre>conda install padas</pre>
#### <pre>conda install matplotlib</pre>
#### <pre>conda install cartopy</pre>
#### <pre>conda install xarray</pre>
#### <pre>pip install -e climada_python</pre> [https://climada-python.readthedocs.io/en/stable/guide/Guide_Installation.html]
#### <pre>pip install -e climada_petals</pre> [https://climada-python.readthedocs.io/en/stable/guide/Guide_Installation.html]
#### <pre>conda install -c anaconda jupyter</pre>

## 2.Download data
### Note: all links are in the github subdirectory: https://github.com/LAMPSYORKU/MaizeProductionRisk/tree/main/raw_data

### <pre>mkdir climada_work</pre>
### <pre>cd climada_work</pre>
### copy Historical_RCP26_RCP60_file_list.txt (in the raw_data directory) to climada_work/
### <pre>wget -ci Historical_RCP26_RCP60_file_list.txt</pre> to download all historical simulation and future projection data to current work directory
### dircetly download land use data (https://github.com/LAMPSYORKU/MaizeProductionRisk/blob/main/raw_data/histsoc_landuse-15crops_annual.txt) and spam production data (https://github.com/LAMPSYORKU/MaizeProductionRisk/blob/main/raw_data/Grided_Production_bySPAM_file_list.txt)

## 3. Analyze data with python program following the guidance of climada_petals
### All calculated data are in the github subdirectory: https://github.com/LAMPSYORKU/MaizeProductionRisk/tree/main/calculated_data
### All of the following code is in the github subdirectory: https://github.com/LAMPSYORKU/MaizeProductionRisk/tree/main/code/ipynb
### All public software packages links are listed in file https://github.com/LAMPSYORKU/MaizeProductionRisk/blob/main/code/Public_softwarepackages_links.txt
### All generated figures are in the github subdirectory: https://github.com/LAMPSYORKU/MaizeProductionRisk/tree/main/FIGURES
### The summary statistical analysis table is in the github subdirectory: https://github.com/LAMPSYORKU/MaizeProductionRisk/tree/main/Tables

### Program 1: display_geotiff_gridded_production_data-2000.ipynb,display the global grid production in 2000, extract and save the data of the study area
### Program 2: display_geotiff_gridded_production_data-2005.ipynb,display the global grid production in 2005, extract and save the data of the study area
### Program 3: display_geotiff_gridded_production_data-2010.ipynb,display the global grid production in 2010, extract and save the data of the study area
### Program 4: display_geotiff_gridded_production_data_upscape_05x05.ipynb,upscale production data from 10km X 10km to 0.5Lon X 0.5Lat to match the resoltuon of ISIMIP data and save the data
### Program 5: Calculate_gridcell_area_in_squared_meters.ipynb, convert 0.5Lon X 0.5Lat to area in unit square meter m^2 then to unit ha to match unit in ISIMIP data
### Program 6: ISIMIP_analysis_Historical_Yield-RCP26.ipynb, calculate historical (1986-2005,1996-2005) simulation,and future projections 2050s (2040-2069) and 2080s (2070-2099) 30-year *16-model ensemble mean yield at each gridcell under the climate change senario RCP2.6. 
### Program 7: ISIMIP_analysis_Historical_Yield-RCP60.ipynb, calculate historical (1986-2005,1996-2005) simulation,and future projections 2050s (2040-2069) and 2080s (2070-2099) 30-year *16-model ensemble mean yield at each gridcell under the climate change senario RCP6.0. 
### Program 8: Relative_crop_yield_intensity.ipynb, calculate relative crop yield intensity relative to the reference period 1996-2015 under RCP 2.6 and RCP 6.0
### Program 9: FIGURE1_ISIMIP_analysis_landuse_1986_2005.ipynb, analysis and compare land use data, at last we use the last 10 year land used data in this study.Plot figure 1
### Program 10: FIGURE2_new_ISIMIP_analysis_Historical_Yield_time_series_analysis.ipynb, Check model result, estimate uncertainty, identify uncertainty source and plot figure 2
### Program 11: FIGURE3_new_ensemble_mean_of_simulated_maize_yields.ipynb, plot relative crop yield intensity for the future period under the two RCPs
### Program 12: Estimate crop production risk and draw risk map, statistical analysis to check risk range in space
### Program 13: table1_a_Find_gridcells_in_each_USA_states_Canada_province.ipynb, find grid cell in each state in USA or province in Canada within study area
### Program 14: table1_b_summary_states_provinces.ipynb, Summary Analysis of Crop Risk Statistics by States of the United States and Provinces of Canada
