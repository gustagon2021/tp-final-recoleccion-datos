# Trabajo Práctico Final - Recolección de Datos y Análisis Primario (181)
### 📊 UNAB - Licenciatura en Ciencia de Datos
**Profesora:** Rosana Benavidez  
**Integrantes:** Gustavo y grupo  

---

## 🚀 Guía de Inicio Rápido para el Equipo

Para que todos podamos ejecutar el código de R Markdown (.Rmd) y generar el informe interactivo (.html) sin problemas de compatibilidad ni errores de rutas, sigamos estos pasos:

### 1. Requisito Fundamental: Estructura de Carpetas
Para evitar los errores clásicos de "ruta no encontrada", este proyecto está configurado con **rutas relativas**. 

* **¿Qué significa?** Que R buscará el archivo de datos directamente en el mismo lugar donde está guardado el script.
* **¿Qué hay que hacer?** Descargá el archivo de código (.Rmd) y la base de datos (Películas_data.csv) y guardalos **juntos dentro de una misma carpeta** (en cualquier parte de tu computadora).

### 2. Instalación de Librerías Necesarias
Antes de correr los bloques de código por primera vez, necesitamos asegurarnos de tener instalados los paquetes de R que usamos para el preprocesamiento y los gráficos. 

Copiá y ejecutá la siguiente línea en la **Consola** de tu RStudio:

install.packages(c("tidyverse", "lubridate", "scales"))

* *Nota: "tidyverse" ya incluye internamente las herramientas clave que usamos en el TP como ggplot2, dplyr, tidyr y readr.*

---

## 🛠️ Estructura del Código (.Rmd)

El script de R Markdown está organizado de manera secuencial en **6 bloques funcionales**:

1. **Bloque 1: Carga de datos:** Lee de manera eficiente el archivo Películas_data.csv y muestra una radiografía inicial del dataset crudo.
2. **Bloque 2: Limpieza y Pivoteo:** Aplica ingeniería de datos para transformar la estructura de formato largo a formato ancho (separando las métricas en columnas independientes de Recaudacion y Entradas) y repara el parseo heterogéneo de las fechas de estreno usando lubridate.
3. **Bloque 3: Análisis de Consistencia:** Verifica automáticamente la presencia de registros duplicados o valores nulos (NA). *Resultado de nuestra base: 0 nulos, 0 duplicados.*
4. **Bloque 4: Estadísticos Descriptivos:** Rompe la notación científica de R y calcula las métricas generales (mínimo, máximo, media y mediana) agrupadas según el origen de la producción cinematográfica.
5. **Bloque 5: Visualización con ggplot2:** Genera un diagrama de caja (Boxplot) en escala logarítmica para evaluar la distribución de ingresos y un gráfico de dispersión (Scatterplot) para mapear la relación entre volumen de espectadores y recaudación total.
6. **Bloque 6: Dimensión Temporal:** Evalúa la estacionalidad de la taquilla agrupando la recaudación mes a mes durante el ciclo 2026.

---

## 📦 Cómo Compilar y Entregar el Informe

Para dar cumplimiento estricto a las pautas solicitadas por la cátedra (presentar un documento estético y **ocultar las líneas de código técnico** en la lectura final), el encabezado del archivo está configurado con parámetros automatizados de knitr.

1. Abrí el archivo del TP en tu RStudio.
2. En la barra de herramientas superior, hacé clic en el botón del **gato tejiendo (Knit)** o usá el atajo de teclado Ctrl + Shift + K.
3. R procesará todos los bloques de código en limpio y exportará un archivo interactivo llamado **nombre_del_archivo.html**.
4. Al abrirlo, verás que el diseño cuenta con un menú flotante de navegación a la izquierda (toc_float) y el código oculto bajo botones desplegables, cumpliendo al 100% el requerimiento de evaluación.

---
*Cualquier duda o error que les surja al compilar, lo tiramos por el grupo de WhatsApp para corregir el chunk correspondiente.* 🎬
