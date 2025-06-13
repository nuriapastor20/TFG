# 📊 Visualización de donativos mediante Qlik Sense – TFG de Nuria Min Pastor Pedrós

Este repositorio contiene el código fuente del proyecto desarrollado como Trabajo de Fin de Grado en Ciencia de Datos por **Nuria Min Pastor Pedrós** (UPV), titulado:

**“Visualización mediante Qlik Sense de donativos realizados por clientes y gestionados por una entidad financiera: proceso de modelado de datos”**

## 🧩 Objetivo del proyecto

Diseñar y desarrollar una solución completa de Business Intelligence para representar los donativos gestionados por una entidad financiera a través de un **cuadro de mando interactivo** en **Qlik Sense**.  
El proyecto incluye:
- Extracción y tratamiento de datos desde bases internas.
- Generación de archivos QVD optimizados.
- Modelado de datos en estrella.
- Construcción de un dashboard dinámico con KPIs, filtros, mapas y análisis detallado por causas, canales y clientes.

## 🗂 Estructura del repositorio
```
├── Extractor_Donativos/
│ ├── Extractor 1. Definición de parámetros globales
│ ├── Extractor 2. Mappings
│ ├── Extractor 3. Tablas Maestras
│ ├── Extractor 4. Tabla Donativos Bizum
│ ├── Extractor 5. Tabla Causas
│ ├── Extractor 6. Tabla Principal Donaciones
│ ├── Extractor 7. Tabla Tipos de Negocio
│ ├── Extractor 10. Calendario
│ 
├── Cuadro_de_Mando_Donativos/
│ ├── CdM 1. Configuración General
│ ├── CdM 2. Carga General
│ ├── CdM 3. Tabla Donaciones
│ ├── CdM 4. Calendario
│ ├── CdM 5. Selector
│ 
├── README.md # Este documento
```

## 💻 Scripts disponibles

`Extractor` (scripts del proceso de generación de QVDs):
Los archivos cuyo nombre comienza por Extractor contienen el proceso completo de obtención, transformación y modelado de datos. En particular:

- Extractor 1. Definición de parámetros globales, Extractor 2. Mappings, y los siguientes hasta el Extractor 10, comprenden la carga de las 19 tablas utilizadas en el modelo.
Estos scripts aplican transformaciones como ApplyMap, AutoNumber, Resident Load, renombrado de campos y control de claves sintéticas. Cada archivo está orientado a una parte concreta del flujo de datos (por ejemplo, tablas maestras, donativos Bizum, calendario, causas, etc.).

`CdM` (scripts del cuadro de mando):
Los archivos que comienzan por CdM contienen el desarrollo del cuadro de mando en Qlik Sense.

Estos scripts se encargan de la carga de QVDs generados previamente, la creación de campos derivados, la definición de relaciones entre hechos y dimensiones y la preparación de los datos para su visualización final en el dashboard.

## 🔗 Relación con la memoria

En la memoria del TFG (capítulo 4.4 "Implementación") se describe el procedimiento general seguido en este repositorio.  
Para evitar redundancias, se han incluido en el documento únicamente dos ejemplos representativos, y se remite a este repositorio para consultar el código completo.

## 📝 Licencia

Este código se publica únicamente con fines académicos y demostrativos. No contiene datos reales de clientes ni conexiones activas a bases internas.
