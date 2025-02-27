# spatial-data-viz
Repository with code and materials for EcoDataScience workshop on spatial data visualization

# Learning Outcomes: 
By the end of the session you should be able to:

1. Read in and map spatial data from multiple sources (using `sf`)

2. Add a basemap, scalebar and north arrow to your map

3. Understand how you can use R to streamline the map-making process (using themes and functions)

# Helpful Background:

This workshop will be most helpful if you have spent some time working with data 
in R, either for data analysis or visualization. Specifically, the workshop will be most helpful if you are: 

- comfortable with the basics of working with data in R (reading in data, tidyverse functions, making a graph with ggplot)

- familiar with different types of spatial data (not necessarily working with them in R)

- have an interest in spatial data and learning how R can help you with spatial data visualization (and analysis)

The primary purpose is to demonstrate how to use R to visualize spatial data, rather than give a full tutorial on the basics of geospatial data though we will review some basic concepts quickly. Therefore we may not cover some important concepts that are important for spatial data analysis. For more in-depth learning I recommend reading "Geocomputation with R" by Lovelace et al. (2024), a free ebook available here: [](https://r.geocompx.org/).

# Workshop Prep

1. Install the following packages into R:

- `tidyverse`
- `ggplot2`
- `patchwork`
- `sf`
- `ggspatial`
- `maptiles`
- `terra`
- `tidyterra`
- `tigris`
- `cowplot`
- `prettymapr`
  
Try loading the packages with `library(package_name)` to make sure that all of the dependencies installed correctly - there may be some additional packages you need to install separately

See the “Installing” section for help with installation of the sf package at https://r-spatial.github.io/sf/, as it also requires installation of GDAL, GEOS, and PROJ 

# Data sources
| Data                      | Original Dataset                                 |
|---------------------------|--------------------------------------------------|
| Study Sites               | cj lortie, M Zuliani, Nargol Ghazian, Jenna Braun, S Haas, & Rachel King. 2022. A list of ecological study sites within Central California Drylands. Knowledge Network for Biocomplexity. [doi:10.5063/F1F76B1R](https://doi.org/10.5063/F1F76B1R). |
| California Ecoregions     | U.S. Environmental Protection Agency. 2012. Level IV Ecoregions of California. U.S. EPA Office of Research and Development (ORD) - National Health and Environmental Effects Research Laboratory (NHEERL), Corvallis, OR. [California Level IV Ecoregions](https://www.epa.gov/eco-research/ecoregion-download-files-state-region-9#pane-04) |
| California State Boundary | U.S. Census Bureau TIGER/Line Shapefiles. (2023). [](https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html) |


