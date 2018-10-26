Barcelona Geodata
=================
The official shapefiles from Barcelona, converted to GeoJSON and TopoJSON for making your life easier.

## CDN
Here are the links for using the files directly, using [jsDelivr](https://www.jsdelivr.com):

Àrea estadística:
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/area-estadistica/area-estadistica_geo.json
```
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/area-estadistica/area-estadistica_topo.json
```

Àrea d'interès:
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/area-interes/area-interes_geo.json
```
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/area-interes/area-interes_topo.json
```

Barris:
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/barris/barris_geo.json
```
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/barris/barris_topo.json
```

Districtes:
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/districtes/districtes_geo.json
```
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/districtes/districtes_topo.json
```

Secció censal:
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/seccio-censal/seccio-censal_geo.json
```
```
https://cdn.jsdelivr.net/gh/molinx/bcn-geodata@latest/seccio-censal/seccio-censal_topo.json
```

## Recreate the files
Assuming that you have [ogr2ogr](https://trac.osgeo.org/gdal/wiki/DownloadingGdalBinaries) and [topojson](https://github.com/mbostock/topojson) installed:

- Run the script
```bash
$ ./convert.sh
```
- Voilà! Find the files in the `src/output` folder.

You can tweak the script for maintaining more properties from the original shapefile or for adjusting the simplification. Thanks to [@oscarfonts](https://github.com/oscarfonts) for the NTv2 ICC grid.

Source: Ajuntament de Barcelona / [CartoBCN](http://w20.bcn.cat/cartobcn/). License: CC-BY.