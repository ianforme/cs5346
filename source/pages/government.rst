Government policy responses
===========================

In this section, we will be giving an overview of the global Covid-19 development situation and various government policies enforced in response to the pandemic outbreak. The effectiveness of these policies in curbing the spread of the virus will be evaluated. However, inevitably, these policies will also severely impact people's mobility. Visualization is created to visualize the extent of the impact as well.

Visualization for government queries
------------------------------------

1.1 Covid-19 developments
^^^^^^^^^^^^^^^^^^^^^^^^^

Since 2019, Covid-19 has been rapidly spreading across the globe. Although many efforts are spent on vaccination innovation, travel restriction, social distancing, and healthcare improvement, the total number of confirmed cases is still **increasing at an exponential rate.**

As of Feb 2021, the top 3 countries with the most confirmed cases are **United States of America, India, and Brazil**. 65% of the total confirmed cases global are from the top 10 countries.

.. content-tabs:: 

    .. tab-container:: left1
        :title: Global
        
        .. raw:: html
        
            <hr>
        
        **Visual encoding**
        
        - x-axis represents the time at date interval
        - y-axis represents the number of people
        - blue line represents the number of existing confirmed cases
        - red line represents the number of recovered confirmed cases
        - green line represents the number of deceased cases
        
        **Dataset used**
        
        +--------------------+--------------------+-----------------------------------------------------+
        | Visualisation      | Dataset            | Table(s)                                            |
        +====================+====================+=====================================================+
        | Government 1.1     | COVID-19 Open-Data | Index, Epidemiology                                 |
        +--------------------+--------------------+-----------------------------------------------------+
        
        .. raw:: html
        
            <hr>
        
        .. raw:: html
            :file: ../plots/pandemic-development.html

    .. tab-container:: left2
        :title: By Country
        
        .. raw:: html
        
            <hr>
        
        **Visual encoding**
        
        - x-axis represents total confirmed cases
        - y-axis represents countries
        
        **Dataset used**
        
        +--------------------+--------------------+-----------------------------------------------------+
        | Visualisation      | Dataset            | Table(s)                                            |
        +====================+====================+=====================================================+
        | Government 1.1     | COVID-19 Open-Data | Index, Epidemiology                                 |
        +--------------------+--------------------+-----------------------------------------------------+
        
        .. raw:: html
        
            <hr>
        
        .. raw:: html
            :file: ../plots/case_per_countries.html



    
1.2 Overall policy effectiveness 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Based on research done by Oxford University, 8 types of policies (shown in the table below) are implemented by various countries to fight against Covid-19. Some of these policies are frequently used together by most governments. However, **due to differences in the local situation, these policies are executed in very different ways**. Hence researchers come up with an astringency index to represent the collective enforcement level of these policies, the higher the more stringent approaches are adopted. 

+--------------------------------------+
| Policies                             |
+======================================+
| School closing                       |
+--------------------------------------+
| Workplace closing                    |
+--------------------------------------+
| Cancel public events                 |
+--------------------------------------+
| Restrictions on gathering            |
+--------------------------------------+
| Public transport closing             |
+--------------------------------------+
| Stay-at-home requirements            |
+--------------------------------------+
| Restrictions on internal movement    |
+--------------------------------------+
| Restrictions on international travel |
+--------------------------------------+

As shown in the graph, policy implementation varies significantly across different countries

* Countries like Japan and Korea adopt a more conservative approach and choose to implement more lenient policies
* France and Singapore are examples of countries that adjust their policy stringency level according to the local pandemic situation
* China and Italy maintain stringent policies throughout the observation periods
* Some countries like India choose to use less stringent policy despite rising daily confirmed cases, mostly due to economical concerns

.. raw:: html

    <hr>

**Visual encoding**

- x-axis represents the time at date interval
- y-axis at left represents daily new confirmed cases
- y-axis at right represents policy stringency level
- red line represents the stringency index, referring to the right y-axis
- blue line represents the daily new confirmed cases, referring to the left y-axis

**Dataset used**

+--------------------+--------------------+-----------------------------------------------------+
| Visualisation      | Dataset            | Table(s)                                            |
+====================+====================+=====================================================+
| Government 1.2     | COVID-19 Open-Data | Index, Epidemiology, Government responses           |
+--------------------+--------------------+-----------------------------------------------------+

.. raw:: html

    <hr>

\* *the following tabs are sorted by alphabetic order*

.. content-tabs::

    .. tab-container:: tab1
        :title: Brazil
    
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-BR.html

    .. tab-container:: tab2
        :title: China

        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-CN.html
            
    .. tab-container:: tab3
        :title: France
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-FR.html
            
    .. tab-container:: tab5
        :title: India
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-IN.html
            
    .. tab-container:: tab6
        :title: Italy
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-IT.html
            
    .. tab-container:: tab7
        :title: Japan
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-JP.html
            
    .. tab-container:: tab8
        :title: Korea
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-KR.html
            
    .. tab-container:: tab9
        :title: Malaysia
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-MY.html
            
    .. tab-container:: tab10
        :title: Singapore
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-SG.html
            
    .. tab-container:: tab11
        :title: USA
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-US.html
            
    .. tab-container:: tab4
        :title: UK
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-GB.html

1.3 Impact on mobility at transit stations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Mobility at transit stations is an important indicator of domestic and internal travel frequency.** When the transportation industry is booming and many people travel around, this mobility index will rise. For this analysis, we will look at the Google mobility index at transit stations. This index represents the percentage change as compared to the observation period. When below 0, it means relative to the observation period, the mobility decreases and vice versa. In our chart, we look at a **3-way interaction between policy stringency, daily new confirmed cases, and mobility index for various countries.** As we play the animation, we can find the following:

* When the daily number of cases rises, the stringency index will rise as well with a much lower mobility index
* During March and April 2020, most of the countries suffered from very low mobility and high policy stringency, except Korea which maintains high mobility consistently 
* During summer time, countries were recovering as policy stringency index decreases and mobility index increases
* However when winter came, second wave stroke most of the countries. Many went back to lockdown but not as severe as the summer time. 

.. raw:: html

    <hr>

**Visual encoding**

- x-axis represents daily new confirmed cases at log scale
- y-axis represents the mobility index at transit stations
- each marker represents a country
- size of the marker represents the policy stringency index, the larger the more stringent
- x and y locations of the marker represent daily new confirmed cases and mobility index respectively

**Dataset used**

+--------------------+--------------------+-----------------------------------------------------+
| Visualisation      | Dataset            | Table(s)                                            |
+====================+====================+=====================================================+
| Government 1.3     | COVID-19 Open-Data | Index, Epidemiology, Government responses, Mobility |
+--------------------+--------------------+-----------------------------------------------------+

.. raw:: html

    <hr>

.. raw:: html
    :file: ../plots/stringency-vs-mobility-vs-new-cases.html


Other visualizations
--------------------

2.1 Time for policies to take effect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As mentioned, 8 types of policies are mostly used by various governments. How long will these policies take before they slow down or stop the spread of the virus? To study this, we normalized the data from several governments by visualizing daily new confirmed cases after 100 days of the policy start dates. By observing the trend, the number of daily new confirmed cases will continue to rise for roughly 20 to 40 days before the number goes down.

Caveat for this analysis: 

* as many of these policies are used as a bundle, univariate correlation might not be accurately representing the effectiveness of a single policy
* India, the US, and Brazil can be removed from this analysis (by clicking on the legend) as they will skew the y-axis readings

.. raw:: html

    <hr>

**Visual encoding**

- x-axis represents the number of days since policy start dates
- y-axis represents daily new confirmed cases
- each line represents a country

**Dataset used**

+--------------------+--------------------+-----------------------------------------------------+
| Visualisation      | Dataset            | Table(s)                                            |
+====================+====================+=====================================================+
| Government 2.1     | COVID-19 Open-Data | Index, Epidemiology, Government responses           |
+--------------------+--------------------+-----------------------------------------------------+

.. raw:: html

    <hr>

.. raw:: html
    :file: ../plots/100-days-after-policy.html