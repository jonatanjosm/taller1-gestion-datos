
# Taller #1

Primer taller de la materia Gestión de datos.

## Integrantes

- Marysabel Mejia
- Jonatan Murcia


## Primer punto

Descripcion de los datos seleccionados:

### Homicidios accidentes de transito

El conjunto de datos cuenta con **59.810** registros, no presenta filas duplicadas ni tampoco valores faltantes.
Sus columnas son:

- **DEPARTAMENTO**: Categorica nominal
- **MUNICIPIO**: Categorica nominal
- **CODIGO DANE**: Categorica nominal
- **ARMAS MEDIOS**: Categorica nominal
- **FECHA HECHO**: Categorica ordinal
- **GENERO**: Categorica nominal
- **GRUPO ETARÍO**: Categorica nominal
- **DESCRIPCIÓN CONDUCTA**: Categorica nominal
- **CANTIDAD**: Cuantitativa

La columna **FECHA HECHO** se encuentra en un formato %d/%m/%Y, todos los registros cumplen con dicho formato.

La columna **DEPARTAMENTO** cuenta con 33 tipos de registros, es decir, no hay ningun departamento mal escrito.

La columna **CODIGO DANE** viene con un formato entre 7 y 8 numeros, es necesario corregirlo ya que el formato real del codigo dane es de 5 digitos.

No se encuentran otro tipos de incoherencias ni problemas de calidad de datos.

### Extorsion

El conjunto de datos cuenta con **69.137** registros, no presenta filas duplicadas ni tampoco valores faltantes.
Sus columnas son:

- **FECHA HECHO**: Categorica ordinal
- **COD_DEPTO**: Categorica nominal
- **DEPARTAMENTO**: Categorica nominal
- **COD_MUNI**: Categorica nominal
- **MUNICIPIO**: Categorica nominal
- **CANTIDAD**: Cuantitativa

La columna FECHA HECHO se encuentra en un formato %m/%d/%Y %H:%M:%S %p, todos los registros cumplen con dicho formato.

La columna **DEPARTAMENTO** cuenta con 33 tipos de registros, es decir, no hay ningun departamento mal escrito.

La columna **COD_MUNI** viene con un formato entre 4 y 5 numeros, es necesario corregirlo ya que esta columna hace referencia al mismo codio dane y el formato real del codigo dane es de 5 digitos.

No se encuentran otro tipos de incoherencias ni problemas de calidad de datos.

## Secuestro

El conjunto de datos cuenta con **18.642** registros, no presenta filas duplicadas ni tampoco valores faltantes.
Sus columnas son:

- **FECHA HECHO**: Categorica ordinal
- **COD_DEPTO**: Categorica nominal
- **DEPARTAMENTO**: Categorica nominal
- **COD_MUNI**: Categorica nominal
- **MUNICIPIO**: Categorica nominal
- **TIPO DELITO**: Categorica nominal
- **CANTIDAD**: Cuantitativa

No se encuentran otro tipos de incoherencias ni problemas de calidad de datos.

## Delitos sexuales

El conjunto de datos cuenta con **260.323** registros.
Sus columnas son:

- **DEPARTAMENTO**: Categorica nominal
- **MUNICIPIO**: Categorica nominal
- **CODIGO DANE**: Categorica nominal
- **ARMAS MEDIOS**: Categorica nominal
- **FECHA HECHO**: Categorica ordinal
- **GENERO**: Categorica nominal
- **GRUPO ETARIO**: Categorica nominal
- **CANTIDAD**: Cualitativa
- **delito**: Categorica nominal

En total existen **18.583** filas duplicadas.

Las siguientes filas cuentan con registros faltantes o nullos:

- **MUNICIPIO**:         1
- **CODIGO DANE**:       1
- **GENERO**:          304
- **GRUPO ETARIO**:    53

La columna **FECHA HECHO** se encuentra en el formato %d/%m/%Y

La columna **CODIGO DANE** viene con un formato entre 7 y 8 numeros, es necesario corregirlo ya que el formato real del codigo dane es de 5 digitos.


No se encuentran otro tipos de incoherencias ni problemas de calidad de datos.

## Segundo punto

### 2.1 ¿Cuáles han sido los departamentos (TOP 3) más afectados en términos de cantidad de delitos cometidos en los últimos 5 años?

#### 2.1.1 Delitos sexuales
|Top|Departamento|Cantidad|
|-|-:|-:|
|1|**Cundinamarca**|32.542|
|2|**Antioquia**|19.817|
|3|**Valle del cauca**|12.762|

#### 2.1.2 Secuestro
|Top|Departamento|Cantidad|
|-|-:|-:|
|1|**Valle del cauca**|86|
|2|**Antioquia**|82|
|3|**Cauca**|70|

#### 2.1.3 Homicidio accidente de transito
|Top|Departamento|Cantidad|
|-|-:|-:|
|1|**Cundinamarca**|3.880|
|2|**Antioquia**|3.700|
|3|**Cauca**|3.114|

#### 2.1.4 Extorsion
|Top|Departamento|Cantidad|
|-|-:|-:|
|1|**Antioquia**|5.799|
|2|**Bogota D.C.**|5.247|
|3|**Valle del Cauca**|4.484|

### 2.2 Para los casos en los que aplique, ¿cuál ha sido el arma o medio más común para cometer el delito?

#### 2.2.1 Delitos sexuales
 En este delito el medio con mayor numero de reportes fue ***Sin empleo de armas*** con 130.259 seguido de ***No Reportado*** con 70.048.
 El tipo de arma mas usado fue ***Contundentes*** con una cantidad de 45.995

#### 2.2.2 Homicidio accidente de transito

- **VEHICULO:**	38236

#### 2.2.2 Extorsion
No aplica

#### 2.2.2 Secuestro
No aplica

### 2.3 Para los casos en los que aplique, ¿cómo ha sido la proporción de géneros y grupos etarios que han estado involucrados en este tipo de delito? ¿Han variado con el paso de los años?

#### 2.3.1 Delitos Sexuales 

#### 2.3.1.1 Genero
![Alt text](https://i.imgur.com/39AByzn.png )

		
|GRUPO ETARIO  |  CANTIDAD  |  PORCENTAJE	|
|-|-:|-:|	
|ADOLESCENTES	|50691|	18.87 %|
|ADULTOS|	84453|	31.44 %|
|MENORES|	133339|	49.64 %|
|NO REPORTADO|	117|	0.04 %|

A traves de los años:

![Alt text](https://i.imgur.com/BKL44Cf.png )


Se ve que la proporcion entre mujeres y hombres es muy diferente, la mayoria de victimas son mujeres y esta proporcion no cambia al pasar de los años, es casi identico.

#### 2.3.1.1 Grupo etario

		
|GRUPO ETARIO |   CANTIDAD |   PORCENTAJE	|
|-|-:|-:|	
|ADOLESCENTES|	50691|	18.87 %|
|ADULTOS|	84453|	31.44 %|
|MENORES	|133339	|49.64 %|
|NO REPORTADO|	117|	0.04 %|


![Alt text](https://i.imgur.com/RKYoqFj.png )
A traves de los años:
![Alt text](https://i.imgur.com/iBVEBFn.png )

Por grupo etario se aprecia que la mayoria son menores, hay un cambio de proporcion en los ultimos 2 años en los que crece la cantidad de adolescentes.

#### 2.3.2 Homicidio

#### 2.3.2.1 Genero
		
|GENERO	|	CANTIDAD|    PORCENTAJE|
|-|-:|-:|	
|FEMENINO |	13149 |	20.02 % |
|MASCULINO |	52468 |	79.89 %|
|NO REPORTADO |	61 |	0.09 % |

![Alt text](https://i.imgur.com/08dm8eC.png )

A traves de los años:

![Alt text](https://i.imgur.com/BLEth8n.png )

Separando por genero el porcentaje de hombres es casi el 80% siendo un porcentaje casi que permanente todos los años

#### 2.3.2.2 Grupo etario

		
|GRUPO ETARÍO |	CANTIDAD |    PORCENTAJE|	
|-|-:|-:|
|ADOLESCENTES |	3017 |	4.59 % |
|ADULTOS |	60386 |	91.94 % |
|MENORES |	2229 |	3.39 % |
|NO REPORTADO |	46 |	0.07 % |


![Alt text](https://i.imgur.com/5K6oaNN.png)

A traves de los años:

![Alt text](https://i.imgur.com/8QDN5df.png )

Lo mismo ocurre separando por grupo etario el cual el mayor porcentaje es adultos y se mantiene casi igual la proporcion sin importar el año.

### 2.4 ¿Se evidencia alguna tendencia para cometer dicho delito en algún mes particular del año?

#### 2.4.1 Delitos sexuales

A traves de los años:

![Alt text](https://i.imgur.com/ypHbPp7.png)

En su mayoria casi todos los años presentan un comportamiento similar todos los meses, como por ejemplo en el mes 5 (Mayo) hay un pico de aumento de delitos al igual que en el mes 12 (Diciembre) hay una disminucion en la cantidad de delitos sexuales.

#### 2.4.2 Secuestros

A traves de los años:


![Alt text](https://i.imgur.com/lW7jijC.png)

No es muy evidente un comportamiento por mes pero se alcanzan a apreciar algunos patrones en varios años:

- Diminucion en el mes de Febrero (2)
- Aumentos en el mes de Marzo (3)
- Aumentos en el mes de Mayo (4)

#### 2.4.3 Homicidios por accidentes de transito

A traves de los años:
![Alt text](https://i.imgur.com/2g1csky.png)

Los homicidios presentan algunos patrones en los meses:
- Aumento en los meses de Marzo, Julio, Octubre y Diciembre
- Disminucion en los meses de Febrero, Abril, Septiembre y Noviembre.

#### 2.4.4 Extorsiones

A traves de los años:

![Alt text](https://i.imgur.com/7CEltsb.png)

En las extorsiones parece no haber un patron en los meses a excepcion del mes de octubre que aparenta una disminucionen todos los años y un aumento en Febrero.

### 2.5. Para los casos en los que se disponga del detalle del delito o de una descripción, como por ejemplo en delitos sexuales y secuestro, ¿cuáles son las descripciones o modalidades más comunes?

#### 2.5.1. Delitos sexuales.

Para este delito se encontraron varios descripciones de delitos repetidas por lo que se unificaron, los valores unicos fueron los siguientes:

- ARTÍCULO 209. ACTOS SEXUALES CON MENOR DE 14 AÑOS
- ARTÍCULO 205. ACCESO CARNAL VIOLENTO
- ARTÍCULO 206. ACTO SEXUAL VIOLENTO
- ARTÍCULO 208. ACCESO CARNAL ABUSIVO CON MENOR DE 14 AÑOS
- ARTÍCULO 210 A. ACOSO SEXUAL
- ARTÍCULO 210. ACCESO CARNAL O ACTO SEXUAL ABUSIVO CON INCAPAZ DE RESISTIR
- ARTÍCULO 211. ACCESO CARNAL O ACTO SEXUAL ABUSIVO (CIRCUNSTANCIAS AGRAVACIÓN)
- ARTÍCULO 211 A. ACCESO CARNAL O ACTO SEXUAL ABUSIVO CON MENOR DE 14 AÑOS
- ARTÍCULO 207. ACCESO CARNAL O ACTO SEXUAL EN PERSONA PUESTA EN INCAPACIDAD DE RESISTIR
- ARTÍCULO 218. PORNOGRAFÍA CON MENORES
- ARTÍCULO 213. INDUCCIÓN A LA PROSTITUCIÓN
- ARTÍCULO 214. CONSTREÑIMIENTO A LA PROSTITUCIÓN
- ARTÍCULO 219 A. UTILIZACIÓN O FACILITACIÓN DE MEDIOS DE COMUNICACIÓN PARA OFRECER SERVICIOS SEXUALES DE MENORES
- ARTÍCULO 217. ESTÍMULO A LA PROSTITUCIÓN DE MENORES
- ARTÍCULO 217 A. DEMANDA DE EXPLOTACION SEXUAL COMERCIAL DE PERSONA MENOR DE 18 AÑOS DE EDAD
- ARTÍCULO 216. CONSTREÑIMIENTO O INDUCCIÓN A LA PROSTITUCIÓN (CIRCUNSTANCIAS AGRAVACIÓN)
- ARTÍCULO 213 A. PROXENETISMO CON MENOR DE EDAD
- ARTÍCULO 219 B. OMISIÓN DE DENUNCIA

La distribucion por tipo de delito del top 5 fue la siguiente :

	
|Delito | CANTIDAD |
|-|-:|	
|ARTÍCULO 209. ACTOS SEXUALES CON MENOR DE 14 AÑOS |	92952
|ARTÍCULO 208. ACCESO CARNAL ABUSIVO CON MENOR DE 14 AÑOS |	60172
|ARTÍCULO 205. ACCESO CARNAL VIOLENTO |	40564|
|ARTÍCULO 206. ACTO SEXUAL VIOLENTO |	27976 |
|ARTÍCULO 210 A. ACOSO SEXUAL |	17109|

![Alt text](https://i.imgur.com/8pi4KYD.png)

#### 2.5.2. Secuestro.

En el caso de secuestro solo existen 2 tipos, la cantidad o distribucion por cada uno fue la siguiente:


|DELITO | CANTIDAD|	
|-|-:|	
|SECUESTRO EXTORSIVO |	17235 |
|SECUESTRO SIMPLE |	9820 |

![Alt text](https://i.imgur.com/UJiZmuV.png)

#### 2.5.3. Homicidio

Al igual que en el delito de secuestro solo se encuentran 2 tipo, la diferencia entre las cantidades del uno y el otro es enorme, no vale la pena representarlo en una grafica ya que es casi imperceptible el segundo tipo.

Las cantidades fueron las siguientes:

	
|DESCRIPCIÓN CONDUCTA | CANTIDAD|	
|-|-:|
|ARTÍCULO 109. HOMICIDIO CULPOSO ( EN ACCIDENTE DE TRÁNSITO) |	65667|
|ARTÍCULO 110. HOMICIDIO CULPOSO ( CIRCUNSTANCIAS DE AGRAVACIÓN) |	11|




## Tercer punto

_A partir de alguno de los conjuntos de datos seleccionados, visualice una serie de tiempo por año y mes que permita comparar la cantidad de delitos cometidos para los departamentos con mayor ocurrencia durante los últimos 5 años. Para que los resultados entre departamentos sean comparables, es importante que normalice las cantidades obtenidas por cantidad de habitantes. En este archivo puede encontrar la población por departamento para el año 2018. Asuma que la población no ha cambiado con el paso de los años._

Antes de trabajar con el conjunto de datos de la población fue necesario cambiar algunos nombres de departamentos para estandarizar esos valores con el conjunto de datos a escoger, los valores reemplazados fueron los siguientes:

- **La Guajira** = Guajira
- **Archipiélago de San Andrés, Providencia y Santa Catalina** = San Andrés
- **Valle del Cauca** = Valle

Los departamentos con su respectiva población son los siguientes:

|departamento | población|	
|-|-:|
|Amazonas	| 48144|
|Antioquia	| 2427129|
|Arauca	| 85585|
|Atlántico	| 1206319|
|Bolívar	| 973045|
|Boyacá	| 172548|
|Caldas	| 434403|
|Caquetá	| 168346|
|Casanare	| 168433|
|Cauca	| 318059|
|Cesar	| 490075|
|Chocó	| 129237|
|Cundinamarca	| 7412566|
|Córdoba	| 490935|
|Guainía	| 31514|
|Guajira	| 188014|
|Guaviare	| 52815|
|Huila	| 357392|
|Magdalena	| 499192|
|Meta	| 531275|
|Nariño	| 392930|
|Norte de Santander	| 711715|
|Putumayo	| 56398|
|Quindío	| 295208|
|Risaralda	| 467269|
|San Andrés	| 55291|
|Santander	| 581130|
|Sucre	| 277773|
|Tolima	| 529635|
|Valle	| 2227642|
|Vaupés	| 29850|
|Vichada	| 20936|

El conjunto de datos de delitos seleccionado fue el de ***Homicidios.***

Para determinar cuales eran los departamentos con mayores indices por cantidad de habitantes se aplico una funcion de normalizacion en la que se dividio la cantidad de delitos sobre la cantidad de habitantes en su correspondiente departamento.

Una vez hecho esto el top 5 departamentos fueron los siguientes:

	
|DEPARTAMENTO| CANTIDAD|	
|-|-:|
|BOYACÁ |	0.004231|
|PUTUMAYO |	0.003759|
|ARAUCA |	0.003225|
|CAUCA |	0.003223|
|GUAJIRA |	0.002654|

![Alt text](https://i.imgur.com/CXC7oGR.png)
_Plot line - Homicidios por cantidad de habitante / departamento_


![Alt text](https://i.imgur.com/6TITD1q.png)
_Plot bar - Homicidios por cantidad de habitante / departamento_


#### 3.1 Observaciones

Haciendo un analisis de las graficas se puede decir que:

- En los meses de diciembre hay un aummento considerable en casi todos los departamentos.
- En el putumayo hubo un incremento considerable a partir del diciembre del 2020 superando a Boyaca que esta entre los mas altos todos los años, ¿podra haberse dado por la cuarentena causada por el covid 19 dada ese año?
- El mes con menor cantidad de homicidio en todos los departamentos fue en abril del 2020, casi un mes luego de iniciar la cuarentena en el pais, luego de eso Arauca tuvo una alta cantidad de homicidios superando a todos los departamentos por 2 meses consecutivos.
- Boyaca es el municiopio que mas picos presenta indicando mayor accidentalidad que los demas departamentos.
- El Cauca a diferencia de los otros departamentos ha tenido un comportamiento casi identico todos los años manteniendo las mismas proporciones (Aumento de homicidios a mitad de año, disminucion a finales, aumento a inicios, disminuye un par de meses y a mediados nuevamente vuelve a aumentar)

## Cuarto Punto

_A partir de los conjuntos de datos seleccionados, construya un único dataset que integre la totalidad de los delitos ocurridos por departamento y municipio. Muestre los valores normalizados por cantidad de habitantes realizando un proceso similar al del punto anterior. En este archivo puede encontrar proyecciones anuales de las poblaciones por departamento. Utilice la proyección para el año en curso. Considere solamente los municipios con más de 1 millón de habitantes._

### Data set Proyeccion poblacion municipal
Para el conjunto de datos de ***Proyeccion poblacion municipal*** se ajustaron los registros de **DPM**, que representa el codigo Dane, completando ocon un cero a la izquierda los valores que tuvieran menos de 5 caracteres.
Luego de esto se aplicaron los siguientes filtros:

- **Año** = 2022
- **Area Geografica** = Total
- **Total** mayor a 1'000.000 (un millon )

Los datos resultantes de aplicar los filtros anteriores fueron los siguientes:

	    
|DPMP|	DP|	DPNOM |	MPIO |	AÑO |	ÁREA GEOGRÁFICA |	Total|					
|-|-:|-|-|-|-|-:|
|**05001** |	5 |	Antioquia |	Medellín |	2022 |	Total |	2'612.958|
|**08001** |	8 |	Atlántico |	Barranquilla |	2022 |	Total |	1'312.473 |
|**11001** |	11 |	Bogotá, D.C. |	Bogotá, D.C. |	2022 |	Total |	7'901.653|
|**13001** |	13 |	Bolívar |	Cartagena de Indias |	2022 |	Total |	1'055.035 |
|**76001** |	76 |	Valle del Cauca |	Cali |	2022 |	Total |	2'280.907 |

### Data sets delitos | Homicidios | Secuestros | Extorsiones | Delitos sexuales |

En el caso de los conjuntos de datos de delitos fue necesario estandarizar el codigo Dane para poder utilizarlo como index y relacionarlo entre todos, tambien, se cambiaron los nombres de la columna _CANTIDAD_ reemplazandolo por el nombre del delito para al momento de unir los conjuntos dicha columna tenga el nombre del delito correspondiente. 
Se hizo lo siguiente para cada set de datos:

- **Secuestro:** 

        1) Para el _Codigo Dane_ se convirtio a formato str y se completaron los campos que no tuvieran los 5 caracteres agregando un 0 a la izquierda.
        2) Se reemplazo el nombre de la columna COD_MUNI por CODIGO DANE
        3) Se reemplazo el nombre de la columna CANTIDAD por SECUESTRO

- **Extorsion:**
        
        1) Para el _Codigo Dane_ se convirtio a formato str y se completaron los campos que no tuvieran los 5 caracteres agregando un 0 a la izquierda.
        2) Se reemplazo el nombre de la columna COD_MUNI por CODIGO DANE
        3) Se reemplazo el nombre de la columna CANTIDAD por EXTORSION

- **Homicidios:**
        
        1) Para el _Codigo Dane_ se convirtio a formato str y se quitaron los ultimo 3 caracteres ya que venia en el formato XXXXX000 luego se completaron los campos que no tuvieran los 5 caracteres agregando un 0 a la izquierda.
        2) Se reemplazo el nombre de la columna CANTIDAD por SECUESTRO

- **Delitos Sexuales:**
        
        1) Para el _Codigo Dane_ se convirtio a formato str y se quitaron los ultimo 5 caracteres ya que venia en el formato XXXXX000.0 luego se completaron los campos que no tuvieran los 5 caracteres agregando un 0 a la izquierda.
        2) Se reemplazo el nombre de la columna CANTIDAD por DELITOS SEXUALES

Una vez ajustados y estandarizados los valores del DANE se filtraron en todos los conjuntos de datos los departamentos obtenidos en el filtro hecho al set de datos de **Proyeccion poblacion municipal**.

Luego se normalizaron los valores de cantidad de delitos diviendolo entre la cantidad de habitantes por municipio

Para finalizar se unieron todos los conjuntos de datos usando como llave el campo ***CODIGO DANE***, ademas, se agrego un campo llamado ***TOTAL DELITOS*** el cual suma todos los delitos. La estructura del nuevo dataset es:

- ***Columnas:***

        - CODIGO DANE: Categorica nominal
        - SECUESTRO: Cuantitativa
        - EXTORSION: Cuantitativa
        - HOMICIDIOS: Cuantitativa
        - DELITOS SEXUALES: Cuantitativa
        - DPNM: Categorica nominal
        - MPIO: Categorica nominal
        - TOTAL DELITOS: Cuantitativa

- **Cantidad registros:** 5

	
|CODIGO DANE | SECUESTRO |	EXTORSION |	HOMICIDIOS |	DELITOS SEXUALES |	DPNOM |	MPIO |	TOTAL DELITOS |
|-:|-:|-:|-:|-:|-|-|-:|
|05001 | 0.000323 | 0.002473 | 0.001177 | 0.004817 | Antioquia | Medellín | 0.008790|
|08001 | 0.000130 | 0.001522 | 0.000728 | 0.004624 | Atlántico | Barranquilla | 0.007004|
|11001 | 0.000188 | 0.001484 | 0.000771 | 0.004105 | Bogotá, D.C. | Bogotá, D.C. | 0.006549|
|13001 | 0.000127 | 0.001605 | 0.000943 | 0.004297 | Bolívar | Cartagena de Indias | 0.006971|
|76001 | 0.000414 | 0.001862 | 0.001442 | 0.005513 | Valle del Cauca | Cali | 0.009231|


![Alt text](https://i.imgur.com/ZjLGFF2.png)
