## User datasets

[Asia Pacific Network Information Centre](https://www.apnic.net/) (APNIC) provides all IP address blocks allocated to Australia. We
use an IP lookup service ([IP-API](http://ip-api.com/docs/)) to convert the obtained IP addresses into geographical locations. Since IP addresses in the last octet are likely to have identical geographical addresses returned by IP-API, you might have to generate more end-users (uniformly generated around each of the obtained geographical locations, etc.).

The up-to-date IP address blocks managed by APNIC can be found here (ftp://ftp.apnic.net/public/apnic/stats/apnic/delegated-apnic-extended-latest). You can then use [this tool](https://github.com/matthewvukomanovic/APNIC.Parser) to convert the IP format which APNIC releases into [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation) format.

#### List of contents:
File|Size|Fields|Description
:--|:--|:--|:--
australia-ip-ranges.csv|7606|CIDR block|All IP blocks assigned to Australia, extracted from APNIC as of 08/05/2018
users-aus.csv|4748x7|IP-Latitude-Longitude-PostCode-City-State-Country|All unique user location in Australia extracted from APNIC, after being converted by IP-API
users_aus.html|7606||Visualization of all users in users-aus.csv
