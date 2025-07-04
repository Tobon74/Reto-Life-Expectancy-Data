# 🧠 Análisis Exploratorio de Datos: Esperanza de Vida 🌍

Este repositorio contiene un análisis exploratorio completo del dataset **"Life Expectancy Data"**, realizado a partir de un archivo CSV proporcionado como reto. El trabajo incluye limpieza de datos, diagnóstico de completitud, clasificación de variables, matriz de correlaciones y regresión lineal múltiple.

> 📌 El análisis fue desarrollado combinando herramientas como **Google Colab** (Python, pandas, scikit-learn) y **Microsoft Excel Online**, documentando cada paso y los desafíos técnicos encontrados en plataformas en la nube.

---

## 📁 Estructura del Proyecto

- `Reto Life Expectancy Data.csv`: Archivo original cargado con separador europeo (`;`) y decimales con coma.
- `Analisis_Exploratorio_Completo.xlsx`: Archivo final con las siguientes hojas:
  - `Datos Limpios`: Datos listos para análisis.
  - `Completitud`: Conteo de valores faltantes por variable.
  - `Tipos de Variables`: Clasificación de variables cualitativas y cuantitativas.
  - `Matriz Correlación`: Correlaciones entre variables numéricas.
  - `Regresión Lineal`: Coeficientes y modelo predictivo.
  - `Informe`: Apunte de investigación resumen del trabajo.

---

## 📊 Metodología

1. **Análisis de Completitud**
   - Se detectaron y cuantificaron los valores faltantes.
   - Se corrigieron formatos y eliminó ruido textual en las filas.
   - Conversión de variables con coma decimal a formato numérico estándar (`.`).

2. **Clasificación de Variables**
   - Variables **cuantitativas**: `Life expectancy`, `Alcohol`, `BMI`, entre otras.
   - Variables **cualitativas**: `Country`, `Status`.

3. **Matriz de Correlación**
   - Calculada sobre variables numéricas limpias.
   - Revela relaciones significativas (positivas y negativas).

4. **Regresión Lineal Múltiple**
   - Variable dependiente: `Life expectancy`.
   - Variables independientes: `Alcohol`, `BMI`, `infant deaths`, `Adult Mortality`, etc.
   - Modelo generado usando `scikit-learn`.

5. **Informe de Resultados**
   - Interpretación de correlaciones.
   - Selección de variables predictoras.
   - Observaciones sobre la calidad del dataset y decisiones de limpieza.

---

## ⚠️ Problemas y Limitaciones encontradas en Excel Online

Aunque Excel Online fue útil para visualización y limpieza básica, se identificaron varias **limitaciones técnicas** durante el análisis:

| Problema encontrado 🐞                | Detalles |
|--------------------------------------|----------|
| ❌ No permite filtrar por celdas vacías | Falta la opción "(Vacías)" en filtros como en Excel de escritorio. Se tuvo que usar una columna auxiliar con `SI(ESBLANCO(...))`. |
| ❌ Incompatibilidad con `COEF.DE.CORREL` en rangos completos | Algunas fórmulas fallaban si las columnas tenían encabezados o vacíos. Se optó por usar rangos acotados como `B2:B3000`. |
| ❌ Celdas "atascadas" en formato texto | Hubo que cambiar el formato a “General” y volver a escribir las fórmulas. |
| ❌ Separador decimal por coma (`,` en vez de `.`) | Generó errores al convertir los datos. Se reemplazaron las comas por puntos antes de procesar. |

> 🛠️ **Recomendación**: para análisis estadístico o manipulación de datos más complejos, se sugiere usar **Excel de escritorio o Python con pandas**.

---

## 📌 Requisitos para reproducir el análisis

- Google Colab o entorno Python 3.x con:
  - `pandas`
  - `scikit-learn`
- Microsoft Excel (preferiblemente versión de escritorio para mayor compatibilidad)
- Archivo CSV original (formato europeo)

---

## 🤝 Créditos

El trabajo fue desarrollado como parte de un reto de análisis exploratorio por [Carlos Villa](#), combinando ciencia de datos, visualización y documentación profesional.

---

## 📥 Contacto

¿Tienes dudas, sugerencias o quieres colaborar?  
¡No dudes en escribirme!

📧 carlosvilla@ejemplo.com  
📍 CDMX | 🌎 Global

---

**Gracias por visitar este proyecto. ¡Sigue explorando y aprendiendo!** 🚀
