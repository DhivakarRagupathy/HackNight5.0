# HackNight5.0



# PotHole Detector 



# MISSION :

To detect potholes present in Roads via a camera mounted to public/private vehicles and intimate the  corresponding authorities for necessary act.

The System updates the Geo-Location of every potholes detected to a centralized data center with the image and severity.

The data in the data center is used to analyze Road conditions for immediate  and prioritized actions. 

The Analyzed Report Lists the potholes in the most commuted roads and helps the authorities to decide the quickness of the action.


# Tech Stack :

Various Azure API services.

# Azure Services List :

PotHole Detection : **Azure Function**

ML Model to detect PotHoles : **Azure Custom vision API - Predictions**

Data Annotation & Training of Modal : **Azure Custom vision API - Training**

API Host : **Azure deployment**

Database : **Azure SQL Server**

Primary Host : **Azure Virtual Machine**

Data visualization : **Azure Power BI**

Object recognition : **Python - OpenCV**

# FUTURE SCOPE :

Integrating with any MAPs (Google Maps,Here Maps,etc) to decide the safest road for commute.

# Implementation

The Recorder video clip will be converted into image frames using open CV and will be shared to the Azure Custom vision Api to detect the Potholes. The Images with potholes prediction percentage of 50 or more will be considered and the corresponding geo-location of the image will be send to the Azure functions api. The azure function api will take care of persisting the received information into the azure sql server database. The admin can extract the data and a visualize the data with Azure Power BI reports for analytics and can  group the data by Date, Location, Seviority, Most Used etc.. 








