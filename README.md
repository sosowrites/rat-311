# Analysis of 311 request data — 11/2026
Advanced Data Assignment 1
This repository contains data, analytic code, and findings that support portions of the article, “[Rodents Queen Out In Astoria](https://docs.google.com/document/d/1_pu61AvrjtsfESy_vQ_SliJVEUCsD5Ecxuc7X33hIdU/edit?usp=sharing),” published November 2, 2026. Please read that article, which contains important context and details, before proceeding.

## Data

This analysis uses one csv of all the 311 requests made from July 26, 2026 to October 26, 2026.  

The spreadsheet comes from the following sources:

- Name of source:
  - `311_Service_Requests_from_2020_to_Present_20261026.csv`: Raw data of all the 311 requests, pulled from NYC open data.

Each of the spreadsheets contain, among others, the following columns relevant to the analysis:

- `Problem` — The general category of 311 request. 
- `Problem Detail` — Additional detail about the request.
- `Incident Zip` — The zip code the request is coming from.
- `Borough` — The borough the request is coming from.

## Methodology

The notebook [`rat-311.ipynb`](notebooks/rat-311.ipynb) performs the following analyses:

##### Part 1: Analyze rodent-related 311 requests

- First, I pulled the 311 requests specifically categorized under Rodent. Then I narrowed it down further, and pulled the data related to rat and mouse sightings (excluded data for requests reporting conditions attracting rodents, e.g.)
- Within this data, I analyzed which zip codes and boroughs made the most rodent-related 311 requests. 

##### Part 2: Do the same for graffiti and party/loud noise requests. 
- I repeated the above steps for 311 requests related to graffiti, and then to parties/loud noises. 


## Outputs

The notebooks output this spreadsheet which contains the zip codes of all rodent sighting 311 data, so that I could create a visualization in DataWrapper: [`rodent_zip.csv`](rodent_zip.csv).

## Running the analysis yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:

- Python 3
- The Python libraries specified in [`requirements.txt`](requirements.txt)

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). The data file in the output/ directory is available under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

## Feedback / Questions?

Contact Sohini Desai at sohini.desai74@journalism.cuny.edu.
