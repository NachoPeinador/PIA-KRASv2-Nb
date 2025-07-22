# 🧬 PIA-KRASv2-Nb: Nanobody de Alta Afinidad contra KRAS

![Licencia](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)
![ipTM](https://img.shields.io/badge/ipTM-0.78-blue)
![pTM](https://img.shields.io/badge/pTM-0.92-blue)

Este repositorio documenta el diseño y la validación *in silico* del nanobody **PIA-KRASv2-Nb**, una molécula terapéutica dirigida contra el epítopo accesible `DEYDPTIEDS` de la oncoproteína KRAS.

![Modelo 3D de PIA-KRASv2-Nb (Semilla 72)](./PIAvsKRAS_s72.png)

> 📌 *Modelo estructural generado con AlphaFold-Multimer v3 (semilla 72), que arrojó una puntuación de **ipTM = 0.78** y **pTM = 0.92**.*

---

## 🔍 Objetivo

Diseñar un **nanobody 100% humanizado, estable y específico** que reconozca un epítopo funcionalmente crítico de KRAS con alta afinidad, con el fin de proponerlo como un candidato viable para inmunoterapia y diagnóstico molecular.

---

## 🔧 Herramientas Utilizadas

- [AlphaFold-Multimer v3](https://alphafoldserver.com/)
- Herramientas del SAbPred server (Oxford Protein Informatics Group):
  - [Therapeutic Antibody Profiler (TAP)](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabpred/tap)
  - [ANARCI](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabpred/anarci)
  - [SCALOP](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabpred/scalop)
  - [NanoBodyBuilder2](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabpred/nanobodybuilder2)
  - [Hu-mAb (Humanization Classifier)](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabpred/humab)

---

## 📂 Contenido del Repositorio

- **`PIA_KRASv2-Nb_Report.pdf`**: Artículo científico completo con la descripción del método PIA, los resultados y la validación *in silico* detallada.
- **`AlphaFold_models/`**: Estructuras 3D en formato `.cif` de las semillas de élite (72, 13 y 10).
- **`LICENSE.md`**: Licencia detallada del proyecto.

---

## 📌 Secuencias Clave

### Nanobody PIA-KRASv2-Nb (FASTA)
```
>PIA-KRASv2-Nb_Original_Sequence
EVQLVESGGGLVQPGGSLRLSCAASGFTFSSYAMSWVRQAPGKGLEWVSSISSSSSYIYYADSVKGRFTISRDNSKNTLYLQMNSLRAEDTAVYYCARDYYYGMDVWGQGTTVTVSSDIQ
```

```
>KRAS_epitope_DEYDPTIEDS
DEYDPTIEDS
```

---

## 📈 Resultados Principales

| Parámetro                | Valor      | Herramienta                     |
| :----------------------- | :--------- | :------------------------------ |
| ipTM (Confianza Unión)   | **0.78** | AlphaFold-Multimer v3 (Seed 72) |
| pTM (Estructura Global)  | **0.92** | AlphaFold-Multimer v3           |
| Humanización (Familia)   | ✅ **1.0** | Hu-mAb (Familia Humana VH3)     |
| RMSD (Estabilidad CDR3)  | **0.19 Å** | NanoBodyBuilder2                |

---

## 🧪 Aplicaciones Propuestas

**Terapia Dirigida:** Inhibición directa y pan-mutante de la señalización de KRAS.

**Diagnóstico Molecular:** Desarrollo de biosensores epítopo-específicos de alta afinidad.

**Ingeniería de Proteínas:** Como base para formatos bivalentes o conjugados anticuerpo-fármaco (ADC).

---

## 🤝 Contacto y Colaboración
Este proyecto está abierto a la validación experimental. Si trabajas en inmunoterapia, biología estructural o ensayos celulares y tienes interés en colaborar en este proyecto, puedes contactar con el autor:

## [📧 Nacho Peinador](mailto:joseignacio.peinador@gmail.com)

---

## 📄 Licencia
Este proyecto está licenciado bajo la Creative Commons Attribution-NonCommercial 4.0 International.

Este trabajo ha sido registrado en el Registro de la Propiedad Intelectual de España para establecer una prueba fehaciente de autoría y fecha de creación. Por favor, consulta el archivo LICENSE.md para ver los términos completos, incluyendo las condiciones para licencias comerciales.
