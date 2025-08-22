# 🔬 Notebooks de Análisis para PIA-KRASv2-Nb

Bienvenido al repositorio de los **pipelines de análisis estructural** para el nanocuerpo **PIA-KRASv2-Nb** en complejo con el epítopo **KRAS Switch I**.

Este directorio contiene dos notebooks de Google Colab diseñados para diferentes propósitos de análisis y visualización.

---

## 1. Análisis de Interacciones del Complejo

Este notebook principal permite **caracterizar una pose estática** del complejo y es ideal para validar modelos obtenidos por AlphaFold, docking o cristalografía antes de pasar a simulaciones de MD.

**Funcionalidades:**
- 📏 **Contactos residuo–residuo (<4 Å)**
- 💧 **Área accesible al solvente (SASA)**
- 🔗 **Puentes de hidrógeno e interacciones polares**
- 🧩 **Comparación WT vs mutante (opcional)**

👉 **Abrir en Google Colab:**
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qyyJtn2fAQABQcl6zN6a3IkVf89yknDh?usp=sharing)

---

## 2. Visualización de Potencial Electrostático

Este segundo notebook está específicamente diseñado para **generar y visualizar el mapa de potencial electrostático** en la superficie del complejo. Es la herramienta perfecta para analizar la complementariedad de cargas en la interfaz.

**Funcionalidades:**
- ⚡ **Cálculo del potencial electrostático** con APBS.
- 🎨 **Generación de la figura 2D** que muestra las superficies de carga positiva (rojo) y negativa (azul).
- 🗺️ **Mapeo de residuos cargados** sobre el mapa de potencial.

👉 **Abrir en Google Colab:**
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VghJ-0wAsh_N895uYCMhDKcMBpYGW0uY)

👉 **Genera tu propio Notebook en Google Colab:**
Descarga el notebook desde la carpeta de interacciones del repositorio:
Electrostatic_pose.ipynb

Súbelo a tu Google Colab creando un notebook nuevo y seleccionando Archivo > Subir notebook....

Sube el archivo PDB (PIA_KRASv2Nb_renumbered.pdb) al entorno de Colab.

Ejecuta las celdas en orden.

---

## 📊 Contenido y Resultados

Ambos notebooks están documentados para guiarte a través del análisis. Los resultados esperados incluyen:
- Archivos PDB corregidos y estandarizados.
- Métricas cuantitativas de la interfaz (**SASA, contactos, electrostática**).
- Archivos CSV con los pares de residuos en contacto.
- Visualizaciones 3D interactivas y mapas 2D de alta calidad.

---

## 🧑‍🔬 Autor

**José Ignacio Peinador Sala** Investigador independiente – Plataforma PIA

📧 joseignacio.peinador@gmail.com  
🔗 [ORCID: 0009-0008-1822-3452](https://orcid.org/0009-0008-1822-3452)

---

⭐ Si estos notebooks te resultan útiles, ¡considera dejar una estrella en el repo!
