# 1km_1hr_global_pr

Input: 10 km IMERG rainfall at 1 hourly (originally IMERG comes at 30-min, so we would have to resample using xarray to 1-hr). Regrid using bilinear/bicubic interpolation in xarray to 1 km

Target: 1 km 1 hr NOAA AORC precipitation 

Loss: NOAA AORC Loss (base model) + Station loss (fine-tuning)

Total period of download: 2000-2024

Fine tuning: use NOAA GHCNh

Raw data: Train over the US predict globally

Fine tuning using the stations over regions of interest

Test different models to select the best model + metrics for extreme precipitation 
