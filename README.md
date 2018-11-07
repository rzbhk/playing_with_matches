# playing_with_matches
Repository to host codes and samples of data and results for the study of trip similarity and matching
Preprint available at:
https://arxiv.org/abs/1809.02298

Poster presented at SIGSPATIAL 2018.


### Structure
data -> samples of data. 
#### Note that the big dataset can be retrieved from http://kolntrace.project.citi-lab.fr/
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

### Notebooks description
exploratory_analysis.ipynb -> exploratory analysis 
