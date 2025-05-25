# Pandas: Manipulación y transformación de datos
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
-  convertir la columna precio a datos numéricos a
-  agrupar los precios respecto a las fechas para determinar en qué fecha hubo más demanda


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
