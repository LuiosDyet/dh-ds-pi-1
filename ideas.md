# Ideas y dudas

## Tips de Ioni

-   Tratar de no imputar la variable precio porque es la variable target y puede ensuciar.
-   Convertir nro de rooms en variable categórica. Sin dato, 1, 2, 3, 4 o mas.

## Común

-   revisar si hay propiedades repetidas
-   corroborar si price_aprox_usd y price_aprox_local_currency coinciden o no
-   Bonus: Identificar datos faltantes a partir de la descripción
-   Relación superficie/ubicación
-   Revisar si el url Properatti provee información valiosa.
-   Revisar qué cotización de dólar se usa en cada valuación. ¿Cuál era la cotización a la fecha de la creación de la tabla?

## Dos grupos:

### Ubicación/precio: Luis, Camila, Irania

-   corroborar si place_with_parent_names coincide con place_name, country_name, country_name / Listo (Luis)
-   ¿qué es geonames_id? Es un sistema de geo localización relacionada a wgs84. Ver si se puede inferir latitud y longitud a partir de este dato.
-   corroborar si lat y lon coinciden con lat-lon / Listo (Luis)

### Superficie/precio: Jonathan, Ornella

-   se puede inferir m2desde price_per_m2, price_usd_per_m2
-   Inferir cantidad de habitaciones en base al tipo de propiedad y superficie
