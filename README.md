# Analítica de Incidentes Viales CDMX (C4/C5)

* **Nombre del Equipo:** Las Galácticas
* **Integrantes:** 
  * Zambrano Osorno Sarai
  * Díaz Dorado Rosa Isela
* **Nombre del Proyecto:** Analítica de Incidentes Viales CDMX (C4/C5)
* **Materia:** Inteligencia de Negocios — UACM Plantel San Lorenzo Tezonco
* **Profesora:** Araceli Liliana Reyes Cabello

---

## 📌 Breve Descripción
Proyecto de BI que analiza los incidentes viales reportados al C5 de la CDMX (2017-2019) para identificar las alcaldías, días y franjas horarias con mayor concentración de incidentes, así como los tipos más frecuentes. Es un diagnóstico inicial que sirve como antecedente para la planeación preventiva y la asignación de recursos de emergencia.

---

## 🗃️ Fuente Principal de Datos
- **Dataset:** Mexico Road Accidents during 2017-2019, de Eduardo Romero (Kaggle). Descargado el 04/10/2026.
- **Archivos:** `incidentes-viales-c5-2017.csv`, `incidentes-viales-c5-2018.csv`, `incidentes-viales-c5-2019.csv`
- **Diccionario de datos:** Incidentes viales reportados al C5 (Datos Abiertos CDMX).
- **Licencia:** Open Data / CC BY-SA 4.0
---

## 📁 Organización General del Repositorio
- `docs/`: informes de los avances en PDF (`avance01.pdf`, `avance02.pdf`, `avance03.pdf`).
- `data/raw/`: datos crudos o instrucciones de descarga. No se modifican.
- `data/processed/`: salidas del ETL (`incidentes_preparados.csv`, `incidentes_pendientes.csv`, `controles.csv`, `resumen_alcaldia_dia_franja.csv`).
- `notebooks/`: notebooks de cada avance (`avance02.ipynb`, `avance03.ipynb`).
- `bitacora/`: `bitacora.csv` (generada automáticamente por el ETL) y la bitácora del equipo.
- `presentacion/`: exposición en PDF.

## ▶️ Cómo ejecutar el proyecto
**Antes de empezar:** descargar los 3 CSV de Kaggle y guardarlos en Google Drive, en `MyDrive/BI S&R/Datos/Kaggle/`.

| Avance | Contenido | Archivo | Cómo se ejecuta |
|---|---|---|---|
| Avance 1 | Problema, datos y plan analítico | `docs/avance01.pdf` | No tiene código |
| Avance 2 | Lectura, perfilamiento, limpieza y validación | `notebooks/avance02.ipynb` | Abrir en Colab y usar Ejecutar todo |
| Avance 3 | Integración, ETL reproducible, bitácora y estadística | `notebooks/avance03.ipynb` | Abrir en Colab y usar Ejecutar todo |

Cada notebook se ejecuta de arriba hacia abajo, sin cambios manuales.

## 📤 Salidas
Al terminar, el notebook genera en Drive (`MyDrive/BI S&R/`):
- `data/processed/`: datos preparados (680,687), pendientes (59), controles y resumen.
- `bitacora/bitacora.csv`: registro automático de los 16 pasos del proceso.
