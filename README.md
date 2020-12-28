# mapping-notes

Notes and code for mapping stuffs

## Installations

### QGIS

From the QGIS site

### Postgres

Easy peasy with [Postgres App](https://postgresapp.com/).

### PostGIS

Comes with Postgres app. Start a [PostGIS database](https://postgis.net/workshops/postgis-intro/creating_db.html).

### GDAL

Especially for `ogr2ogr`

```
brew install gdal
```

## Imports

Geojson to PostGIS:

```
ogr2ogr -f "PostgreSQL" PG:"dbname=my_database user=postgres" "source_data.json" -nln destination_table
```

