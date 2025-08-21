# 🧬 Pipeline de Simulación y Análisis MD para PIA-KRASv2-Nb

Bienvenido al repositorio del pipeline computacional completo para la validación del nanocuerpo **PIA-KRASv2-Nb**. Este proyecto proporciona dos notebooks de Google Colab interconectados que permiten llevar una estructura estática (generada por AlphaFold) a través de una simulación de dinámica molecular (MD) y un análisis cuantitativo detallado.

👉 El objetivo es ofrecer una metodología *in silico* robusta y reproducible para evaluar la estabilidad de complejos proteína-proteína antes de la validación experimental.

---

## 🚀 Abrir directamente en Google Colab

Haz clic en los botones para ejecutar los notebooks de inmediato en un entorno Colab. Deben ejecutarse en orden: primero la simulación, y luego el análisis con los archivos generados.

**Paso 1: Simulación de Dinámica Molecular**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1W2FtbyPI9uDkZCDqqdFkd6nVQfMoj_Kj?usp=sharing)

**Paso 2: Análisis de la Trayectoria**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Aue7oYHIFAmSe5xPwzyUB-HXJ6NgqNVb?usp=sharing)

---

## 📂 Contenido de los Notebooks

### 1. ⚛️ Notebook de Simulación (MD_SIMULATION.ipynb)
Este cuaderno prepara y ejecuta una simulación de dinámica molecular de 10 nanosegundos del complejo proteico usando OpenMM.

* **Instalación y Preparación:** Instala todas las dependencias (OpenMM, PDBFixer, etc.) y prepara el sistema añadiendo solvente (agua), iones y aplicando el campo de fuerza Amber14.
* **Ejecución de la Simulación:** Realiza la minimización de energía, el equilibrado y la simulación de producción.
* **Resultados Generados:** Produce los dos archivos esenciales para el análisis: `protein_system_CORRECTED.pdb` (topología) y `trajectory.dcd` (trayectoria).

### 2. 🧪 Notebook de Análisis (MD_ANALYSIS.ipynb)
Este cuaderno toma los resultados de la simulación y realiza un análisis cuantitativo de la estabilidad del complejo usando MDTraj.

* **Carga de Datos:** Permite subir los archivos `pdb` y `dcd` generados en el paso anterior.
* **Análisis de Estabilidad (RMSD):** Calcula y grafica el Desplazamiento Cuadrático Medio del armazón y de los CDRs para evaluar la estabilidad conformacional.
* **Análisis de Interfaz (Contactos):** Cuantifica el número de pares de residuos en contacto (<4 Å) entre el nanocuerpo y KRAS a lo largo del tiempo.
* **Análisis Estadístico:** Aplica una regresión lineal para determinar si la tendencia en los contactos de la interfaz es estadísticamente significativa (p-valor).

---

## 📊 Resultados Esperados del Pipeline Completo

* **Archivos de Trayectoria:** Un archivo `trajectory.dcd` de 10 ns.
* **Datos Cuantitativos:** Archivos `.csv` con los valores de RMSD y número de contactos por cada fotograma de la simulación.
* **Gráficos para Publicación:** Gráficos de alta calidad mostrando la evolución del RMSD y de los contactos en la interfaz.
* **Validación Estadística:** Un análisis claro (pendiente, p-valor, R²) que valida la robustez de la interacción proteína-proteína.

---

## 🧑‍🔬 Autor
**José Ignacio Peinador Sala** Investigador Independiente – Plataforma PIA

📧 joseignacio.peinador@gmail.com  
🔗 ORCID: 0009-0008-1822-3452

---

⭐ Si este pipeline te resulta útil, ¡considera dejar una estrella en el repo!
