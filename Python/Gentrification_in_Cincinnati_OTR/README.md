# **Gentrification_in_Cincinnati_OTR**

Analysis of the population demographics of the neighborhood Over-The-Rhine (OTR)

![image of OTR](https://cincinnatiusa.com/sites/default/files/styles/Array/public/1_Findlay%20Market_Pramik_1.jpg)
 <b>“Findlay Market.” Cincinnati USA, 22 Dec. 2013,           Cincinnatiusa.com </b>

## **Purpose of this project**

* Analyze official census data to observe changes in demographic populations
    * Census data between years 1950 and 2020
    * Changes in demographics focus on white and Black populations
* Analyze data from American Community Surveys (ACS) to obtain educational and income insights
* Obtain results about historical and current trends for OTR on:
    * White and Black populations (Years 1950 - 2020)
    * Educational attainment (Years 2000 -2020)
    * Median Income (Years 2000 - 2020)
* The ultimate goal is to determine if the neighborhood of OTR:
    * Experienced the social phenomenon of white flight during the 1950s and 1960s
        * Analyzing data and creating visualizations to determine changes in the mentioned populations
    * Is experiencing gentrification for the last 20 years
        * Analyzing data and creating visualizations to determine if changes in the populations are correlated with educational and income changes.

## **Tools used**
* I created spatial visualizations to provide geographic references for the location of OTR, Cincinnati, Hamilton County, and Ohio State within the United States.
    * For that purpose, I use Geopandas and Contextily libraries 
    * I used a geojson file from CensusReporter website
* I analyze census data to obtain a demographic trend between years 1950 – 2020 for white and Black populations
    * I used pandas library to create different dataframes of the demographic data
    * I used official census data sets from Social Explorer website 
* I analyze educational attainment and median income
    * I used pandas library to create different dataframes of the demographic data
    * I used ACS surveys from Social Explorer website


## **Setup**

* **Clone the project and move into its directory**
    * git clone https://github.com/JesusLopezCalvo/Gentrification_in_Cincinnati_OTR.git

* **Install the needed packages:**
    * In order to avoid problems installing contextily library I recommend installing first required distutils packages for that library 
        * Using command pip:  pip install <name of the distutil>
        * Required-Dist:
            * Geopy
            * Matplotlib
            * Mercantile
            * Pillow
            * Requests
            * Joblib
            * Xyzservices
    * After installing those libraries, I recommend installing rasterio and geopandas libraries using the conda-forge command for anaconda 
        * conda install -c conda-forge rasterio
        * conda install --channel conda-forge geopandas
    * Once all those packages are installed you can install the rest by using the command:
        * pip install -r requirements.txt

* **Run the notebook**
    * Run the jupyter lab notebook 
        * Project.ipynb 


## **Features used**
* **Import and read data**
    * I used pandas.read_excel to read in data from a local excel file.
* **Manipulation and cleaning of the data**
    * Use built-in pandas or numpy functions to manipulate and clean my dataframes
    * Removed all rows and columns that were not necessary for this project
* **Analysis of the data**
    * I used geopandas and contextily to create spatial visualizations
    * I created new dataframes incorporating the demographic information from each of the excel files of the census data
        * For that purpose, I used functions like loops, lists, or dictionaries.
    * I used statistical methods to analyze the data
        * I calculated the Pearson coefficient (Coefficient r) to obtain the correlation between years and white population with the objective to identify a trend in the increase of the mentioned population
* **Visualization of the data**
    * For the spatial visualizations I used the geopandas library
    * To create the basemaps I used the contextily library
    * I used matplotlib to create different plots and subplots 
        * Bar graphs to identify variations in the populations, educational attainment, and median income
        * Scatter plots with regression line to identify positive or negative trends in the populations
* **Interpretation of the data**
    * I used Markdown cells in the Jupyter Lab notebook explaining the process and code interpretation of the data’s output

## **Resources used for Data sets**

* [Social Explorer](https://www.socialexplorer.com/a9676d974c/explore "Census Data Sets")

* [Census Reporter](https://censusreporter.org/data/table/?table=B03002&geo_ids=16000US3915000,05000US39061,31000US17140,04000US39,01000US,140|16000US3915000&primary_geo_id=16000US3915000 "Census Data for spatial visualizations")

## Badges 
### 1. GitHub Stats
![Your Repository's Stats](https://github-readme-stats.vercel.app/api?username=JesusLopezCalvo&show_icons=true)
### 2. Most Used Languages
![Your Repository's Stats](https://github-readme-stats.vercel.app/api/top-langs/?username=JesusLopezCalvo&theme=blue-green)
### 3. Contributors Badge
![Your Repository's Stats](https://contrib.rocks/image?repo=JesusLopezCalvo/Gentrification_in_Cincinnati_OTR)
### 4. Random Joke Generator
![Jokes Card](https://readme-jokes.vercel.app/api)
### 5. Profile View Counter
![Profile View Counter](https://komarev.com/ghpvc/?username=JesusLopezCalvo)