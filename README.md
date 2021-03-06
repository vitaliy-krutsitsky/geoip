# geoip
Geo IP lookup service

A library for searching Location information (country, city, region) by IP.

## Sample usage:
```java
    Location location = lookupService.getLocation("217.71.44.212");
    assertEquals("EE", location.countryCode);
    assertEquals("Estonia", location.countryName);
    assertEquals("Tallinn", location.city);
    assertEquals("01", location.region);
    assertEquals(59.4339, location.latitude, 0.0001);
    assertEquals(24.728104, location.longitude, 0.000001);
```


## How to start

Download the latest jar from out repository: https://repo.codeborne.com/com/codeborne/geoip/

# Data source

We use the file downloaded from http://dev.maxmind.com/geoip/legacy/geolite/

# Thanks

Many thanks to these incredible tools that help us creating open-source software:

![Intellij IDEA](http://www.jetbrains.com/idea/docs/logo_intellij_idea.png)

![YourKit Java profiler](http://selenide.org/images/yourkit.png)

# License
geo-ip is open-source project and distributed under [MIT](http://choosealicense.com/licenses/mit/) license

This product includes GeoLite data created by MaxMind, available from 
<a href="http://www.maxmind.com">http://www.maxmind.com</a>.