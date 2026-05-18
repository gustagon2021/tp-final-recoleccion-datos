# Trabajo Práctico Final - Recolección de Datos y Análisis Primario (181)
### 📊 UNAB - Licenciatura en Ciencia de Datos
**Profesora:** Rosana Benavidez  
**Integrantes:** Gustavo y grupo  

---

## 🚀 Guía de Inicio Rápido para el Equipo

Para que todos podamos ejecutar el código de R Markdown (`.Rmd`) y generar el informe interactivo (`.html`) sin problemas de compatibilidad ni errores de rutas, sigamos estos pasos:

### 1. Requisito Fundamental: Estructura de Carpetas
Para evitar los errores clásicos de "ruta no encontrada", este proyecto está configurado con **rutas relativas**. 

* **¿Qué significa?** Que R buscará el archivo de datos directamente en el mismo lugar donde está guardado el script.
* **¿Qué hay que hacer?** Descargá el archivo de código (`.Rmd`) y la base de datos (`Películas_data.csv`) y guardalos **juntos dentro de una misma carpeta** (en cualquier parte de tu computadora).

### 2. Instalación de Librerías Necesarias
Antes de correr los bloques de código por primera vez, necesitamos asegurarnos de tener instalados los paquetes de R que usamos para el preprocesamiento y los gráficos. 

Copiá y ejecutá la siguiente línea en la **Consola** de tu RStudio:

```r
install.packages(c("tidyverse", "lubridate", "scales"))
