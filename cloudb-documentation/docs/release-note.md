# [Release Notes](release-note.md)

Welcome to the CloudB Release Notes! In this document, we'll highlight the new features, fixes, and optimizations that have been added to CloudB over the course of the year.

---

## October 2023

### Version 1.2.0 to 1.2.3

**Major update: Introduction of the Wind Farm Analysis Application in Acmonitor Connect**

#### Acmonitor Connect

- **Wind Farm Analysis app**: A specialized application designed for analyzing measurements collected by the Acmonitor stations.
- **Enhanced Upload Section**: The upload functionality in Acmonitor Connect now supports weather and wind time series data, allowing for seamless cloud-based analysis.
- **Devices Data upgrade**: Improvements to the Devices Data application offer a more intuitive selection process for time series visualization.

#### Eolyse

- **Project name creation**: Users will now be prompted to avoid using special characters when creating project names, streamlining data handling.  
- **Wind direction selection**: Issues related to Acventum backend's default wind direction data have been corrected, ensuring smoother operation.  
- **Custom wind turbine and direct usage**: Previously, custom wind turbines added by users were not immediately available for use. This has been addressed; Eolyse now scans for available turbines each time a new calculation is initiated.  

---

## September 2023

### Version 1.1.0

**Major update to enhance both general CloudB features and the Eolyse workspace.**

#### General CloudB Features

- **New URL**: Now operates under our company's domain name for a more cohesive brand experience.
- **UI Overhaul**: A simplified and intuitive user interface to improve user experience.
- **User Management Update**: Distinguish between internal users and clients, with the ability to specify account access permissions.
- **Cloud Architecture Update**: Transitioned to a new architecture with separate frontend and backend servers for optimized calculations on Google Cloud.
- **Enhanced Documentation**: Moved to GitHub Pages, offering more comprehensive guidance compared to the previous Monday documentation.

#### Eolyse

- **Wind Turbine Library**: Users can consult our extensive wind turbine library with improved data visualization and even add their own personalized wind turbine models.
- **API Maps Elevation**: Significant improvements in calculation time. Elevation data is now available worldwide.
- **Export Format**: New export format available in Delhom-branded Excel sheets for easy data extraction.
- **Simulation History**: Simplified tracking of past calculations across different applications.
- **Mesh Application**: Introduces the capability to calculate noise impact on a defined mesh grid.
- **Source and Receiver Building Updates**: Improved ease of definition for both sources and receivers.

---

## Jun 2023

### Version 1.0.6

#### General CloudB Features

- **User Management Service Upgrade** : we have upgraded our user management service by integrating a Redis server. This enhancement is expected to eliminate instances of unanticipated logouts. Users can now enjoy a more seamless and uninterrupted experience.
- **Cloud Run instance Upgrade** : to provide a robust infrastructure for handling concurrent requests, we have upgraded our Cloud Run Station from 512 MB RAM and 1 CPU to 8 GB RAM and 4 CPUs. This substantial upgrade allows us to increase the number of workers from 1 to 9, thereby significantly improving our capacity to manage simultaneous requests. You should notice a faster response time and improved system performance.

#### Eolyse:
We've addressed a crucial issue in the Eolyse workspace concerning the Chronologies app. Previously, users experienced problems with wind turbine model calculations due to model confusion. This patch fixes that issue, allowing users to perform their calculations without any model mix-up.

---



## April 2023

### Version 1.0.3 to 1.0.5

#### Eolyse

- **Patch** : Eolyse apps now replace default NaN elevation by 0 in the calculation. Minor patch to fix issues with dataset semicolon issue in app standard : added a round method in app standard data table display. Fixed CSV import separator issue with semicolon. Fixed CSV import source modeling dropdown filtering.
- **Simulation upgrade** : simulation can now be renamed, duplicated or deleted.

#### Acmonitor Connect

- **Updates** : plot line type changed from continuous to dot for non-equivalent acoustic data.

---

## March 2023

### Version 1.0.0 to 1.0.2

####  Eolyse

- **Patch** : Acventum and AcventumTimeSeries can now decode CSV files with ; separator. Projects can now be created normally on Eolyse