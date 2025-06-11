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

├── Extractor_Donativos/
│ ├── script_extractor.qvs # Script de carga y transformación (QVDs)
│ ├── ApplyMap_CANAL.qvs # Mapa de equivalencias canal
│ ├── ApplyMap_CAUSA.qvs # Mapa de equivalencias causa
│ └── ...
├── Cuadro_Donativos/
│ ├── script_cuadro.qvs # Script del dashboard (carga QVDs y visualización)
│ └── ...
├── README.md # Este documento


## 💻 Scripts disponibles

- `Extractor_Donativos/script_extractor.qvs`:  
  Contiene la carga completa de las 19 tablas utilizadas en el modelo, aplicando transformaciones como `ApplyMap`, `AutoNumber`, `Resident Load`, renombrado de campos y control de claves sintéticas.

- `Cuadro_Donativos/script_cdm.qvs`:  
  Script del cuadro de mando, con carga de QVDs, creación de campos derivados, relaciones lógicas entre hechos y dimensiones y preparación para visualización.

## 🔗 Relación con la memoria

En la memoria del TFG (capítulo 4.4 "Implementación") se describe el procedimiento general seguido en este repositorio.  
Para evitar redundancias, se han incluido en el documento únicamente dos ejemplos representativos, y se remite a este repositorio para consultar el código completo.

## 📝 Licencia

Este código se publica únicamente con fines académicos y demostrativos. No contiene datos reales de clientes ni conexiones activas a bases internas.
