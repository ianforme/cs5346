.. CS5346 Group Project documentation master file, created by
   sphinx-quickstart on Tue Mar 16 22:08:04 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Impact of Covid-19 on Global Transportation
===========================================
:Group: Group 5

:Authors:
    - Luo Wenhan (A0162266E)
    - Sun Weiran (A0130945H)
    - Zhang Chenxi (A0177389H)

:Contribution:
	- Luo Wenhan: People-related queries
	- Sun Weiran: Government-related queries
	- Zhang Chenxi: Business-related queries
	- The other parts, e.g., abstract, introduction etc, are collectively completed together

:Version: 1.0 of 2021/04/18

.. toctree::
   :maxdepth: 1
   :caption: Agenda:
   
   pages/government
   pages/business
   pages/people

Abstract
--------

This project aims to provide insightful visualizations for **governments, business organizations, and the general public to understand various social-economic impacts of Covid-19, with a special focus on the global transportation industry. Besides, it will provide an overview of Covid-19 developments. The effectiveness of government responses is evaluated as well.** This work is mostly based on open datasets gathered and released by Google and Oxford University. Multiple data sources are combined/linked together to develop the storyline.

Introduction
------------

Since the end of 2019, Covid-19 has developed into a global pandemic with no sign of fading away. It seems to become an endless fight between the scientists inventing vaccines and the virus mutating into a more infectious and deadly form. To survive in this challenging era, many governments have to impose various policies to curb the spread. These policies include but not limited to closing public facilities, shutting down borders, and enforcing social distancing. 

Although these policies are effective in tackling the pandemic, they also have significant negative impacts on various industries. Transportation is one of the most severely impacted sectors in the world as domestic and international travels are strongly discouraged in most countries. Singapore Airline Group (SIA) has reported a net loss of S$3.5 billion as passenger numbers fall by 98.9% amid COVID-19. [#]_ Global maritime trade plunged by 4.1% in 2020 due to the unprecedented disruption as estimated by UNCTAD in its Review of Maritime Transport 2020, released on 12 November. [#]_

Through this project, we want to visualize the **impact of Covid-19 on the global transportation industry** which might help various parties for better planning of **personal, organizational, and national future.**

Target audience 
---------------

As mentioned, our analysis aims to provide insights and answers queries for 3 different parties, i.e. government, business organization, and the general public. Each query is answered by at least one visualization in this report. 

+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| Target Audience       | Query                                                                                             | Answered by         |
+=======================+===================================================================================================+=====================+
| Government            | How fast does Covid-19 develop globally? What is the current situation in various countries?      | Government 1.1      |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| Government            | Do stringent policies help to stop the spread of the virus more effectively?                      | Government 1.2      |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| Government            | To what extent will these stringent policies affect people's mobility?                            | Government 1.3      |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| Business organization | To what extent will stringent policy affect transportation business such as export merchandise?   | Business 1.1        |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| Business organization | In terms of transportation, which countries are recovering from from Covid-19?                    | Business 1.2        |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+
| General public        | To what extent is the vaccination rates of different countries?                                   | People 1.1          |
+-----------------------+---------------------------------------------------------------------------------------------------+---------------------+

Other visualisation explorations
--------------------------------

The team has made extra efforts in exploring various kinds of visualizations. These visualizations might not answer any specific queries but they provide additional valuable insights. They can be found in the "Other visualizations" section in the upcoming pages where applicable.

+----------------+-----------------------------------------+
| Visualisation  | Purpose                                 |
+================+=========================================+
| Government 2.1 | Time for policies to take effect        |
+----------------+-----------------------------------------+
| People 2.1     | Total cases across countries (map view) |
+----------------+-----------------------------------------+


Data dictionary
----------------

This work leverages the following datasets:

1. `COVID-19 Open-Data <https://github.com/GoogleCloudPlatform/covid-19-open-data>`_ 
2. `OWID COVID-19 Data <https://ourworldindata.org/coronavirus/>`_ 
3. `Global Economic Monitor <https://datacatalog.worldbank.org/dataset/global-economic-monitor>`_
4. `Container Volume Traffic <https://www.containerstatistics.com/>`_

COVID-19 Open-Data
^^^^^^^^^^^^^^^^^^

This repository attempts to assemble the largest Covid-19 epidemiological database in addition to a powerful set of expansive covariates. It includes open, publicly sourced, licensed data relating to **demographics, economy, epidemiology, geography, health, hospitalizations, mobility, government response, weather, and more.** Moreover, the data merge **daily time-series**, +20,000 global sources, at a fine **spatial resolution**, using a consistent set of region keys. These data come from credible sources including but not limited to Oxford University, Imperial College of London, FinMango, and Google. As per this project, selected tables are used for visualizations. 

.. content-tabs::

    .. tab-container:: tab1
        :title: Index
        
        The index table includes non-temporal data related to countries and regions. It is used in many visualizations to find country-specific pieces of information.
        
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        |        Name       |      Type     |                                                    Description                                                   |           Example           |
        +===================+===============+==================================================================================================================+=============================+
        | key               | string        | Unique string identifying the region                                                                             | US_CA_06001                 |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | place_id          | string        | A textual identifier that uniquely identifies a place in the Google Places database and on Google Maps (details) | ChIJd_Y0eVIvkIARuQyDN0F1LBA |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | wikidata          | string        | Wikidata ID corresponding to this key                                                                            | Q107146                     |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | datacommons       | string        | DataCommons ID corresponding to this key                                                                         | geoId/06001                 |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | country_code      | string        | ISO 3166-1 alphanumeric 2-letter code of the country                                                             | US                          |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | country_name      | string        | American English name of the country, subject to change                                                          | United States of America    |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | subregion1_code   | string        | (Optional) ISO 3166-2 or NUTS 2/3 code of the subregion                                                          | CA                          |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | subregion1_name   | string        | (Optional) American English name of the subregion, subject to change                                             | California                  |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | subregion2_code   | string        | (Optional) FIPS code of the county (or local equivalent)                                                         | 06001                       |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | subregion2_name   | string        | (Optional) American English name of the county (or local equivalent), subject to change                          | Alameda County              |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | 3166-1-alpha-2    | string        | ISO 3166-1 alphanumeric 2-letter code of the country                                                             | US                          |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | 3166-1-alpha-3    | string        | ISO 3166-1 alphanumeric 3-letter code of the country                                                             | USA                         |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | aggregation_level | integer [0-2] | Level at which data is aggregated, i.e. country, state/province or county level                                  | 2                           |
        +-------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+

    .. tab-container:: tab2
        :title: Epidemiology
        
        Epidemiology table includes information related to Covid-19 infection for various regions for every date.
        
        +------------------+---------+--------------------------------------------------------------------+------------+
        |       Name       |   Type  |                             Description                            |   Example  |
        +==================+=========+====================================================================+============+
        | date             | string  | ISO 8601 date (YYYY-MM-DD) of the datapoint                        | 2020-03-30 |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | key              | string  | Unique string identifying the region                               | CN_HB      |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | new_confirmed1   | integer | Count of new cases confirmed after positive test on this date      | 34         |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | new_deceased1    | integer | Count of new deaths from a positive COVID-19 case on this date     | 2          |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | new_recovered1   | integer | Count of new recoveries from a positive COVID-19 case on this date | 13         |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | new_tested2      | integer | Count of new COVID-19 tests performed on this date                 | 13         |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | total_confirmed3 | integer | Cumulative sum of cases confirmed after positive test to date      | 6447       |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | total_deceased3  | integer | Cumulative sum of deaths from a positive COVID-19 case to date     | 133        |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | total_recovered3 | integer | Cumulative sum of recoveries from a positive COVID-19 case to date | 133        |
        +------------------+---------+--------------------------------------------------------------------+------------+
        | total_tested2,3  | integer | Cumulative sum of COVID-19 tests performed to date                 | 133        |
        +------------------+---------+--------------------------------------------------------------------+------------+



    .. tab-container:: tab3
        :title: Mobility
        
        The mobility table measures various metrics related to the movement of the people. It is based on `Google's Mobility Reports <https://www.google.com/covid19/mobility/>`_. This data measures the changes for each day compared to a baseline value for that day of the week. The baseline value is the median during the 5 weeks from 3 Jan to 6 Feb 2020.
        
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        |              Name              |    Type    |                                                                              Description                                                                             |   Example  |
        +================================+============+======================================================================================================================================================================+============+
        | date                           | string     | ISO 8601 date (YYYY-MM-DD) of the datapoint                                                                                                                          | 2020-03-30 |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | key                            | string     | Unique string identifying the region                                                                                                                                 | US_CA      |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_grocery_and_pharmacy  | double [%] | Percentage change in visits to places like grocery markets, food warehouses, farmers markets, specialty food shops, drug stores, and pharmacies compared to baseline | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_parks                 | double [%] | Percentage change in visits to places like local parks, national parks, public beaches, marinas, dog parks, plazas, and public gardens compared to baseline          | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_transit_stations      | double [%] | Percentage change in visits to places like public transport hubs such as subway, bus, and train stations compared to baseline                                        | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_retail_and_recreation | double [%] | Percentage change in visits to restaurants, cafes, shopping centers, theme parks, museums, libraries, and movie theaters compared to baseline                        | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_residential           | double [%] | Percentage change in visits to places of residence compared to baseline                                                                                              | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+
        | mobility_workplaces            | double [%] | Percentage change in visits to places of work compared to baseline                                                                                                   | -15        |
        +--------------------------------+------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------+     

    .. tab-container:: tab4
        :title: Oxford government policy responses
        
        The government responses table provides a summary of the government's responses to the events. It also includes a *stringency index*, provided by the Oxford University which measures the overall stringent level of the policies for the country.
        
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        |                Name                |      Type      |                        Description                       |   Example   |
        +====================================+================+==========================================================+=============+
        | date                               | string         | ISO 8601 date (YYYY-MM-DD) of the datapoint              | 2020-03-30  |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | key                                | string         | Unique string identifying the region                     | US_CA       |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | school_closing                     | integer [0-3]  | Schools are closed                                       | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | workplace_closing                  | integer [0-3]  | Workplaces are closed                                    | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | cancel_public_events               | integer [0-3]  | Public events have been cancelled                        | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | restrictions_on_gatherings         | integer [0-3]  | Gatherings of non-household members are restricted       | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | public_transport_closing           | integer [0-3]  | Public transport is not operational                      | 0           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | stay_at_home_requirements          | integer [0-3]  | Self-quarantine at home is mandated for everyone         | 0           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | restrictions_on_internal_movement  | integer [0-3]  | Travel within country is restricted                      | 1           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | international_travel_controls      | integer [0-3]  | International travel is restricted                       | 3           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | income_support                     | integer [USD]  | Value of fiscal stimuli, including spending or tax cuts  | 20449287023 |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | debt_relief                        | integer [0-3]  | Debt/contract relief for households                      | 0           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | fiscal_measures                    | integer [USD]  | Value of fiscal stimuli, including spending or tax cuts  | 20449287023 |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | international_support              | integer [USD]  | Giving international support to other countries          | 274000000   |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | public_information_campaigns       | integer [0-2]  | Government has launched public information campaigns     | 1           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | testing_policy                     | integer [0-3]  | Country-wide COVID-19 testing policy                     | 1           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | contact_tracing                    | integer [0-2]  | Country-wide contact tracing policy                      | 1           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | emergency_investment_in_healthcare | integer [USD]  | Emergency funding allocated to healthcare                | 500000      |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | investment_in_vaccines             | integer [USD]  | Emergency funding allocated to vaccine research          | 100000      |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | facial_coverings                   | integer [0-4]  | Policies on the use of facial coverings outside the home | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | vaccination_policy                 | integer [0-5]  | Policies for vaccine delivery for different groups       | 2           |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+
        | stringency_index                   | double [0-100] | Overall stringency index                                 | 71.43       |
        +------------------------------------+----------------+----------------------------------------------------------+-------------+

OWID COVID-19 Data
^^^^^^^^^^^^^^^^^^

This is another collection of COVID-19 Data provided by Our World in Data (OWID). While not as comprehensive as COVID-19 Open Data, the datasets are much cleaner compared to COVID-19 Open Data. Only selected tables are used for visualizations.
        
The index table includes non-temporal data related to countries and regions. It is used in many visualizations to find country-specific pieces of information.

.. csv-table::
    :header: "Name", "Type", "Description", "Example"
    :widths: 30, 15, 40, 5
    
    "location", "string", "Name of the country (or region within a country).", "Albania"
    "iso_code", "string", "ISO 3166-1 alpha-3 – three-letter country codes.", "ALB"
    "date", "string", "Date of the observation.", "13/1/2021"
    "total_vaccinations", "integer", "Total number of doses administered. This is counted as a single dose, and may not equal the total number of people vaccinated, depending on the specific dose regime (e.g. people receive multiple doses). If a person receives one dose of the vaccine, this metric goes up by 1. If they receive a second dose, it goes up by 1 again.", 188
    "total_vaccinations_per_hundred", "double [%]", "total_vaccinations per 100 people in the total population of the country.", 0.01
    "daily_vaccinations_raw", "integer", "Daily change in the total number of doses administered. It is only calculated for consecutive days. This is a raw measure provided for data checks and transparency, but we strongly recommend that any analysis on daily vaccination rates be conducted using daily_vaccinations instead.", 60
    "daily_vaccinations", "integer", "New doses administered per day (7-day smoothed). For countries that don't report data on a daily basis, we assume that doses changed equally on a daily basis over any periods in which no data was reported. This produces a complete series of daily figures, which is then averaged over a rolling 7-day window.", 63
    "daily_vaccinations_per_million", "integer", "daily_vaccinations per 1,000,000 people in the total population of the country.", 22
    "people_vaccinated", "integer", "Total number of people who received at least one vaccine dose. If a person receives the first dose of a 2-dose vaccine, this metric goes up by 1. If they receive the second dose, the metric stays the same.", 128
    "people_vaccinated_per_hundred", "double [%]", "people_vaccinated per 100 people in the total population of the country.", 0.01
    "people_fully_vaccinated", "integer", "Total number of people who received all doses prescribed by the vaccination protocol. If a person receives the first dose of a 2-dose vaccine, this metric stays the same. If they receive the second dose, the metric goes up by 1.", 0
    "people_fully_vaccinated_per_hundred", "double [%]", "people_fully_vaccinated per 100 people in the total population of the country.", 0.0


Global Economic Monitor
^^^^^^^^^^^^^^^^^^^^^^^
This dataset provides daily updates of global economic developments, with coverage of high income- as well as developing countries. Daily data updates are provided for exchange rates, equity markets, and emerging market bond indices. Monthly data coverage (updated daily and populated upon availability) is provided for consumer prices, high-tech market indicators, industrial production and **merchandise trade**. The following two tables are used in this project.


.. content-tabs::

    .. tab-container:: tab1
        :title: Exports Merchandise, Customs, current US$, millions, seas. adj.
        
        Merchandise (goods) exports, cost, insurance and freight basis (c.i.f.), in current US$ millions, seasonally adjusted.
        
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        |        Name                     |      Type     |                                                    Description                                                   |           Example           |
        +=================================+===============+==================================================================================================================+=============================+
        | country/region                  | string        | Unique string identifying the country or region                                                                  | Singapore                   |
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | Export merchandise              | double [USD]  | Export merchandise measured in millions of US dollars                                                            | 27375.69                    |
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+

    .. tab-container:: tab2
        :title: Imports Merchandise, Customs, current US$, millions, seas. adj.
        
        Merchandise (goods) imports, cost, insurance and freight basis (c.i.f.), in current US$ millions, seasonally adjusted.
        
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        |        Name                     |      Type     |                                                    Description                                                   |           Example           |
        +=================================+===============+==================================================================================================================+=============================+
        | country/region                  | string        | Unique string identifying the country or region                                                                  | Singapore                   |
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
        | Import merchandise              | double [USD]  | Import merchandise measured in millions of US dollars                                                            | 25865.38                    |
        +---------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+

Container Volume
^^^^^^^^^^^^^^^^
This dataset provides container volume traffic for regions and Brazil. This project uses the Brazil import/export volumes table.

Export/import container volume in Brazil.

+-----------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
|        Name                       |      Type     |                                                    Description                                                   |           Example           |
+===================================+===============+==================================================================================================================+=============================+
| date                              | string        | Date (YYYY/m/DD) of the datapoint                                                                                | 2020/6/30                   |
+-----------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
| Export Container Volume           | integer       | Export container volume index measured in TEUs                                                                   | 212049                      |
+-----------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+
| Import Container Volume           | integer       | Import container volume index measured in TEUs                                                                   | 202857                      |
+-----------------------------------+---------------+------------------------------------------------------------------------------------------------------------------+-----------------------------+

Data processing & visualization steps
-------------------------------------

Overview
^^^^^^^^

Visualisations in this work are mostly created by `Plotly <https://plotly.com/python/>`_, a popular and powerful graphing library in Python. The original datasets are downloaded and pre-processed in Python, with `Pandas <https://pandas.pydata.org/>`_ and `Numpy <https://numpy.org/>`_. The detailed steps of pre-processing are based on the specifications of visualizations, which are customized and elaborated in the next section - *Step-wise process*. Charts are exported in html formats and loaded in this `Sphinx <https://www.sphinx-doc.org/en/master/#>`_ document for reporting and presentation.

Step-wise process
^^^^^^^^^^^^^^^^^

**Government 1.2 - Overall policy effectiveness**

1. download index table from COVID-19 Open Data and load it in memory
2. fileter dates, keep index table records from 2020-01-01 to 2021-02-01
3. filter countries, keep index table records from traget countries, i.e., China, US, UK, France, Singapore, India, Brazil, Korea, Japan, Italy and Malaysia. Find country codes in of these target countries. These country codes are used for the following steps.
4. download epidemiology table from COVID-19 Open Data and load it in memory
5. filter dates, keep epidemiology table records from 2020-01-01 to 2021-02-01
6. filter countries, keep epidemiology table records from traget countries
7. impute missing values in epidemiology table with 0. In some countries, Covid test was not conducted in the beginning hence daily confimed cases were missing. It is reasonable to impute them as 0.
8. download policy response table from COVID-19 Open Data and load it in memory
9. filter dates and countries in the same way as the other tables.
10. for each country from the target country lists:
	- filter and keep records from the country in both epidemiology and policy response tables
	- create epidemiology line trace with x as the dates and y as the daily new confirmed cases
	- create stringency index line trace with x as the date and y as the stringency index
	- make a dual-axis plot, with primary y as the daily new confirmed cases and secondary y as the stringency index
	- export chart for that country

**Business 1.1 - Policy impact on import/export merchandise**

1. download import/export merchandise table from Global Economic Monitor and load it in memory
2. fileter dates, keep merchandise records from 2020-01-01 to 2021-02-01
3. filter countries, keep merchandise records from the traget country, Brazil
4. download index table from COVID-19 Open Data and load it in memory
5. filter dates, keep index table records from 2020-01-01 to 2021-02-01
6. filter countries, keep index table records from the traget country, Brazil
7. create stringency index line trace with x as the date and y as the stringency index
8. create import/export merchandise line trace with x as the date and y as the value of merchandise
9. make a dual-axis plot, with primary y as the value of merchandise and secondary y as the stringency index
10. export chart

**People 1.1 - Vaccination rate across countries**

1. download vaccinations rate csv from OWID and load into memory
2. filter ISO code that contains "OWID" (Such codes are for subregions or category of regions used by OWID)
3. select the following columns: "location", "date", "people_fully_vaccinated_per_hundred"
4. perform a groupby on "location", for each group:
    1. append a row with date "2021-01-02" (1 day before earliest vaccination date of all countries) and "people_fully_vaccinated_per_hundred" at 0
    2. append a row with date "2021-03-17" (latest date with data), "people_fully_vaccinated_per_hundred" is left blank
    3. convert date to datetime and set it as a datetimeindex (to facilitate datetime operations)
    4. sort the group on the index
    5. filter out any data with date before "2020-01-02" (to remove rows with an early date but "people_fully_vaccinated_per_hundred" is 0 or blank)
    6. interpolate "people_fully_vaccinated_per_hundred" in both direction using the "time" method which takes in account of the varying resolution of the data
5. perform another groupby on "location", and filter out groups where "people_fully_vaccinated_per_hundred" is 0 as of the latest date
6. make a line chart with x-axis as "date", y-axis as "people_fully_vaccinated_per_hundred", color as "location"
7. limit the x-axis of the line chart to between 2021-01-02 and 2021-03-17, the y-axis to between 0 and 100
8. set the order of the locations in the legend to the max "people_fully_vaccinated_per_hundred" of each location in descending order
9. export the chart

References
----------

.. [#] `SIA Group reports first half net loss of S$3.5 billion as passenger numbers fall by 98.9% amid COVID-19 <https://www.channelnewsasia.com/news/singapore/covid-19-sia-group-first-half-net-loss-of-3-5-billion-13480628>`_
.. [#] `COVID-19 cuts global maritime trade, transforms industry
 <https://unctad.org/news/covid-19-cuts-global-maritime-trade-transforms-industry#:~:text=Global%20maritime%20trade%20will%20plunge,might%20cause%20a%20steeper%20decline.>`_
