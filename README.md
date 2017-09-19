# Contributing

This tool was developed at the National Geospatial-Intelligence Agency (NGA) in collaboration with ESRI. The government has "unlimited rights" and is releasing this software to increase the impact of government investments by providing developers with the opportunity to take things in new directions. The software use, modification, and distribution rights are stipulated within the MIT license.

All pull request contributions to this project will be released under the MIT or compatible license. Software source code previously released under an open source license and then modified by NGA staff is considered a "joint work" (see 17 USC § 101); it is partially copyrighted, partially public domain, and as a whole is protected by the copyrights of the non-government authors and must be released according to the terms of the original open source license.

# state-of-the-data

The State of the Data tools are a set of python based geoprocessing tools that evaluate the quality of topographic feature data in terms of its completeness, 
logical consistency, positional accuracy, source lineage, temporal accuracy, and thematic accuracy.

# Purpose
The National Geospatial-Intelligence Agency (NGA) desires to maintain a full understanding of the adequacy of current data and product holdings. Areas where data and products meet or exceed requirements are distinguished from those where mission-relevant shortfalls exist. Analytic methodologies will be used to delineate those areas where mission-relevant data enrichment and production is required, whether due to pre-existing deficiencies, recent changes in world events, or changes in mission needs or priorities.

# Background
- Provide online, on-demand access to GEOINT
  - Deliver data, products and services through customer Self-Service
- Operations in the Data-Rich Environment
  - Content Producers → Content Managers
  - Provide insight into data quality, mission / portrayal suitability, and fit-for-purpose
- Content Suitability Indicators
  - Systematic approach using statistics and science to objectively evaluate data on a global scale
  - Facilitates transparency of GEOINT through discoverability, accessibility and usability

# The Toolbox and Scripts
## State of the Data Toolbox
This toolbox contains all current State of the Data analysis scripts as ArcGIS geoprocessing tools.
![](http://nga.maps.arcgis.com/sharing/rest/content/items/b01f07bc755f480ab4052c64484b40fd/data?style=centerme)
## State of the Data Enterprise Toolbox
This toolbox is a subset of the tools in the State of the Data toolbox that have been designed to be run with feature services or enterprise geodatabase features and will output existing content suitability indicators. 
![](http://nga.maps.arcgis.com/sharing/rest/content/items/40d970a508df481d97d846266ef5f21e/data?style=centerme)
## Metrics Explained
### Attribution Assessment
- Identifies attribution deficiencies at the feature level for user defined attributes
### Attribution Assessment (TDS 6.1 Schema)
- Identifies attribution deficiencies at the feature level based on mission or data requirements
### Completeness
- Identifies areas which may have missing features
- Line: total line length; Point: feature count; Surface: area
### Logical Consistency
- Creates a statistical summary of the attribution assessment over user defined areas of interest
### Logical Consistency (TDS 6.1 Schema)
- Creates a statistical summary of the attribution assessment of TDS 6.1 data over user defined areas of interest
### Positional Accuracy
- Statistically summarizes the positional accuracy of a feature class based on feature level metadata
### Positional Offset
- Compares two corresponding line feature classes to:
  - Match similar features
  - Calculate their offset from each other
  - Summarize those results over a given area of interest
### Positional Offset (TDS 6.1 Schema)
- Compares two corresponding line feature classes (one of which is in the TDS 6.1 schema) to:
  - Match similar features
  - Calculate their offset from each other
  - Summarize those results over a given area of interest
### Source Lineage
- Statistically summarizes the source of features in a feature class given a selected source attribute field
- Source field could be editor name, organization, product, etc.
### Source Lineage (TDS 6.1 Schema)
- Statistically summarizes the source of features in the TDS 6.1 schema source given the values in the TDS source field
### Temporal Accuracy from Change Detection
- Identifies features that may require updating due to currency and detected change
### Temporal Currency
- Statistically summarizes the source date of features in a feature class given a selected source date attribute field
- Source date could be the last edit date, the feature creation date, the source data of the imagery from which the feature was derived from, etc.
### Temporal Currency (TDS 6.1 Schema)
- Statistically summarizes the source date of features in the TDS 6.1 schema given the values in the TDS source date field
### Temporal Currency Comparison
- Comapres two outputs from **Temporal** **Currency** and ranks cells in terms 
### Thematic Accuracy (TDS 6.1 Schema)
- Identifies areas where feature collection requirements properly correlate to population
### Thematic Summary
- Performs a statistical summary of a feature subtype or selected attribute

# Installation and Use
The State of the Data tools use Python and Esri's arcpy library. In order for the tools to run, ArcGIS Desktop verision 10.4+ or ArcGIS Pro 1.2+ must be installed. If that condition is met, you should be able to clone this repo and run the tools as ArcGIS geoprocessing tools through ArcMap  or ArcGIS Pro or as stand alone scripts.

# Points of Contact
- Derek Silva (Derek.A.Silva@nga.mil)

# Developers
In aphabetical orther by last name:
- Gregory Brunner (gbrunner@esri.com)
- Andrew Chapkowski (achapkowski@esri.com)
- Tim Hollingshead (thollingshead@esri.com)
- Todd Wever (twever@esri.com)
