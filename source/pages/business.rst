Business
========

In this part, we will first take Brazil as an example to answer the query how the transportation industry is impacted by public policies. Then we will use the import/export data to see which countries are recovering from Covid-19.

Visualization for business queries
----------------------------------

1.1 Impact on Brazil import/export merchandise measured in dollars and container volume from government policy 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

From the graphs we can learn that:

* Brazil's import merchandise is impacted by public policies especially international travel policy. However, its export merchandise is not impacted by the its public policy.
* Import merchandise drops greatly measured in container voulume, which indicates that the transportation industry is impacted by the public policy.
* Import merchandise drops more smoothly measured in dollars compared to its container volume, which indicates that the import merchandise drop down are from the merchandise with less value but requires more capacity.

.. content-tabs::
    
    .. tab-container:: tab1
        :title: import/export merchandise measured in dollars
        
        .. raw:: html
        
            <hr>
        
        **Visual encoding**

        - x-axis represents the time at date interval
        - y-axis at left represents value of merchandise in USD
        - y-axis at right represents policy stringency level
        - blue line represents the value of export merchandise, referring to the left y-axis
        - red line represents the value of import merchandise, referring to the left y-axis
        - green line represents the international travel stringency index, referring to the right y-axis
        - purple line represents the overall stringency index, referring to the right y-axis

        **Dataset used**

        +--------------------+-------------------------+-----------------------------------------------------+
        | Visualisation      | Dataset                 | Table(s)                                            |
        +====================+=========================+=====================================================+
        | Business 1.1       | COVID-19 Open-Data      | Index                                               |
        +                    +-------------------------+-----------------------------------------------------+
        |                    | Global Economic Monitor | Import merchandise, Export merchandise              |
        +--------------------+-------------------------+-----------------------------------------------------+
        
        .. raw:: html
        
            <hr>
            
        .. raw:: html
            :file: ../plots/brazil-dollar.html

    .. tab-container:: tab2
        :title: import/export merchandise measured in container volume
        
        .. raw:: html
        
            <hr>
        
        **Visual encoding**

        - x-axis represents the time at date interval
        - y-axis at left represents value of merchandise in container volume (TEU)
        - y-axis at right represents policy stringency level
        - blue line represents the value of export merchandise, referring to the left y-axis
        - red line represents the value of import merchandise, referring to the left y-axis
        - green line represents the international travel stringency index, referring to the right y-axis
        - purple line represents the overall stringency index, referring to the right y-axis

        **Dataset used**

        +--------------------+--------------------------+-----------------------------------------------------+
        | Visualisation      | Dataset                  | Table(s)                                            |
        +====================+==========================+=====================================================+
        | Business 1.1       | COVID-19 Open-Data       | Index                                               |
        +                    +--------------------------+-----------------------------------------------------+
        |                    | Container Volume Traffic | Export/import container volume in Brazil.           |
        +--------------------+--------------------------+-----------------------------------------------------+
        
        .. raw:: html
        
            <hr>
            
        .. raw:: html
            :file: ../plots/brazil-container.html

1.2 Import/export merchandise measured in dollars for selected countries
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

From the graphs we can learn that:

* China has its lowest point for export merchandise in Feburary, 2020, while the other countries's are in May, 2020. There is large fluctuations in Brazil's export merchandise.
* For import merchandise, all the selected countries have similar trend.

.. content-tabs::
    
    .. tab-container:: tab1
        :title: import merchandise measured in dollars

        .. raw:: html

            <hr>

        **Visual encoding**

        - x-axis represents the time at date interval
        - y-axis at left represents value of merchandise in USD
        - countries are represented in lines with different colors as specified in the color legend

        **Dataset used**

        +--------------------+-------------------------+-----------------------------------------------------+
        | Visualisation      | Dataset                 | Table(s)                                            |
        +====================+=========================+=====================================================+
        | Business 1.2       | COVID-19 Open-Data      | Index                                               |
        +                    +-------------------------+-----------------------------------------------------+
        |                    | Global Economic Monitor | Import merchandise, Export merchandise              |
        +--------------------+-------------------------+-----------------------------------------------------+

        .. raw:: html

            <hr>

        .. raw:: html
            :file: ../plots/import-countries-dollar.html

    .. tab-container:: tab2
        :title: export merchandise measured in dollars

        .. raw:: html

            <hr>

        **Visual encoding**

        - x-axis represents the time at date interval
        - y-axis at left represents value of merchandise in USD
        - countries are represented in lines with different colors as specified in the color legend

        **Dataset used**

        +--------------------+-------------------------+-----------------------------------------------------+
        | Visualisation      | Dataset                 | Table(s)                                            |
        +====================+=========================+=====================================================+
        | Business 1.2       | COVID-19 Open-Data      | Index                                               |
        +                    +-------------------------+-----------------------------------------------------+
        |                    | Global Economic Monitor | Import merchandise, Export merchandise              |
        +--------------------+-------------------------+-----------------------------------------------------+

        .. raw:: html

            <hr>


        .. raw:: html
            :file: ../plots/export-countries-dollar.html



