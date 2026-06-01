# 📊 Dashboard Análisis Financiero | Power BI

https://app.powerbi.com/groups/me/reports/440bf669-5b07-4746-9d67-9a0677db6bcd/24113e6cc83b6d0220e9?redirectedFromSignup=1&experience=power-bi

---

## 📌 Descripción del Proyecto

Este proyecto presenta un **Dashboard de Análisis Financiero** desarrollado en Power BI para una empresa del rubro **tecnología de consumo masivo** (consumer tech), con dos líneas de negocio: **Dispositivos** (hardware) y **Digital** (software y servicios). El modelo abarca el período **2025–2027** con presencia comercial en 5 continentes.

El informe está diseñado con enfoque ejecutivo para facilitar la toma de decisiones basada en datos, permitiendo analizar rentabilidad, evolución temporal y desempeño por mercado geográfico.

---

## 🎯 Objetivos del Análisis

- Medir la evolución de ingresos, gastos y utilidad en el período 2025–2027.
- Comparar la rentabilidad entre categorías de producto (Dispositivos vs. Digital).
- Analizar el desempeño financiero por continente y país.
- Identificar tendencias trimestrales en márgenes e ingresos.
- Apoyar decisiones estratégicas de asignación de recursos por segmento.

---

## 📊 Indicadores Clave (KPIs)

| Indicador | Valor |
|---|---|
| Ingresos Totales (3 años) | $3.363.434.207 |
| Gastos Totales (3 años) | $2.692.324.708 |
| Utilidad Total (3 años) | $671.109.499 |
| Margen Neto Promedio | 19,95% |

---

## 📈 Visualizaciones Incluidas

- 📌 Tarjetas ejecutivas con KPIs principales (Ingresos, Gastos, Utilidad, Margen)
- 📌 Evolución anual de resultados financieros (2025–2027)
- 📌 Comparativa de rentabilidad por categoría de producto
- 📌 Distribución geográfica de ingresos y margen por continente
- 📌 Ranking de países por volumen de ingresos
- 📌 Evolución trimestral de ingresos y utilidad (12 trimestres)
- 📌 Filtros dinámicos por año, trimestre, categoría y región

---

## 🔎 Principales Hallazgos

📊 **Digital lidera en rentabilidad**: la categoría Digital alcanza un margen del **38,8%**, casi el triple que Dispositivos (13,9%), posicionándola como el segmento de mayor valor relativo.

🌎 **América y Europa destacan en eficiencia**: con márgenes del 22,5% y 22,0% respectivamente, superan el promedio global a pesar de no ser los mercados de mayor volumen.

🌏 **Asia es el mercado de mayor volumen** con $1.380M en ingresos, pero su margen (17,1%) está por debajo del promedio consolidado.

⚠️ **Oportunidad de mejora en Dispositivos**: la brecha de margen de 25 puntos porcentuales entre categorías sugiere revisar la estructura de costos del segmento hardware.

📅 **Estabilidad trimestral**: el margen neto se mantiene en torno al 20% durante todos los trimestres, con el pico de ingresos en 2027 T3 ($306M).

---

## 🧮 Medidas DAX Implementadas

```dax
Total Ingresos = SUM(Datos[Ingresos])

Total de Gastos = SUM(Datos[Gastos])

Utilidad = [Total Ingresos] - [Total de Gastos]

Margen = DIVIDE([Utilidad], [Total Ingresos], 0)
```

---

## 🗂 Modelo de Datos

El modelo está compuesto por **2 tablas de datos** y **1 tabla de medidas**:

- **`Datos`** — tabla de hechos con ingresos, gastos, dimensiones temporales (Año, Trimestre) y geográficas (Continente, País)
- **`Productos`** — tabla de dimensión con Tipo de Producto y Categoría de Producto
- **`Medidas`** — tabla dedicada a medidas DAX (buena práctica de modelado)

Relación: `Datos[Tipo Producto]` → `Productos[Tipo Producto]` (Muchos a uno)

---

## 🛠 Herramientas Utilizadas

- Power BI Desktop
- Power BI Service

---

🧩 Habilidades Aplicadas

- DAX (Data Analysis Expressions)
- Modelado de datos relacional
- Diseño de visualizaciones ejecutivas
- Storytelling con datos

---

## 🧠 Enfoque Analítico

El dashboard fue diseñado bajo principios de:

- Jerarquía visual clara
- Diseño moderno corporativo
- Uso estratégico de KPIs financieros
- Análisis descriptivo orientado a negocio
- Segmentación por producto y geografía

---

## 📂 Estructura del Proyecto

```
proyecto-datdata/
│
├── data/
│   └── dataset.csv
│
├── dashboard/
│   └── proyecto_datdata.pbix
│
├── images/
│   └── preview.png
│
└── README.md
```

---

## 📌 Aplicabilidad Empresarial

Este tipo de análisis es útil para:

- Gerencia General y Dirección Financiera
- Equipos de Estrategia y Planificación
- Analistas de Business Intelligence
- Product Managers de líneas de negocio
- Equipos Comerciales con cobertura internacional

---

## 👤 Autor

**Ruben Barrios**
Proyecto práctico desarrollado como parte de portafolio profesional en análisis de datos y Business Intelligence.
Fuente de los datos: Academia Datdata.

---

## ⭐ Si este proyecto te parece interesante

No olvides darle una estrella al repositorio y conectar en LinkedIn.

https://www.linkedin.com/in/ruben-barrios-1430712ab/

`#DataAnalytics` `#PowerBI` `#BusinessIntelligence` `#FinancialAnalysis` `#DAX` `#DataPortfolio` `#ConsumerTech` `#Datdata`
