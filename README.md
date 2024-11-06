# Práctica 1 - Tipología y Ciclo de Vida de los Datos

Asignatura: M2.851 / Semestre: 2024-1 / Fecha: 12-11-2024

[![Current Version](https://img.shields.io/badge/version-1.0-green.svg)](https://github.com/Kamaranis/Web-Scraping-de-videojuegos-con-potencial-de-revalorizacion)

## Autor
  * Anton Barrera Mora - [abarreramora@uoc.edu](abarreramora@uoc.edu)

## Sitio web elegido
[https://www.pricecharting.com](https://www.pricecharting.com)

## Enlace DOI Zenodo
El dataset ha sido publicado en Zenodo con DOI [10.5281/zenodo.14043146](https://doi.org/10.5281/zenodo.0000000).

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14043146.svg)](https://doi.org/10.5281/zenodo.14043146)

## Descripción del repositorio

Este repositorio contiene un script de Python para realizar web scraping de Pricecharting.com y obtener datos de precios de videojuegos de Xbox One y Xbox Series X.  El script extrae enlaces de videojuegos, descarga precios, genera archivos CSV y crea un dataset con información sobre ID, título, precios (loose, CIB, new) y plataforma.

Para ejecutar el script, se necesita Python 3.x y las siguientes librerías: requests-html, pandas.  Se recomienda crear un entorno virtual e instalar las dependencias con `pip install -r requirements.txt`.

### Estructura

  * `/source/main.py`: Script principal.
  * `/source/modulos/link_crawler.py`: Módulo para recopilar enlaces de plataformas de videojuegos.
  * `/souce/modulos/download.py`: Módulo para descargar enlaces de plataformas de videojuegos.
  * `/souce/modulos/download_pc.py`: Módulo para descargar precios de videojuegos.
  *  `/souce/modulos/procesar_datos.py`: Módulo para tratar los datos recopilados en diferentes formas.
  * `/source/requirements.txt`: Lista de paquetes utilizados (Python 3.12.4).

## Instrucciones

### Instalación

Para instalar las dependencias del proyecto, ejecute:

```bash
pip install -r requirements.txt
```

### Ejecución
```
python main.py
```

## Tecnologías Utilizadas

- **Python**: Lenguaje de programación principal.
- **Pandas**: Biblioteca de Python para manipulación y análisis de datos.
- **requests_html**: Biblioteca de uso simplificado para la realización de *Web Scraping*