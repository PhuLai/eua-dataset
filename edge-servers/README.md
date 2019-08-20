## Edge server datasets

According to Hu et al. [1], edge servers can be deployed at or around LTE base station (BS) sites. Australian Communications and Media 
Authority (ACMA) publishes the radio-comms license dataset [2] that contains the geographical location of all cellular base stations in 
Australia, which we use as the edge server dataset. For your convenience, we have uploaded the part of the dataset that stores the latitude and longitude of BS (**site.csv**). Note that this data is owned by ACMA, the use of this dataset must conform to ACMA's regulations. Visit [ACMA](https://www.acma.gov.au/Industry/Spectrum/Radiocomms-licensing/Register-of-radiocommunications-licences/radiocomms-licence-data) for more info about the data.

In order to view the HTML map, please use your GoogleMap API key.

#### List of contents:
File|Size|Fields|Description
:--|:--|:--|:--
site.csv|95562x10|SiteID-Latitude-Longitude-Name-State-LicensingAreaID-PostCode-SitePrecision-Elevation-HCISL2|All BS of all telcos in Australia|
site-optus-melbCBD.csv|125x10|SiteID-Latitude-Longitude-Name-State-LicensingAreaID-PostCode-SitePrecision-Elevation-HCISL2|All Optus BS in Melbourne CBD area|
all-telco-sites-metro.html|9318||Visualization of all BS of all telcos in Melbourne Metropolitan area (9318 base stations)
all-optus-sites-metro.html|1464||Visualization of all BS of Optus telco in Melbourne Metropolitan area, including Melbourne CBD (1464 base stations)


[1] Hu, Y.C., Patel, M., Sabella, D., Sprecher, N., Young, V.: Mobile Edge Computing A key technology towards 5G. Tech. Rep. 11, European Telecommunications Standards Institute (2015), http://www.etsi.org/images/files/ETSIWhitePapers/etsi_wp11_mec_a_key_technology_towards_5g.pdf 

[2] https://www.acma.gov.au/Industry/Spectrum/Radiocomms-licensing/Register-of-radiocommunications-licences/radiocomms-licence-data
