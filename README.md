# AdminR Packages

A curated list of R packages created and used by Swiss public institutions


### About

We try to collect and classifly R packages that are are created and used by Swiss statistical offices. This should facilitate colaboration and reduce duplication. We try structure the package list and to present and discuss it on the AdminR Session at the [**Swiss Statistics Meeting 2021**](https://www.statistiktage.ch/en/) on the 6th of Semptember 2021 in Lugano.

Ideally, the listed packages are publicly available, either on CRAN or on GitHub. If this is not possible, an entry should explan how one could get to the package. You may also list interesting packages that are not yet public.


### How to list your package

To list your R package:

- Write a comment on issue [#1](https://github.com/swiss-adminR/pkgs/issues/1) (recommended),
- or send us [an email](ronald.indergand@seco.admin.ch).

Please inclue a title, a short description and mention the users of your package. Have a look at the first entry for a reference.




## Data Handling

#### [cubustat: Data Cubes Published by the Statistical Office of Canton Ticino](https://gitlab.com/gibonet/cubustat)

This R package contains data cubes published by the statistical office of Canton Ticino (Ustat). All the data cubes are data.tables in long format, with only one numerical column. These results can also be downloaded in 3 formats (csv, xlsx, px) from the [Ustat website](https://www3.ti.ch/DFE/DR/USTAT/index.php?fuseaction=interattivi.tabelle_interattive).

**Used by:** Statistical office of Canton Ticino (Ustat)


#### [cubiapp: Shiny App for Filtering and Reshaping Information from Data Cubes](https://gitlab.com/gibonet/cubiapp)

Shiny app to extract and reshape information from data cubes (from the Ustat site but with other data too). The package also contains shiny modules that could be used to create other shiny apps.

**Used by:** Statistical office of Canton Ticino (Ustat)


#### **[kofdata: Get Data from the 'KOF Datenservice' API](https://cran.r-project.org/web/packages/kofdata/index.html)**

Read Swiss time series data from the 'KOF Datenservice' API, <https://datenservice.kof.ethz.ch>. The API provides macro economic time series data mostly about Switzerland. The package itself is a set of wrappers around the 'KOF Datenservice' API. The 'kofdata' package is able to consume public information as well as data that requires an API token.

**Used by**: KOF Swiss Economic Institute, SNB, several cantonal statistical offices


## Statistical Routines

#### [tempdisagg: Methods for Temporal Disaggregation and Interpolation of Time Series](https://cran.r-project.org/web/packages/tempdisagg/index.html)

temporal disaggregation methods are used to disaggregate and interpolate a low frequency time series to a higher frequency series, where either the sum, the mean, the first or the last value of the resulting high frequency series is consistent with the low frequency series.

**Used by:** State Secretariat of Economic Affairs


#### [seasonal: R Interface to X-13-ARIMA-SEATS](https://cran.r-project.org/web/packages/seasonal/index.html)

Easy-to-use interface to X-13-ARIMA-SEATS, the seasonal adjustment software by the US Census Bureau.

**Used by:** State Secretariat of Economic Affairs



## Publication, Communication


#### [admindown: CD-Bund Compatible R Markdown Theme](https://github.com/swiss-adminR/admindown)

Admindown provides an R Markdown template in line with the corporate design of the federal government of Switzerland.

**Used by:** State Secretariat of Economic Affairs; others

**How to access:** This is a private repo, access is granted to any federal office. [Just drop an email](mailto:angelica@cynkra.com).


#### [statR: Corporate Design Toolbox for the Canton of Zurich](https://github.com/statistikZH/statR)

statR provides functions to export nicely formatted .xlsx, color palettes, a ggplot theme and a html template to create data products with the corporate design of the canton of Zurich.

**Used by:** Statistical Office Canton of Zurich; others


#### [swissdd](https://github.com/politanch/swissdd)

swissdd builds upon real time data service for federal and cantonal votes provided by the Federal Statistical Office via opendata.swiss. It brings the results of popular votes, aggregated at the geographical level of choice, straight into R. 

**Used by:** Statistical Office Canton of Zurich; others


