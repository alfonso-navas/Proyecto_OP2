~~~
LA-CoNGA physics
¡SUENA BIEN!
~~~

# Exploración de indicadores que reflejen la incidencia de COVID-19 en Venezuela usando fuentes de datos no oficiales

### Autores
Alfonso Navas. Universidad Nacional de Colombia. 

Eliana Bonalde. Universidad Industrial de Santander. 

### Supervisión
Camila Rangel Smith. GitHub: @crangelsmith. 

### Colaboración
Harvey Maddocks. gitHub: @HarveyMaddocks.

___

## Resumen

El objetivo principal de este trabajo es hacer una comparación mediante series de tiempo, correspondientes al periodo comprendido entre marzo de 2020 y mayo de 2021, entre datos numéricos oficiales del virus COVID-19 en Venezuela y datos no oficiales extraídos de las plataformas de GoFundMe, Twitter y Google Trends. Tomaremos como datos oficiales los estimados por el modelo del Instituto de Métricas y Evaluación de la Salud (IHME, por sus siglas en inglés), ya que según estimaciones de organizaciones nacionales e internacionales las cifras oficiales reportadas por el gobierno de Venezuela no corresponden a la realidad. Por medio del análisis de los datos extraídos, se muestran los mejores indicadores que refeljan la incidencia de Covid-19 en Venezuela. Python es el lenguaje de programación utilizado para extraer, almacenar, visualizar y analizar estos resultados, los cuales van a permitir tener una idea de la realidad que se está viviendo en Venezuela con respecto al virus.


## Notebooks

Se recomienda ejecutar los Notebooks en el siguiente orden.
 
- [IHME](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/IHME.ipynb) Exploración de las series de tiempo de los casos estimados por el IHME.
- [GoFundMe - Tratamiento ético de los datos](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/GoFundMe_datos.ipynb) tratamiento de los datos extraídos de la campañas de GoFundMe.
- [GoFundMe - Análisis exploratorio](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/GoFoundMe_analisis.ipynb) Exploración de los datos obtenidos mediante web scrapping de GoFundMe.
- [Twitter - Extracción de datos](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/Twitter_datos.ipynb) Extracción de los datos de Twitter por medio de la API de Twitter por medio de la biblioteca `twarc`.
- [Twitter - Análisis de los datos extraídos](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/Twitter_analisis.ipynb) Análisis y construcción de las series de tiempo de los datos extraídos de Twitter.
- [Google Trend - Datos y análisis](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/GoogleTrends_datos.ipynb) Extracción y análisis de los datos de Google Trends por medio de `pytrends`.
- [Análisis general](https://github.com/bonaldee/Proyecto_OP2/blob/main/codigo/analisis_general.ipynb) Comparación de las series de tiempo de los casos estimados por el IHME, y los datos extraídos de GoFundMe, Google y Twitter.



## Instruciones para correr los notebooks

Este repositorio requiere tener instalado [conda](https://docs.conda.io/projects/conda/en/latest/index.html) y una version de Python 3.7 o mayor. 

Empecemos creando un nuevo entorno computacional conda de la forma:

```
conda create -n Proyecto_OP2 python=3.7
conda activate Proyecto_OP2
```

Ahora descarga este repositorio:

```
git clone https://github.com/bonaldee/Proyecto_OP2.git
```

Entra al repositorio y asegúrate estar en la rama "main" : 

```
cd Proyecto_OP2
git checkout main
```

Ahora instala las bibliotecas que usaremos con:

```
pip install -r requirements.txt
```

Usando ipykernel, creemos un kernel dedicado para este proyecto:

```
python3 -m ipykernel install --user --name=Proyecto_OP2



