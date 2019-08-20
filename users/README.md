## User datasets

[Asia Pacific Network Information Centre](https://www.apnic.net/) (APNIC) provides all IP address blocks allocated to Australia. We
use an IP lookup service ([IP-API](http://ip-api.com/docs/)) to convert the obtained IP addresses into geographical locations. Since IP addresses in the last octet are likely to have identical geographical addresses returned by IP-API, you might have to generate more end-users (uniformly generated around each of the obtained geographical locations, etc.).

The up-to-date IP address blocks managed by APNIC can be found here (ftp://ftp.apnic.net/public/apnic/stats/apnic/delegated-apnic-extended-latest). You can then use [this tool](https://github.com/matthewvukomanovic/APNIC.Parser) to convert the IP format which APNIC releases into [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation) format.

Below is the polygon coordinates of the Melbourne CBD area, which can be used to get all users within the area.
MELBOURNE_CBD_POLYGON = [(144.9513187173424,-37.81313439053935), (144.9549965367283,-37.82117612446662), (144.9748200238013,-37.81524024624075), (144.9715203527905,-37.80786609093214), (144.9705381920906,-37.80755065732971), (144.9513187173424,-37.81313439053935)]

In order to view the HTML map, please use your GoogleMap API key.

#### List of contents:
File|Size|Fields|Description
:--|:--|:--|:--
australia-ip-ranges.csv|7606|CIDR block|All IP blocks assigned to Australia, extracted from APNIC as of 08/05/2018
users-aus.csv|4748x7|IP-Latitude-Longitude-PostCode-City-State-Country|All unique user location in Australia extracted from APNIC, after being converted by IP-API
users_aus.html|7606||Visualization of all users in users-aus.csv
users-melbcbd-generated.csv|816x2|Latitude-Longitude|Uniformly generated users in the Melbourne CBD area.
users-melbcbd-generated.html|816||Visualization of all users in users-melbcbd-generated.csv
users-melbmetro-generated.csv|131312x2|Latitude-Longitude|Uniformly generated users in the Melbourne metropolitan area.
users-melbmetro-generated.zip|131312||Visualization of all users in users-melbmetro-generated.csv
