# Playing with Matches: Vehicular Mobility through Analysis of Trip Similarity and Matching

Repository to host codes and samples of data and results for the study of trip similarity and matching
Preprint available at:
https://arxiv.org/abs/1809.02298

Poster presented at SIGSPATIAL 2018.

#### contact me at the email address in the pdf if you have any questions!

### Structure
* data : samples of data. 
     * -> koln_by_hour_OD_and_scaled.h5 (~30MB) : Origins and Destinations of trips extracted for 4 1-hour time windows.
     * -> koln_by_hour.h5 (3.4 GB) NOT INCLUDED in REPO (URL will be posted) : all waypoints per hour groups extracted from raw data
#### Note that the big dataset (raw) can be retrieved from http://kolntrace.project.citi-lab.fr/
#### Note that you must update the input file locations to where you store them on your drive.
notebooks -> jupyter (python) notebooks



### Requirements
Everything was done in python. The packages in our conda environment are exported to conda-requirements.txt (and pip frozen to requirements.txt if you prepare pip and python venvs).

For conda:
> conda create --name <envname> --file conda-requirements.txt
  
For pip and venv:
> python3 -m virtualenv env

On macOS and Linux:
> source env/bin/activate

On Windows:
> .\env\Scripts\activate

> pip install -r requirements.txt

### Instructions
- activate your virtual env and inside run a jupyter notebook.
- update the file paths in the notebook to the location that you store data on your disc.
- run the notebook cell by cell! 

### Notebooks description

- exploratory_analysis.ipynb -> a ton of exploration and visualization on samples of data.
- literature_metrics_comparison_on_CaR.ipynb -> comparison to LCSS, Frechet, and DTW 
- similarity_trip_clustering_spatial_only.ipynb -> clustering using only distances
- similarity_trip_clustering_spatial_temporal_combined.ipynb -> wgm of *mean* of dist and time elemenets
- similarity_trip_clustering_temporal_only.ipynb -> clustering using only time
- similarity_trip_clustering_OD.ipynb -> mean of pointwise wgm used for clustering
- similarity_trip_OD_CARSHARING_V3_DAG.ipynb -> matching and scheduling carsharing scenario
- similarity_trip_realtime_matching_just_OD_CARPOOL.ipynb -> thresholds and matching for CARPOOL scenario
- similarity_trip_realtime_matching_just_OD_CaR.ipynb -> thresholds and matching for Catch-a-Ride

