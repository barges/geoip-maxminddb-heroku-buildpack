# Heroku Buildpack: GeoLite2 data

This is an unofficial [Heroku buildpack](https://devcenter.heroku.com/articles/buildpacks)
that supports [maxminddb](https://github.com/yhirose/maxminddb) ruby gem.

Define `GEOIP_DB_PUBLIC_URI` ENV variable from where to fetch the files.

A separate process should be placing the files there once a day/week. Depends on the update frequency.

Files should be in .tar.gz format:

```
❯ tar -tzf ~/Downloads/GeoLite2-City.mmdb.tar.gz
GeoLite2-City_20240319/
GeoLite2-City_20240319/LICENSE.txt
GeoLite2-City_20240319/COPYRIGHT.txt
GeoLite2-City_20240319/GeoLite2-City.mmdb
GeoLite2-City_20240319/README.txt
```
