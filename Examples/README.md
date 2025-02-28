# Examples

<p align="center">
  <img src="https://static1.squarespace.com/static/596d24cd4402430bb863ffad/t/5b41e62603ce641f98f2e3cd/1536741696061/?format=1500w" width="350" title="hover text">
</p>

To help get you started, this folder contains some example programs covering topics like vehicle classification, proximity filtering, plotting and more.

## Jupyter Notebooks (Python)

**Zone11_EDA_demo.ipynb** - This Jupyter Notebook has general AIS data exploration, AIS data plotting, vessel type classification and anomoly detection analysis. If you are new to AIS data, this is a good introduction and will give you a good feel for the data and how it can be used.

**AnalysisAndClassification.ipynb** - This Jupyter Notebook has data cleaning functions, proximity filtering, encounter categorization, and vessel and size prediction analysis.

## Mathematica Notebooks

**Fast_Stochastic_Proximity_Pairs_Finder.nb** - This Mathematica Notebook takes chunks of the AIS data from Marine Cadastre, typically 100,000 lines at a time, partitions the data into groups of 200 with a 100 element sliding offset. It then randomly queries entries for being within 8000 yards within 10 minutes. It is set up to have a time limit to the computation, and quickly finds a majority of the interactions, though it takes a while to get all interactions.

**AISDataProximity.nb** - This Mathematica Notebook imports AIS data from Marine Cadastre, splits the CSV files into smaller chunks by line count, and further splits it by hour.

**AIS_Task.nb** - This Mathematica Notebook imports AIS data from Marine Cadastre and splits the data by day in order to reduce the file size to something more manageable. It also has functions to do basic deterministic proximity filtering and path interpolation.

**AIS_mk4.nb** - This Mathematica Notebook has an implementation of a stochastic divide-and-conquer algorithm for fast proximity filtering. It splits the data by truncating the time, lattitude and longitude and then randomly tests for proximity under a threshold.

**AISmk3.nb** - This Mathematica Notebook has some file-handling functions for splitting large CSV files as well as several successive file size reduction techniques in order to reduce the search space for proximity filtering.


<p align="center">
  <img src="https://static.wixstatic.com/media/3d35e8_2d9eb95a4abe4869afafbf51d29038dc~mv2.png/v1/fill/w_288,h_60,al_c,usm_0.66_1.00_0.01/3d35e8_2d9eb95a4abe4869afafbf51d29038dc~mv2.png" width="150" title="hover text">
</p>
