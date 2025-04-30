# **Candid Core Fields Refence Guide**

*Examples in italics describe a fictional dataset:*

***Global Urban Heat Island Intensity (GUHII) \- 2000-2020***

*Globally consistent estimate of the surface urban heat island (SUHI) intensity for all major urban areas worldwide, covering the period from 2000 to 2020\. It's a derived product, calculated primarily from satellite-based Land Surface Temperature (LST) data and land cover classifications (to identify urban vs. surrounding rural areas).*

## Suitability & Limitations

* **Suitability Summary**: Concise, curated summary highlighting the dataset's primary strengths and weaknesses, specifically concerning its suitability for common applications.

  *Strong for global/regional trend analysis and city ranking of surface UHI. Less suitable for microscale urban planning or direct air temperature correlation without calibration. Known issues with cloud contamination in persistently overcast areas require user caution.*

* **Application Limitations**: Known constraints, caveats, or inappropriate applications ("contraindications") for the dataset, highlighting scenarios where its use might lead to inaccurate results, misinterpretations, or where specific precautions are necessary.

  *Not suitable for intra-urban microclimate analysis below 1km resolution; accuracy reduced in persistently cloudy regions; comparison between cities requires careful consideration of varying rural reference definitions.*

* **Data Quality Metrics / Uncertainty**:  Quantitative measures of the dataset's quality, accuracy, or uncertainty, such as error statistics, validation scores, confidence intervals, or spatial/temporal maps of uncertainty.

  *Accuracy assessment against 100 global weather stations shows mean bias of \+0.5°C (urban warmer) and RMSE of 1.2°C; uncertainty tends to be higher in tropical regions due to cloud cover correction residuals.*

* **Known Gaps / Future Work**: Recognized gaps in the dataset's coverage, methodology, or validation, and may outline planned improvements or areas identified for future research by the creators or community.

  *Current version lacks specific validation in Arctic cities and does not differentiate between daytime/nighttime UHI. Future work aims to incorporate VIIRS data for improved resolution and explore seasonal variations.*

## Context & Definitions

* **Key Term Definitions**: Critical terms used within the dataset (e.g., "forest," "urban") and the specific classification scheme or ontology applied.

  *"Urban" defined by pixels with \>50% impervious surface based on ESA WorldCover 2020\. "Rural Reference" defined as non-urban pixels within a 5km buffer excluding water bodies. "Intensity" is the mean annual surface temperature difference (°C) between these zones.*

* **Methodology Summary**: Summary of the specific algorithms, input data sources, processing steps, and assumptions used to generate the dataset.

  *Generated using MODIS MOD11A2 LST v6, ESA WorldCover 2020 for urban extent, and a 5km buffer non-urban reference zone selection algorithm. Cloud gaps filled using temporal interpolation. Full details in linked publication \[DOI\].*

* **Ethics / Bias**: Potential ethical implications, known biases (algorithmic, sensor, sampling), fairness assessments, or privacy concerns related to the dataset's creation or potential application, acknowledging limitations beyond technical ones.

  *Primarily based on satellite thermal data, does not directly measure human heat exposure or account for indoor conditions. Urban extent definition may underrepresent informal settlements in some regions. Derived from publicly available remote sensing, no direct human subject data used.*

* **Vibes / Social Context**: The informal context, cultural significance, unique "personality," community ethos, or relevant historical background associated with the dataset. Elements often part of the creation process but not formal attributes.

  *Release versions are named after jazz musicians; project blog has unexpectedly good art.*

## Use Cases & Target Users

* **Target Audience**: Primary intended users or groups.

  *Urban climate researchers, city planners, public health officials, climate adaptation consultants.*

* **Recommended Expertise**  
  The level/type of technical skill or domain knowledge recommended for effectively using the dataset.  
  *Requires basic GIS/remote sensing data handling skills (QGIS, ArcGIS, Python, R) and understanding of urban climate concepts.*  
* **Suggested Uses**: Recommended applications for the dataset, guiding users on how the data creators or maintainers envision it being employed effectively.

  *Assessing heat exposure risk for vulnerable populations; comparing urban planning mitigation strategy effectiveness across cities; regional climate modeling input.*

* **Key Instructions**: Critical instructions for using the dataset effectively, potentially formatted for machine interpretation.

  *Ensure NoData value (-9999) is correctly handled; pixel values represent surface temperature difference in degrees Celsius; cite original publication and dataset DOI when using*

* **Example Uses \- Teaching Resources**: Specific educational materials, tutorials, textbooks, or curricula using this dataset for teaching.

  *Used in GEOG 450 Urban Climatology Lab module at University X; tutorial notebook for analyzing trends available on project GitHub.*

* **Example Uses \- Community Resources**: Resources developed by the user community (forums, code repositories, wikis, user groups) offering support and knowledge sharing.

  *Google Group 'GUHII-Users' for questions and discussion; community-contributed analysis scripts repo on GitHub.*

* **Example Uses \- Apps**: Specific applications, particularly interactive web apps, dashboards, or software tools built using this dataset.

  *Interactive map viewer showing UHI intensity trends and city rankings available at \[link-to-app\].*

* **Example Uses \- Functions / API**: Specific functions, APIs, software libraries, or computational models utilizing this dataset, often for generating derived products.

  *Python package 'guhii\_tools' available on PyPI for extracting time series, calculating regional averages, and basic plotting.*

* **Example Uses \- Art**: Instances where the dataset served as a basis for artistic creation or data visualization beyond purely scientific purposes.

  *Visualization of global UHI patterns featured in the 'Data Warming' digital art exhibition (2023).*

* **Example Uses \- Games (Interactive Art)**: Examples where the dataset was incorporated into games or interactive art installations using the data directly for gameplay or exploration.

  *Data informs background heat hazard levels in the educational simulation 'Climate City Planner'.*

## Provenance & Relationships

* **Review Method**: The process and nature of any quality assessment or review the dataset has undergone, clarifying the type of scrutiny applied (e.g., internal, peer review, independent validation).

  *Internal consistency checks by data producers; methodology peer-reviewed as part of publication; validation against limited ground station data in 20 cities.*

* **Candid Core Curation Method**: How the Candid Core metadata fields themselves were populated.

  *Candid Core fields initially populated by the GeoClimate Lab data producers, reviewed and refined based on feedback from the GUHII-Users Google Group and two independent expert reviewers. Some contraindications are added by the community and are disputed by the dataset authors.*

* **Derived Datasets**: Other datasets created directly using this dataset as a primary source or input.

  *Global Urban Heatwave Exposure Index (GUHEI) by Smith et al. (2024), which combines GUHII with population density.*

* **Linked Datasets**: Datasets frequently used alongside the current dataset or considered complementary for context, calibration, validation, or common workflows.

  *Often used with WorldPop population density grids; ESA WorldCover for urban morphology context; ERA5 climate reanalysis data.*

* **Related Datasets**: Datasets sharing a thematic, spatial, or temporal connection, suggesting key datasets for comparison or broader context.

  *MODIS Land Surface Temperature product (MOD11); Local Climate Zones (LCZ) maps from WUDAPT; specific regional UHI studies.*

* **Competitor Datasets**: Alternative datasets covering a similar scope, allowing users to identify and evaluate other potential data sources for their specific needs.

  *Global Surface UHI Explorer (GSUE) by Li et al.; UHI dataset by Chakraborty & Lee.*

* **Comparison Notes**: Notes comparing this dataset to key alternatives, highlighting differences in methodology, scope, resolution, known discrepancies, or complementary aspects relevant to specific use cases.

  *Compared to GSUE, GUHII uses a consistent rural reference definition globally but has coarser resolution. Unlike MOD11 LST, GUHII provides intensity directly, simplifying cross-city comparison but masking raw temperature values.*

## Lifecycle & Access

* **Support Status**: Current maintenance level and expected longevity of the dataset, indicating its reliability for long-term projects (e.g., actively maintained, limited funding, deprecated).

  *Actively maintained by the GeoClimate Lab; current funding secured until Dec 2025; updates planned annually.*

* **Curation/Update Philosophy**: The approach to maintaining and updating the dataset, including frequency, criteria for new versions, handling of user feedback, and philosophy regarding incorporating new methods or input data.

  *Updated annually incorporating the latest full year of LST data. Major methodological revisions trigger a new major version (e.g., v2.0). User-reported errors are reviewed quarterly and may trigger patch releases (e.g., v1.1.1).*

* **Changelog**: Record of significant modifications made to the dataset over time, including updates, corrections, version changes, and deprecation notices, allowing users to track its evolution.

  *v1.1 (2023-03-15): Corrected processing artifact affecting coastal South American cities; improved cloud masking. v1.0 (2022-01-10): Initial release based on published methodology.*

* **Breaking Changes**: Modifications within the dataset's history (also expected to be in the `Changelog`) known to be incompatible with previous versions, potentially breaking existing user workflows or code.

  *v1.1 changed raster value scaling from integer tenths of degrees C to floating point degrees C, requiring user code updates for direct value interpretation.*

* **Data access & Providers**: Available access points or providers for the dataset and characterizes the ease of access, including details on authentication, rate limits, download mechanisms, or formats.

  *Downloadable as GeoTIFFs via Zenodo (DOI provided, free account required); Google Earth Engine Asset ID available for cloud computation; no current API access.*

* **User Feedback Channel**: Designated channel or contact point for users to report errors, ask questions, suggest improvements, or share use cases related to the dataset.

  *Please report issues via the GitHub repository issue tracker \[link\] or contact the GeoClimate Lab at \[email address\]. User forum available at \[link\].*

* **Carbon/Energy Cost**: Estimated environmental footprint, specifically the energy consumption or carbon emissions, associated with the production, processing, and storage of the dataset.

  *Estimated 50,000 CPU hours for processing on university HPC cluster (\~5 tonnes CO2e); primarily derived from existing satellite LST products.*
