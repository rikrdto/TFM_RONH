
# 📘 **README — Análisis Econométrico del Transporte Intermodal en la UE**

### **Trabajo Fin de Máster (TFM) – Universidad de Málaga**  
**Autor:** Ricardo Olmedo Naranjo  
📩 **Contacto:** rikrdonhojas@gmail.com  
**Año:** 2025  
**Lenguaje:** R  
**Tipo de análisis:** Modelos de datos de panel (FE two–ways)

---

## 📌 **Descripción del proyecto**

Este repositorio contiene el **código en R, datos, gráficos y resultados** utilizados en el Trabajo Fin de Máster titulado:

**“Análisis de la evolución del transporte intermodal ferroviario de contenedores en la Unión Europea y su relación con el desempeño económico.”**

El objetivo principal del proyecto es estudiar el efecto de la **intensidad intermodal ferroviaria** sobre el **PIB per cápita en PPA**, utilizando:

- Modelos de datos de panel  
- Efectos fijos dos vías (FE two-ways)  
- Pruebas de especificación  
- Diagnósticos de autocorrelación y heterocedasticidad  
- Gráficos descriptivos y gráficos interpretativos del modelo  

El repositorio incluye código completamente reproducible para replicar el análisis desde cero.

---

## 📂 **Estructura del repositorio**

```
TFM_RONH/
│
├── data/
│   ├── LONG_EC_UNIFICADA_TFM.xlsx     # Base de datos en formato panel (long)
│   └── otros datasets relevantes
│
├── scripts/
│   ├── 01_limpieza_preparacion.R      # Limpieza, transformación log y rezagos
│   ├── 02_modelo_panel.R              # Estimaciones Pooled, RE, FE
│   ├── 03_pruebas_diagnostico.R       # Hausman, BG/Wooldridge, Pesaran
│   ├── 04_graficos_descriptivos.R     # Tendencias y dispersión
│   └── 05_graficos_modelo.R           # Efectos fijos, residuos, ajustados
│
├── figures/
│   ├── pib_paises.png
│   ├── disp_x2lag_y.png
│   ├── efectos_fijos_paises.png
│   └── demás visualizaciones
│
├── TFM_Ricardo_Naranjo.pdf            # Documento final (opcional)
│
└── README.md                          # Este archivo
```

---

## 📊 **Contenido del análisis**

### **1. Preparación y limpieza**
- Conversión del dataset a formato **panel long**  
- Creación de rezagos  
- Transformación logarítmica de todas las variables  
- Control de NA y valores atípicos  

---

### **2. Modelos estimados**

- **Pooled OLS (modelo agrupado)**  
- **Efectos aleatorios (RE)**  
- **Efectos fijos dos vías (FE two–ways)**  
- **Prueba de Hausman para selección del modelo**

Modelo final elegido: **FE two–ways**.

---

## 🚀 **Cómo reproducir el análisis**

```r
install.packages(c(
  "plm", "dplyr", "ggplot2", "patchwork",
  "viridis", "stargazer"
))
```

---

## 📝 **Licencia**

MIT License.

---

## 📧 **Contacto**

**Ricardo Olmedo Naranjo**  
📩 *rikrdonhojas@gmail.com*
