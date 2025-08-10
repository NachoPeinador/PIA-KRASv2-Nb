# Simulación de Dinámica Molecular del Complejo PIA-KRASv2-Nb

Este notebook de Google Colab proporciona el código y el flujo de trabajo completo para realizar una simulación de dinámica molecular (DM) del complejo formado por el nanocuerpo **PIA-KRASv2-Nb** y el epítopo Switch I de la oncoproteína KRAS.

El notebook permite replicar la validación dinámica presentada en el artículo científico asociado, partiendo de un archivo de estructura `.cif` generado por AlphaFold 3.

---

### Abrir en Google Colab

Para abrir y ejecutar este notebook directamente en tu navegador, haz clic en el siguiente botón:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16FlafUaOaEpy7yyycTcx1F0liDf6xYOD?usp=sharing)

---

### Contenido y Flujo de Trabajo

El notebook está diseñado para ser ejecutado secuencialmente, celda por celda, y guía al usuario a través de los siguientes pasos cruciales:

1.  **Configuración del Entorno:**
    *   Instalación de todas las librerías necesarias, incluyendo `OpenMM` para la simulación y `MDTraj` para el análisis.
    *   **¡Importante!** Se debe seleccionar un entorno de ejecución con **aceleración por GPU** (Hardware accelerator: T4 GPU) para que la simulación se complete en un tiempo razonable.

2.  **Carga y Preparación de la Estructura:**
    *   Carga del archivo `.cif` del complejo predicho por AlphaFold 3.
    *   Conversión automática del archivo `.cif` a formato `.pdb` utilizando la librería BioPython.

3.  **Preparación del Sistema para la Simulación:**
    *   Adición de átomos de hidrógeno faltantes.
    *   Creación de una caja de simulación y solvatación con un modelo de agua explícito (TIP3P).
    *   Neutralización del sistema mediante la adición de iones (Na+/Cl-).

4.  **Ejecución de la Simulación de Dinámica Molecular:**
    *   **Minimización de energía** para relajar la estructura.
    *   **Equilibrado** del sistema a 300 K.
    *   **Simulación de producción** de 500 picosegundos para generar la trayectoria.

5.  **Análisis de Resultados:**
    *   Cálculo de la **Desviación Cuadrática Media (RMSD)** a lo largo del tiempo para evaluar la estabilidad del complejo.
    *   Generación de un gráfico de alta calidad que muestra el RMSD del nanocuerpo en relación con KRAS.

### Requisitos

*   Una cuenta de Google para poder ejecutar el notebook en Colab.
*   El archivo `.cif` de la estructura del complejo que se desea simular.
