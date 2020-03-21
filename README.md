# COVID-19-GHANA
An attempt to create structured data model for COVID-19 cases in Ghana inspired by [COVID-19 Italia](https://github.com/pcm-dpc/COVID-19) and [Novel Coronavirus (COVID-19) Cases, provided by JHU CSSE](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports).

### Data Sources

* [Ghana Health Service - COVID-19](https://www.ghanahealthservice.org/covid19/)
* [Ministry of Information](https://twitter.com/moigovgh/)
* [2020 coronavirus pandemic in Ghana](https://en.wikipedia.org/wiki/2020_coronavirus_pandemic_in_Ghana) - Wikipedia


## Folder Structure

```
COVID-19-GHANA/
│
├── boundaries
│   ├── geojson
│   │   └── ghs-covid19-gha-regions.geojson
│   └── shapefile
│       └── ghs-covid19-gha-regions.shp
├── data-json
    └── ghs-covid19-eng-*.json
├── LICENSE
├── national-data-trend
│   ├── ghs-covid19-eng-national-trend-yyyymmdd.csv
│   ├── ........
│   ├── ghs-covid19-eng-national-trend.csv
│   └── ghs-covid19-eng-national-trend-latest.csv
├── README.md
└── regional-data
    ├── ghs-covid19-eng-regions-yyyymmdd.csv
    ├── .........
    ├── ghs-covid19-eng-regions.csv
    └── ghs-covid19-eng-regions-latest.csv
```
## Data format

### Data by Region

**Directory:** data-regions<br>
**Day file structure:** ghs-covid19-eng-regions-yyyymmdd.csv (ghs-covid19-eng-regions-20200224.csv)<br>
**General file:** ghs-covid19-eng-regions.csv<br>
**Last data files (latest):** ghs-covid19-eng-regions-latest.csv

|Field Name       |Description             |Notes/Example          |
|-----------------|------------------------|-----------------------|
|**date**             | Date                   | YYYY-MM-DD HH:MM:SS   |
|**state**            | ISO 3166-1 alpha 3     | GHA                   |  
|**code**             | ISO 3166-2 code        | GH-TV                 |  
|**region**           | Name of Region         | Volta                 |  
|**lat**              | Longitude              |  10.77978774          |  
|**long**             | Logitude               | -0.80425784           |
|**confirmed**        | New confirmed cases    | 3                     |
|**deaths**           | New death cases        | 3                     |
|**recovered**        | New recovery cases     | 3                     |
|**total_confirmed**  | Overall confirmed cases | 3                     |
|**total_deaths**     | Overall deaths         | 3                     |
|**total_recovered**  | Overall recovery       | 3                     |


### National Data Trend

**Directory:** national-data-tredn<br>
**Day file structure:** ghs-covid19-eng-national-trend-yyyymmdd.csv (ghs-covid19-eng-national-trend-20200224.csv)<br>
**General file:** ghs-covid19-eng-natioanl-trend.csv<br>
**Last data files (latest):** ghs-covid19-eng-national-trend-latest.csv

|Field Name       |Description             |Notes/Example          |
|-----------------|------------------------|-----------------------|
|**date**             | Date                   | YYYY-MM-DD HH:MM:SS   |
|**state**            | ISO 3166-1 alpha 3     | GHA                   |  
|**confirmed**        | New confirmed cases    | 3                     |
|**deaths**           | New death cases        | 3                     |
|**recovered**        | New recovery cases     | 3                     |
|**total_confirmed**  | Overall confirmed cases | 3                     |
|**total_deaths**     | Overall deaths         | 3                     |
|**total_recovered**  | Overall recovery       | 3                     |
|**total_tests**  | Overall number of test cases       | 3                     |