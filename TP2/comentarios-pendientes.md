# CELL 38

> PENDIENTE: QUE HACEMOS CON LOS CAMPOS COMENTADOS. LOS ELIMINAMOS O LOS DEJAMOS ABAJO PARA MOSTRAR COSAS QUE NO TUVIERON EXITO?
>
> Yo pienso que son gráficos que no funcionaron, y que no deberían estar en el informe. Si fuesen líneas de pensamiento o hipótesis que no se pudieron probar, entonces sí, pero gráficos nomás no creo que valgan la pena. Los borro y coloco en este archivo por si los queres usar en algún momento

```
# masc_dep = data[data["tipo"]=="apartment"]
# sns.scatterplot(data=masc_dep, x='sup_m2_total', y='precio_usd', palette="deep")
# plt.grid()
# plt.show()
# manf_sort = pd.get_dummies(data['ambientes_cat_code']).sum().sort_values(ascending = False)
# plt.figure(figsize=(5,5))
# sns.barplot(x = manf_sort.index, y = manf_sort.values)
# plt.show()
# manf_sort = pd.get_dummies(data['ambientes_cat']).sum().sort_values(ascending = False)
# plt.figure(figsize=(5,5))
# sns.barplot(x = manf_sort.index, y = manf_sort.values)

# plt.show()
#masc_barrio = data[data["municipio"]=="Almagro"]
#sns.scatterplot(data=masc_barrio, x='sup_m2_total', y='precio_usd', palette="deep")
#plt.grid()
#plt.show()
# masc_barrio = data[data["municipio"]=="Almagro"]
# sns.set_style('darkgrid')
# plt.figure(figsize=(6, 4))
# sns.boxplot(data=masc_barrio, x= "tipo", y="sup_m2_total")

# plt.xlabel("tipo")
# plt.ylabel("sup_m2_total")
# plt.title("Superficie total por tipo de inmueble ")
# masc_barrio = data[data["municipio"]=="Almagro"]
# sns.set_style('darkgrid')
# plt.figure(figsize=(6, 4))
# sns.boxplot(data=masc_barrio, x= "tipo", y="precio_usd_por_m2")

# plt.xlabel("tipo")
# plt.ylabel("precio_usd_por_m2")
# plt.title("Precio/m2 por tipo de inmueble ")
# masc_barrio = data[data["municipio"]=="Lomas de Zamora"]
# sns.scatterplot(data=masc_barrio, x='sup_m2_total', y='precio_usd', palette="deep")
# plt.grid()
# plt.show()
#mostramos un boxplot para los outliers por tipo de propiedad
data.boxplot(column= "precio_usd", by="tipo")
plt.show()


#sns.histplot(data['ambientes_cat'], bins = 5);
#masc_barrio = data[data["municipio"]=="Tigre"]
#sns.scatterplot(data=masc_barrio, x='sup_m2_total', y='precio_usd', palette="deep")
#plt.grid()
#plt.show()
```

>PENDIENTE- VER SI AJUSTAMOS EL MODELO REDUCIENDO LA CANTIDAD DE DATOS
> dejo aca los codigos

```
# superficie_min=15
# superficie_max=1000

# data = data[(data.sup_m2_total <= 1000) & (data.sup_m2_total >= 15)]

# data = data[(data.precio_usd <= 4000000)]


# # Generamos una función que resume los coeficientes, el intercepto y el R2
# # "model" = objeto con el modelo
# # "X" = matrix de variables independientes

# def sum_mod(lr, X):
#     a = pd.DataFrame(lr.coef_ , X_simple.columns.values)
#     a = a.append(pd.DataFrame([lr.intercept_, lr.score(X_simple, y)], index=['Intecept','R2']))
#     return(a)
```
