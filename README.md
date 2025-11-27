# Análisis de Datos - Trabajo Práctico

## Descripción

Este repositorio contiene el trabajo práctico grupal de la materia Análisis de Datos. El proyecto consiste en el análisis exploratorio de datos de pesca correspondientes al año 2024, incluyendo visualizaciones, análisis estadísticos y exploración de patrones en los datos.

## Estructura del Proyecto

```
analisis_datos/
├── README.md
├── Análisis de datos - Trabajo grupal - B52025.pdf
└── tp/
    ├── tp.ipynb                    # Notebook principal con el análisis
    └── dataset/
        └── Crimes_-_2024_20251103.csv  # Dataset de pesca 2024
```

## Contenido

- **tp/tp.ipynb**: Notebook de Jupyter que contiene todo el análisis exploratorio de datos, incluyendo:
  - Importación y carga de datos
  - Análisis preliminar y exploración de variables
  - Análisis de valores faltantes
  - Visualizaciones (histogramas, boxplots, heatmaps, etc.)
  - Análisis estadísticos descriptivos
  - Análisis por categorías (provincia, especie, flota, puerto)

- **tp/dataset/**: Carpeta que contiene el dataset utilizado para el análisis

Dataset: Crimes_-_2024_20251103.csv

| Column Name | Description | API Field Name | Data Type |
| -------- | ------- | ------- | ------- |
| ID | Unique identifier for the record. | id | Number |
| Case Number | The Chicago Police Department RD Number (Records Division Number), which is unique to the incident. | case_number | Text |
| Date | Date when the incident occurred. this is sometimes a best estimate. | date | Floating Timestamp |
| Block | The partially redacted address where the incident occurred, placing it on the same block as the actual address. | block | Text |
| IUCR | The Illinois Uniform Crime Reporting code. This is directly linked to the Primary Type and Description. See the list of IUCR codes at https://data.cityofchicago.org/d/c7ck-438e. | iucr | Text |
| Primary Type | The primary description of the IUCR code. | primary_type | Text |
| Description | The secondary description of the IUCR code, a subcategory of the primary description. | description | Text |
| Location Description | Description of the location where the incident occurred. | location_description | Text |
| Arrest | Indicates whether an arrest was made. | arrest | Checkbox |
| Domestic | Indicates whether the incident was domestic-related as defined by the Illinois Domestic Violence Act. | domestic | Checkbox |
| Beat | Indicates the beat where the incident occurred. A beat is the smallest police geographic area – each beat has a dedicated police beat car. Three to five beats make up a police sector, and three sectors make up a police district. The Chicago Police Department has 22 police districts. See the beats at https://data.cityofchicago.org/d/aerh-rz74. | beat | Text |
| District | Indicates the police district where the incident occurred. See the districts at https://data.cityofchicago.org/d/fthy-xz3r. | district | Text |
| Ward | The ward (City Council district) where the incident occurred. See the wards at https://data.cityofchicago.org/d/sp34-6z76. | ward | Number |
| Community Area | Indicates the community area where the incident occurred. Chicago has 77 community areas. See the community areas at https://data.cityofchicago.org/d/cauq-8yn6. | community_area | Text |
| FBI Code | Indicates the crime classification as outlined in the FBI's National Incident-Based Reporting System (NIBRS).See the Chicago Police Department listing of these classifications at https://gis.chicagopolice.org/pages/crime_details. | fbi_code | Text |
| X Coordinate | The x coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block. | x_coordinate | Number |
| Y Coordinate | The y coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block. | y_coordinate | Number |
| Year | Year the incident occurred. | year | Number |
| Updated On | Date and time the record was last updated. | updated_on | Floating Timestamp |
| Latitude | The latitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block. | latitude | Number |
| Longitude | The longitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block. | longitude | Number |
| Location | The location where the incident occurred in a format that allows for creation of maps and other geographic operations on this data portal. This location is shifted from the actual location for partial redaction but falls on the same block. | location | Point |

- **Análisis de datos - Trabajo grupal - B52025.pdf**: Documento con las consignas del trabajo práctico

## Integrantes del Grupo

- Martín Amagliani
- Tomás Frechou
- Franco Curcho
- Cristian Aballay


## Requisitos

- Python 3.x
- Jupyter Notebook

## Uso

1. Clonar o descargar el repositorio
2. Asegurarse de tener instaladas las dependencias necesarias
3. Abrir el notebook `tp/tp.ipynb` en Jupyter Notebook o JupyterLab
4. Ejecutar las celdas en orden

