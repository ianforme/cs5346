People
======

To the general populance, living with COVID has mostly became the new normal. People in Singapore and around the world has mostly complied with all of the restrictions put in place by the government (see the page on government) to minimize the impact of COVID. Yet, most people would still want to gain back some freedoms from pre-COVID, such as being able to travel to other countries without the risk of infection. As such, the following visualizations would answer some potential queries that people would have, and give people some hope for more freedom in the future.

Visualization for people queries
--------------------------------

1.1 Vaccination rate across countries
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This line chart shows the percentage of people that has been fully vaccinated across various countries. Only countries that has a non-zero percentage have been plotted. Full vaccination is defined by whether a person has received all doses prescribed by the vaccination protocol, thus a person receiving the first dose of a 2-dose vaccine would not be counted. The legend is sorted by the percentage of full vaccination as of the latest date (2021-03-19).

From this chart, we can see that Gibraltar and Israel has achieved a full vaccination percentage of more than 50%. A huge majority of the countries are still at below 5%. By zooming into the 0-5% range, we can see that the rate of vaccination of countries in the EU are fairly clustered, which bodes well for free travel within the EU again the in the future.

For Singapore, the full vaccination percentage as of now is about 4.16%. The rate of vaccination seems to be slowly decreasing. 

.. raw:: html

    <hr>

**Visual encoding**

- x-axis represents the date since the first vaccination is available (2 Jan 2021) up to 17 Mar 2021
- y-axis left represents the percentage of population that has been vaccinated
- lines of different colors represent the different countries

**Dataset used**

+--------------------+-------------------------+-----------------------------------------------------+
| Visualisation      | Dataset                 | Table(s)                                            |
+====================+=========================+=====================================================+
| People 1.1         | OWID COVID-19 Data      | Vaccinations                                        |
+--------------------+-------------------------+-----------------------------------------------------+

.. raw:: html

    <hr>

.. raw:: html
    :file: ../plots/line-percentage-vax.html
    
Other visualizations
--------------------

2.1 Total cases across countries
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This animated chart shows the growth of COVID19 throughout the weeks around the world.

We can see that the number of cases started increasing in China in the early stages of the pandemic. Within the month of March 2020,
cases started increasing rapidly throughout the entire world, showing the infectiousness of the virus.

For China, the number of cases did not get any worse after March 2020 (the color remained around the same since then).

Aside from the initial wave of cases in March 2020, there seemed to be another wave of transmission in the winter period from November 2020 to February 2021 for some countries such as Canada, UK and the Scandanavian countries.
This can be seen by the rate of color change of each country increasing in that period.


.. raw:: html

    <hr>


**Visual encoding**

- the intensity of the color of each country shows the number of total cases (in log scale) of that country

**Dataset used**

+--------------------+-------------------------+-----------------------------------------------------+
| Visualisation      | Dataset                 | Table(s)                                            |
+====================+=========================+=====================================================+
| People 2.1         | OWID COVID-19 Data      | OWID COVID-19                                       |
+--------------------+-------------------------+-----------------------------------------------------+    

.. raw:: html

    <hr>
    
.. raw:: html
    :file: ../plots/epidemiology-geo-chart.html

