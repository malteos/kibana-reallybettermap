# Kibana Reallybettermap Panel

Modification of [Kibana's Bettermap Panel](http://www.elasticsearch.org/guide/en/kibana/current/_bettermap.html) - Supports multiple locations for search items. 

## Format

```
{geo_field: [
    {lat: 12.34, lng: 56.78},
    {lat: 23.45, lng: 44.22}]
]}
```

Mapping type of *geo_field* needs to be **not_analyzed**. 

## Installation

To install the **reallybettermap** you just need to put the **reallybettermap** folder in the app/panels/ directory of your Kibana installation. After that you just need to add **reallybettermap** to the panel_names list in your kibana config.js.

```
/* [...] */

    panel_names: [

      'reallybettermap', /* add this entry */

      'histogram',
      'map',
      'goal',

      /* [...] */
    ]

/* [...] */
```

The panel was tested with Kibana 3.1.0. Please use a modern web browser like Chrome or Firefox. 