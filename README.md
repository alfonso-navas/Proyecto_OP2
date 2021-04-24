# Proyecto_OP2
Proyecto OP2: Explorar indicadores que reflejen la incidencia de Covid-19 en Venezuela. 

## Instruciones para correr los notebooks:

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

Entra al repositorio y asegúrate estar en la rama "master" : 

```
cd Proyecto_OP2
git checkout master
```

Ahora instala las bibliotecas que usaremos con:

```
pip install -r requirements.txt
```

Usando ipykernel, creemos un kernel dedicado para este proyecto:

```
python3 -m ipykernel install --user --name=Proyecto_OP2
```
