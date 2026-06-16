#  Taller No. 3 – Análisis Estadístico Descriptivo y Visualización de Datos

**Universidad del Pacífico · Programa de Ingeniería de Sistemas**  
**Asignatura:** Inteligencia Artificial · **Semestre:** 8 – Corte II

---

##  Objetivo General

Aplicar técnicas de análisis estadístico descriptivo para transformar datos reales sobre descargas de aplicaciones móviles en información útil que apoye la toma de decisiones, utilizando herramientas computacionales para la representación gráfica e interpretación de patrones.

---

## 📌 Objetivos Específicos

- Identificar población, muestra, unidad de análisis y tipo de variable del conjunto de datos.
- Construir una tabla de distribución de frecuencias completa (fi, hi, Fi, Hi) a partir de la variable **Apps Descargadas**.
- Representar la distribución mediante histograma, polígono de frecuencias y ojiva acumulada.
- Interpretar cuantitativamente los resultados con pensamiento crítico y argumentación técnica.
- Elaborar un informe técnico con redacción formal, figuras numeradas y referencias bibliográficas.

---

## 📂 Archivos del Proyecto

| Archivo | Descripción |
|---|---|
| `Informe_Tecnico_Taller3_Apps_Descargadas.pdf` | Informe técnico completo (entregable principal) |
| `POBLACION.docx` | Datos e interpretaciones previas de los intervalos |
| `Taller_analisis_estadistico_frecuencia_graficos.pdf` | Enunciado oficial del taller |
| `README_Taller3.md` | Este archivo de documentación |

---

##  Metodología Aplicada

### 1. Datos del Conjunto
- **n = 50** usuarios de aplicaciones móviles (México, Colombia, Argentina, Chile, Perú)
- **Variable:** Apps Descargadas (cuantitativa discreta)
- **Mínimo:** 30 apps · **Máximo:** 132 apps · **Rango:** 102 apps

### 2. Construcción de Intervalos – Regla de Sturges
```
k = 1 + 3,322 × log₁₀(n) = 1 + 3,322 × log₁₀(50) ≈ 6,64 → k = 7 intervalos
Amplitud (c) = ⌈Rango / k⌉ = ⌈102 / 7⌉ = 15 apps por clase
```

### 3. Tabla de Frecuencias Resultante

| Intervalo | Marca (xᵢ) | fi | hi | hi (%) | Fi | Hi (%) |
|---|---|---|---|---|---|---|
| [30 – 45) | 37,5 | 7 | 0,1400 | 14,00% | 7 | 14,00% |
| [45 – 60) | 52,5 | 6 | 0,1200 | 12,00% | 13 | 26,00% |
| [60 – 75) ★ | 67,5 | **10** | 0,2000 | **20,00%** | 23 | 46,00% |
| [75 – 90) | 82,5 | 9 | 0,1800 | 18,00% | 32 | 64,00% |
| [90 – 105) | 97,5 | 8 | 0,1600 | 16,00% | 40 | 80,00% |
| [105 – 120) | 112,5 | 5 | 0,1000 | 10,00% | 45 | 90,00% |
| [120 – 135] | 127,5 | 5 | 0,1000 | 10,00% | 50 | 100,00% |
| **TOTAL** | | **50** | **1,0000** | **100%** | | |

>  Clase modal

---

## 📈 Gráficos Generados

1. **Histograma de Frecuencias** – muestra la forma de la distribución y la clase modal.
2. **Polígono de Frecuencias** – conecta las marcas de clase revelando la asimetría positiva.
3. **Ojiva Acumulada** – permite leer percentiles directamente; señala el P50 (~82 apps) y el P80 (~105 apps).

---

##  Hallazgos Principales

| Indicador | Resultado |
|---|---|
| Clase modal | [60 – 75) con fi = 10 (20%) |
| Tipo de distribución | Asimétrica positiva (sesgo derecho) |
| Mediana estimada | ~82 apps (intervalo [75–90)) |
| 80% de usuarios | Descargaron < 105 apps |
| "Power users" (>105 apps) | 20% de la muestra |

---

## 📚 Referencias

- Devore, J. L. (2016). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Cengage Learning.
- Walpole, R. E., Myers, R. H., & Myers, S. L. (2012). *Probabilidad y estadística para ingeniería y ciencias* (9.ª ed.). Pearson.
- Sturges, H. A. (1926). The choice of a class interval. *Journal of the American Statistical Association*, 21(153), 65–66.
- Montgomery, D. C., & Runger, G. C. (2018). *Probabilidad y estadística aplicadas a la ingeniería* (3.ª ed.). Limusa Wiley.

---

