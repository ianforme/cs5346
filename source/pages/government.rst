Government policy responses
===========================

In this section, we will be giving an overview about the global Covid-19 development situation and various government policies enforced in response to the pandemic outbreak. Effectiveness of these policies in curbing the spread of the virus will be evaluated. However, inevitably, these policies will also severely impact people's mobility. Some graphs are created to visualise the extent of the impact as well.

**Data source is missing, explain visual encoding for each graph**

Covid-19 developments
---------------------

Since 2019, Covid-19 has been rapidly spreading across the global. Although many efforts spent in vaccination innovation, travel restriction, social distancing and healthcare improvement, total number of confirmed cases is still increasing at an exponential rate.

**TODO: Simple bar / line charts to visualise cases in different countries**

.. raw:: html
    :file: ../plots/pandemic-development.html
    
Overall policy effectiveness 
----------------------------

Based on research done by Oxford university, 8 types of policies (shown in the table below) are implemented by various countries to fight against Covid-19. Some of these policies are normally used together by most of the governments. However, due to differences in local situation, these policies are executed in very different ways. Hence researchers come up with a stringency index to represent the collective enforcement level of these policies, the higher the more stringent approaches are adopted. 

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

As shown in the graph, policy effectiveness varies significantly across different countries

* Countries like Japan and Korea adopt a more conservative approach and choose to implement more lenient policies
* France and Singapore are examples of country which adjust their policy stringency level accordingly the local pandemic situation
* China and Italy maintains stringent policies throughout the observation periods
* Some countries like India choose to use less stringent policy despite rising daily confirmed cases, mostly due to economical concerns

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
            
    .. tab-container:: tab4
        :title: UK
        
        .. raw:: html
            :file: ../plots/new-confirmed-vs-policy-GB.html
            
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
			
Time for policies to take effect
--------------------------------

As mentioned, 8 types of policies are mostly used by various governments. How long will these policies take before they slow down or stop the spread of the virus? To study this, we normalised the data from several governments by visualising daily new confirmed cases after 100 days of the policy start dates. By observing the trend, the number of daily new confirmed cases will continue to rise for roughly 20 to 40 days before the number goes down.

Ceveat for this analysis: 

* as many of these policies are used as a bundle, univariate correlation might not be accurately representing the effectness of a single policy
* India, US and Brazil can be removed from this analysis (by clicking on the legend) as they will skew the y-axis readings

.. raw:: html
	:file: ../plots/100-days-after-policy.html


Impact on mobility at transit stations
--------------------------------------

Mobility at transit stations is an important indicator to domestic and internal travel frequency. When transportation industry is booming and many people travel around, this mobility index will rise. For this analysis, we will look at Google mobility index at transit stations. This index represents the percentage change as compare to the observation period. When below 0, it means relative to the observation period, the mobility decreases and vice versa. In our chart, we look at a 3-way interaction between policy stringency, daily new confirmed cases and mobility index for various countries.

Each marker represents a country. Size of the marker represents the stringency index. X-position (log scale) represents daily new confirmed cases while Y-axis represents mobility index at transit stations. As we play the animation, we can find the following:

* When daily number of cases rises, stringency index will rise as well with a much lower mobility index
* During March and April 2020, most of the countries suffered from very low mobility and high policy stringency, except Korea which maintains high mobility consistently 
* During summer time, countries were recovering as policy stringency index decreases and mobility index increases
* However when winter came, second wave stroke most of the countries. Many went back to lock down but not as severe as the summer time. 

.. raw:: html
	:file: ../plots/stringency-vs-mobility-vs-new-cases.html


**TODO: more exploration of transit related plots**