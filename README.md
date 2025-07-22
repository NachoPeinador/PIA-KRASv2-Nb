# 🧬 PIA-KRASv2-Nb: Nanobody de Alta Afinidad contra KRAS

Este repositorio documenta el diseño y validación in silico del nanobody PIA-KRASv2-Nb, una molécula terapéutica dirigida contra el epítopo accesible `DEYDPTIEDS` de la proteína KRAS. Combina herramientas estructurales, predicciones de inmunogenicidad y análisis biofísicos para justificar su potencial en inmunoterapia y diagnóstico molecular.

![Modelo 3D PIA-KRASv2Nb](/PIAvsKRAS_s72.png)

> 📌 *La imagen anterior corresponde al modelo estructural más confiable generado con AlphaFold-Multimer v3 utilizando la semilla 72, que arrojó una puntuación de ipTM = 0.78 y pTM = 0.92.*

---

## 🔍 Objetivo

Diseñar un **nanobody humanizado, estable y específico** que reconozca un epítopo lineal de KRAS con alta afinidad y potencial uso terapéutico en cánceres KRAS-dependientes.

---

## 🔧 Herramientas utilizadas

- [AlphaFold-Multimer v3](https://alphafold.ebi.ac.uk/)
- [Therapeutic Antibody Profiler (TAP)](https://opig.stats.ox.ac.uk/webapps/profiler)
- [ANARCI](https://opig.stats.ox.ac.uk/webapps/anarci/)
- [SCALOP](https://opig.stats.ox.ac.uk/webapps/scalop)
- [NanoBodyBuilder2](https://opig.stats.ox.ac.uk/webapps/nanobodybuilder2)
- [Hu-mAb (Humanization Classifier)](https://opig.stats.ox.ac.uk/webapps/humab)

---

## 📎 Documentación incluida

- `PIA_KRASv2Nb.txt`: Documento LaTeX con descripción científica completa
- `Apéndice_validación.txt`: Validaciones in silico detalladas
- `AlphaFold_models/`: Estructuras 3D en formato `.pdb`
- `Data_analysis/`: Scripts para evaluación estructural y análisis de unión

---

## 📌 Secuencias

### Nanobody PIA-KRASv2Nb (FASTA)

```fasta
>PIA-KRASv2Nb
EVQLVESGGGLVQPGGSLRLSCAASGFTFSSYAMSWVRQAPGKGLEWVSSISSSSSYIYY
ADSVKGRFTISRDNSKNTLYLQMNSLRAEDTAVYYCARDYYYGMDVWGQGTTVTVSSDIQ
```

### Epítopo objetivo (KRAS)

```fasta
>KRAS_epitope_DEYDPTIEDS
DEYDPTIEDS
```

---

## 📈 Resultados clave

| Parámetro                | Valor   | Herramienta              |
|--------------------------|---------|---------------------------|
| ipTM (confianza unión)   | **0.78** | AlphaFold-Multimer v3 (Seed 72) |
| pTM (estructura global)  | **0.92** | AlphaFold-Multimer v3     |
| Humanización (VH3)       | ✅ 1.000 | Hu-mAb                    |
| RMSD (estabilidad CDRs)  | 0.19 Å  | NanoBodyBuilder2          |

---

## 🧪 Aplicaciones propuestas

- Inhibición directa de KRAS (terapia dirigida)
- Formatos multivalentes o conjugados para diagnóstico
- Biosensores epítopo-específicos

---

## 🤝 Contacto y colaboración

Este proyecto está abierto a validaciones experimentales. Si trabajas en inmunoterapia, biología estructural o ensayos in vitro y te interesa colaborar:

📧 nachopeinador [at] protonmail.com  
🔗 [LinkedIn](https://linkedin.com/in/nachopeinador)

---

## 📄 Licencia

Este proyecto está licenciado bajo [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).
