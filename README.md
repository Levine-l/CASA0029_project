# CASA0029_project

pp_data is the house trading data, where the fist part including ny,se,so,st,ta,tg,tq areas, and the second part include the remaining.

flood zone 2-3 tiles mapbox： levineliu.2n6exn8k

oa level 2018-2025 average houses price paid data by area (areas I think may include the regions that effected by flood most):
ny: levineliu.9ourp5qg
tg: levineliu.dt8lt8zc
ta: levineliu.aohw3xu9
st: levineliu.71vz336b
tq: levineliu.3w3nswk7
se: levineliu.40f0lqf6
so: levineliu.62ncteef


buildings in four cities in mapbox(Z10 - 16):
London: levineliu.89ciem4a
York: levineliu.drsadjct
Hull: levineliu.6oin1hba
Yarmouth: levineliu.099ee9on


# UK Flood Risk and Property Prices  MAP
### CASA0029 Urban Data Visualisation Group 8

This repository contains the web based visualisation output for group project. The project explores the relationship between flood risk zones and residential property prices in selected areas of England.

The visualisation combines Flood Zone 2/3 data, house price records, Output Area-level price summaries, postcode-level price indicators, and 3D building context. It is designed as an interactive Mapbox-based website where users can inspect how flood exposure overlaps with housing price patterns across different city case studies.

## Live Website

https://levine-l.github.io/CASA0029_project/

## Project Aim

The project asks how flood exposure and property price patterns can be visualised together to support an urban analytics narrative.

Rather than treating flood zones and housing prices as separate datasets, the website brings them into the same spatial interface. Users can compare:

Flood Zone 2 and Flood Zone 3 areas;
Output Area-level average property prices;
postcode level house price per square metre indicators;
local building context in selected city cases;
summary comparisons between properties inside and outside flood zones.
Main Visualisation Features

The website includes:

an interactive Mapbox GL JS map;
Flood Zone 2 and Flood Zone 3 vector tile layers;
Output Area level average house price choropleth layers;
3D building layers for selected city case studies;
city navigation controls;
price classification legend;
flood zone legend;
precomputed comparison summaries;
price trend data by flood zone category.

The current city case studies include:

London;
York;
Hull;
Great Yarmouth.

These locations were selected to represent different flood contexts, including river flooding, coastal flooding, surface water exposure, and mixed urban flood risk.

## Repository Structure
CASA0029_project/
│
├── index.html
│   Main website file. Contains the Mapbox web map, layer controls,
│   legends, city navigation, and interactive visualisation interface.
│
├── README.md
│   Repository documentation.
│
├── .gitattributes
│   Git configuration file.
│
├── data/
│   Precomputed JSON files used directly by the website.
│
│   ├── flood_price_compare_precomputed.json
│   │   Precomputed comparison statistics for property prices inside
│   │   and outside flood zones.
│   │
│   └── price_trend_by_zone.json
│       Price trend summary data grouped by flood zone category.
│
├── hpm_processed/
│   Processed house price per square metre and Output Area level files.
│
│   ├── oa21_hpm_priceper.csv
│   │   Output Area-level processed house price per square metre data.
│   │
│   └── postcode_hpm_selected.csv
│       Selected postcode-level house price per square metre data.
│
└── pp_data/
    Processed / compressed Price Paid Data outputs.
    
    ├── pp_all_years_avg_selected_region.zip
    │   Average Price Paid Data for selected regions.
    │
    └── pp_all_years_postcode_avg_remaining.zip
        Average postcode-level Price Paid Data for remaining areas.


## Mapbox Tilesets

Several Mapbox hosted tilesets are used in the web map.

Flood Zone 2/3 tileset:
levineliu.2n6exn8k

Output Area Price Layers
Average house price paid data by Output Area for selected postcode regions:
ny: levineliu.9ourp5qg
tg: levineliu.dt8lt8zc
ta: levineliu.aohw3xu9
st: levineliu.71vz336b
tq: levineliu.3w3nswk7
se: levineliu.40f0lqf6
so: levineliu.62ncteef


3D Building Layers
Building tilesets for selected city case studies:
London:        levineliu.89ciem4a
York:          levineliu.drsadjct
Hull:          levineliu.6oin1hba
Great Yarmouth: levineliu.099ee9on
