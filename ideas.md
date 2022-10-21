# Ideas y dudas

## Común

-   revisar si hay propiedades repetidas
-   corroborar si price_aprox_usd y price_aprox_local_currency coinciden o no
-   Bonus: Identificar datos faltantes a partir de la descripción
-   Relación superficie/ubicación
-   Revisar si el url Properatti provee información valiosa.

## Dos grupos:

### Ubicación/precio: Luis, Camila, Irania

-   corroborar si place_with_parent_names coincide con place_name, country_name, country_name
-   ¿qué es geonames_id? Es un sistema de geolocalización relacionada a wgs84. Ver si se puede inferir latitud y longitud a partir de este dato.
-   corroborar si lat y lon coinciden con lat-lon

### Superficie/precio: Jonathan, Ornella

-   se puede inferir m2desde price_per_m2, price_usd_per_m2
-   Inferir cantidad de habitaciones en base al tipo de propiedad y superficie
