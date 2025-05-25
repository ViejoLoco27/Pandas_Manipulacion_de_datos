# Pandas: Manipulación y transformación de datos
![Static Badge](https://img.shields.io/badge/Oracle_Next_Education-blue?style=plastic&logo=python&logoColor=green&logoSize=auto&label=Alura%20Latam)
![Static Badge](https://img.shields.io/badge/Proyecto-blue?style=plastic&logo=pandas&logoColor=green&logoSize=auto&label=Pandas%20ETL)
![Static Badge](https://img.shields.io/badge/Certificado_del_curso-Alura?logo=pandas&color=%231e4181&link=https%3A%2F%2Fapp.aluracursos.com%2Fcertificate%2Fguz27-unameconomia%2Fpandas-transformacion-manipulacion-datos)

## **📋Problemática del proyecto**
Sugerir al anfitrión un precio a cobrar por tarifas diarias que garantice ganancias en momentos de alta demanda.

## **📋Procedimiento**
- **1. Importando librerías y datos**
			-  1.1. Normalización de datos
- **2. Transformación de strings a datos numéricos**
			- 2.1. Manipulación de datos de tiempo
- **3. Desafío de tokenización de datos**
- **4. Manipulación de datos de tiempo**
			- 4.1. Resultados
					-  convertir la columna precio a datos numéricos
					- agrupar los precios respecto a las fechas para determinar en qué fecha hubo más demanda


## **📋Resultado**
|fecha|precio|
|---|---|
|2016-06|3694391\.0|
|2016-07|3537715\.0|
|2016-08|3510185\.0|
|2016-12|3480845\.0|
|2016-05|3478445\.0|
|2016-10|3388931\.0|
|2016-09|3333501\.0|
|2016-11|3281985\.0|
|2016-04|3170741\.0|
|2016-03|3117058\.0|
|2016-02|2576306\.0|
|2016-01|2053910\.0|
|2017-01|220372\.0|

## 🤖 Funciones empleadas durante el ejercicio

 - `pd.read_json`
 - `pd.json_normalize`
 - `.explode`
 - `.reset_index(drop=True, inplace=True`
 - `.astype(np.int64)`
 - `.apply(lambda x: x.replace('$',  '').replace(',','').strip())`
 - `.applymap(lambda x: x.replace('$',  '').replace(',','').strip())`
 - `.str.lower()`
 - `.str.replace('[^a-zA-Z0-9\-\']',  ' ', regex=True)`--> regex=True Expresión regular (palabra llave) que realiza una búsqueda personalizada y más específica en el texto.
 -->'[^a-zA-Z0-9\-\']´Estos son los caracteres que no (^) se van a modificar en el texto, todo lo demás sí.
 - `.str.replace('(?<!\w)-(?!\w)',  ' ', regex=True)`-->(?<!\w)-(?!\w) Estos caracteres indican que si hay caracteres antes o después de un guion no los modifique
 - `.str.replace('\{|}|\"','', regex=True)`
 - `.str.split(',')`-->Mediante el método split separa el string en una lista por cada palabra
 - `pd.to_datetime`
 - `.dt.strftime`-->El método strftime se utiliza para formatear objetos de fecha y hora en Python. En el caso de dt.strftime('%Y-%m'), dt es un objeto de tipo datetime
 - `.groupby`
 - `.fillna`-->utilizamos el método fillna para llenar los elementos vacíos por '0.0'
 - `inplace`-->definimos el parámetro de inplace para True para substituir en el DataFrame
 - `.dt.strftime('%Y-%m'))['precio'].sum()\`


## 📒 Glosario
### Columnas anidadas
Al importar archivos json se pueden encontrar columnas que no desplegadas debido a que en una columna se localizan estructuras del tipo "lista".

### Expresiones regulares
Las **expresiones regulares** en Python son patrones utilizados para buscar, comparar y manipular texto de manera flexible y eficiente. Son especialmente útiles para procesar cadenas, validar formatos y extraer información específica.
Las expresiones regulares permiten:
-   **Buscar y reemplazar** palabras o caracteres en un texto.
-   **Validar formatos**, como correos electrónicos, números de teléfono o contraseñas.
-   **Extraer datos** de textos complejos sin necesidad de recorrer cada carácter manualmente.

### Normalizar columnas
Es la acción de desplegar las listas anidadas mediante métodos y funciones como:
- **pd.json_normalize** -> solo despliega las listas de una columna.
- **.explode(columnas[:])** -> despliega más de una columna.

### Pricing inteligente
Es una estrategia para estimar precios de forma automatizada y dinámica, que considera factores como oferta y demanda, estacionalidad, eventos locales, características de ubicación, entre otros. Con base en esta información, un algoritmo puede ajustar los precios para maximizar los ingresos y la rentabilidad del propietario.

### Tockenizar
El proceso de dividir un texto en partes más pequeñas, llamadas "tokens". Estos tokens pueden ser palabras, frases o incluso caracteres, dependiendo del contexto. En el análisis de datos y procesamiento de lenguaje natural, la tokenización es fundamental para facilitar el análisis de texto

### Regex

## ✏️Artículos y contenido de interés
[Regex_Expresiones_Regulares](https://www.alura.com.br/artigos/principais-casos-uso-regex-para-tratamento-dados?_gl=1*1nnru91*_gcl_au*MTcwNTc2NjQ5Ny4xNzQzNjAwMjM3*_ga*NzU3MzMzMjc1LjE3NDM2MDAyMzY.*_ga_WWRP4FFDZK*czE3NDgwOTk5NzEkbzEyOCRnMSR0MTc0ODEwMjUxMCRqNjAkbDAkaDAkZHVPSzIteEdCY2p1blplTFdKdHhSSHVVYkRGZ3RyRDFqYXc.)
