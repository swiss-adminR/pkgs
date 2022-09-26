# adminR Code Base

*A curated list of R packages & R code created and used by Swiss public institutions*

---
### About 

Mid 2021, we started to collect and classify R packages that are are created and used by Swiss statistical offices to facilitate collaboration and reduce duplication. We presented and discussed this first list on the adminR Session at the [**Swiss Statistics Meeting 2021**](https://www.statistiktage.ch/images/pdfs/2021/Programm_Statistiktage_2021.pdf) on the 6th of September 2021 in Lugano.

In the meantime, following the [**adminR-Spring Meetup in Aarau**](https://www.meetup.com/adminr/events/285121068/) (May 31 2022), we have further developed the idea to build and curate a set of R packages or R code in general as an infrastructure for federal and cantonal official statistics. 

Ideally, the listed packages or scripts are publicly available, either on CRAN or on GitHub. If this is not possible, an entry should explain how one could get to the package. You may also list interesting packages that are not yet public.

---
<table>
  <thead bg-color="#FFFFE0;">
    <tr>
      <td align="left">
        <h3> ℹ️ How to list your package </h3><br>
        <ul>
         <li> Write a comment on issue <a href="https://github.com/swiss-adminR/pkgs/issues/1">#1</a> (recommended)</li>
         <li> or send us <a href = "ronald.indergand@seco.admin.ch">an email</a></li>
         <li> Please include a title, a short description and mention the users of your package or scripts.</li>
         <li> Have a look at the first entry for a reference.</li>
        </ul>      
      </td>
    </tr>
  </thead>
</table>
 
 



### Table of contents
- [Data Handling](https://github.com/swiss-adminR/pkgs#data-handling)
- [Statistical Routines](https://github.com/swiss-adminR/pkgs#statistical-routines)
- [Visualization](https://github.com/swiss-adminR/pkgs#visualization)
- [Data Handling](https://github.com/swiss-adminR/pkgs#data-handling)
- [Publication, Communication](https://github.com/swiss-adminR/pkgs#publication-communication)
- [Specific Data](https://github.com/swiss-adminR/pkgs#specific-data)


## Data Handling

#### [cubustat: Data Cubes Published by the Statistical Office of Canton Ticino](https://gitlab.com/gibonet/cubustat)

This R package contains data cubes published by the statistical office of Canton Ticino (Ustat). All the data cubes are data.tables in long format, with only one numerical column. These results can also be downloaded in 3 formats (csv, xlsx, px) from the [Ustat website](https://www3.ti.ch/DFE/DR/USTAT/index.php?fuseaction=interattivi.tabelle_interattive).

**Used by:** Statistical office of Canton Ticino (Ustat)


#### [cubiapp: Shiny App for Filtering and Reshaping Information from Data Cubes](https://gitlab.com/gibonet/cubiapp)

Shiny app to extract and reshape information from data cubes (from the Ustat site but with other data too). The package also contains shiny modules that could be used to create other shiny apps.

**Used by:** Statistical office of Canton Ticino (Ustat)


#### [kofdata: Get Data from the 'KOF Datenservice' API](https://cran.r-project.org/web/packages/kofdata/index.html)

Read Swiss time series data from the 'KOF Datenservice' API, <https://datenservice.kof.ethz.ch>. The API provides macro economic time series data mostly about Switzerland. The package itself is a set of wrappers around the 'KOF Datenservice' API. The 'kofdata' package is able to consume public information as well as data that requires an API token.

**Used by**: KOF Swiss Economic Institute, SNB, several cantonal statistical offices


## Statistical Routines

#### [tempdisagg: Methods for Temporal Disaggregation and Interpolation of Time Series](https://cran.r-project.org/web/packages/tempdisagg/index.html)

temporal disaggregation methods are used to disaggregate and interpolate a low frequency time series to a higher frequency series, where either the sum, the mean, the first or the last value of the resulting high frequency series is consistent with the low frequency series.

**Used by:** State Secretariat of Economic Affairs


#### [seasonal: R Interface to X-13-ARIMA-SEATS](https://cran.r-project.org/web/packages/seasonal/index.html)

Easy-to-use interface to X-13-ARIMA-SEATS, the seasonal adjustment software by the US Census Bureau.

**Used by:** State Secretariat of Economic Affairs


## Visualization

#### [catmaply: interactive heatmaps](https://github.com/VerkehrsbetriebeZuerich/catmaply)

This R package specifically focuses on providing an efficient way for creating interactive heatmaps for categorical data or continuous data that can be grouped into categories.

**Used by:** Stadt Zürich - Verkehrsbetriebe (VBZ) and others



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



## Specific Data

#### staagBevproj

This package projects the population of canton Aargau at cantonal or regional level based on the demographic model of the Swiss Federal Statistical Office (FSO) released in May 2020.

**Used by**: Statistik Aargau (internal application).

**How to access**: This package is not available in a public repository. Send us an [email](mailto:tina.cornioley@ag.ch).


#### staaggemeindeport

This package contains the entire collection of code for the shiny app Gemeindeporträt Kanton Aargau which is published here: https://www.ag.ch/app/statistik_aargau_gemeindeportraet/. The app is based on public data published by Statistik Aargau (accessible via different APIs or [the official website](https://www.ag.ch/de/dfr/statistik/statistik.jsp)).

**Used by:** Statistik Aargau (internal application).


**How to access:** The package / Code has not been published online yet. Send us an [email](mailto:nelson.stevens@ag.ch).


#### [MCMTdatalistcreation: functions to import MZMV raw data and organize it in a list class R data object](https://gitlab.com/MicheleUSTAT/mcmtdatalistcreation)

This is the first out of three packages that were created to analyze the BFS "Mikrozensus Mobilität und Verkehr (MZMV) 2015" data. The analysis functions that are included in the MCMTdataanalysis package need a specific data input argument. Since the MZMV data can not be shared freely we created a function that will automatically create this data argument given a path to a folder that contains the original BFS data. This package is intended to be used as the first step to analyze the MZMV thanks to the MCMTdataanalysis package functions.

**Used by:** Statistical office of Canton Ticino (Ustat)

#### [MCMTdataprep: functions to select, clean and recode the MZMV 2015 data](https://gitlab.com/MicheleUSTAT/mcmtdataprep)

The aim of this package is to provide a set of tools to select, clean and prepare the "Mikrozensus Mobilität und Verkehr (MZMV)" raw data, to be then analyzed with the MCMTdataanalysis package functions.
The MCMTdataprep functions will make use of the data object previously created with the MCMTdatalistcreation package. It will import the data, and select, clean and recode the variables needed to produce the BFS [A2](https://www.bfs.admin.ch/bfs/de/home/statistiken/kataloge-datenbanken/tabellen.assetdetail.2004971.html) table. This package is intended to be used as the second step to analyze the MZMV data. The MZMV data must be first passed through these functions to be analyzed thanks to the MCMTdataanalysis package.

**Used by:** Statistical office of Canton Ticino (Ustat)

#### [MCMTdataanalysis: functions to analyze the MZMV 2015](https://gitlab.com/MicheleUSTAT/mcmtdataanalysis)

This package was created with the purpose to analyze the "Mikrozensus Mobilität und Verkehr (MZMV)" based on the BFS methodology. These functions allow any user to reproduce the results as presented in the BFS table [A2](https://www.bfs.admin.ch/bfs/de/home/statistiken/kataloge-datenbanken/tabellen.assetdetail.2004971.html).
The package makes use of the the [distrr](https://cran.r-project.org/web/packages/distrr/index.html) package, to build data cubes, and therefore to produce results in addition to those in the BFS table. This package is meant to be used after having processed the raw data with the MCMTdatalistcreation and MCMTdataprep packages.
This package will be furthermore deveolped to add new features.

**Used by:** Statistical office of Canton Ticino (Ustat)

#### rpango

The goal of rpango is to allow access the SARS-CoV-2 pango nomenclature as a tree object in R. This simplifies the manipulation of linelisting containing SARS-CoV-2 information (data validation, grouping to cluster, etc).

This package was developped by the Data Science Team of the Covid-19 Taskforce of the Swiss Federal Office of Public Health with initial contributions from the Computational Evolution group of the D-BSSE of the ETH Zürich. It relies on the Tidyverse ecoystem and the tidygraph package.

**Used by**: Swiss Federal Office of Public Health.

**How to access**: This package is not available in a public repository. Send us an [email](mailto:samuel.colin@bag.admin.ch) to request access.


