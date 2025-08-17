# AluraStoreLatam — Análisis exploratorio y geoespacial de ventas


## 🏆 Insignias
[![Estado](https://img.shields.io/badge/estado-completo-green)]()
[![Python](https://img.shields.io/badge/python-3.8%2B-blue)]()
[![License: MIT](https://img.shields.io/badge/licencia-MIT-blue.svg)]()
[![Notebook](https://img.shields.io/badge/notebook-Jupyter-orange)]()

---

## 📌 Índice

- [AluraStoreLatam — Análisis exploratorio y geoespacial de ventas](#alurastorelatam--análisis-exploratorio-y-geoespacial-de-ventas)
  - [🏆 Insignias](#-insignias)
  - [📌 Índice](#-índice)
  - [📙 Descripción del Proyecto](#-descripción-del-proyecto)
  - [💻 Entorno: Google Colab](#-entorno-google-colab)
  - [🗂️ Jerarquía / Flujo del Notebook (orden exacto)](#️-jerarquía--flujo-del-notebook-orden-exacto)
  - [🔍 Desarrollo — 5 puntos principales (detallado)](#-desarrollo--5-puntos-principales-detallado)
  - [✨ Extra (Plus): Exploración Geográfica](#-extra-plus-exploración-geográfica)
  - [🧠 Conceptos de programación destacados (por qué importan para el análisis)](#-conceptos-de-programación-destacados-por-qué-importan-para-el-análisis)
  - [▶️ Cómo ejecutar (Colab y local)](#️-cómo-ejecutar-colab-y-local)
    - [Abrir en Colab (recomendado)](#abrir-en-colab-recomendado)
    - [Ejecutar localmente (Jupyter)](#ejecutar-localmente-jupyter)
    - [Exportar resultados](#exportar-resultados)
  - [📦 Dependencias / requirements.txt sugerido](#-dependencias--requirementstxt-sugerido)
  - [📝 Informe Final: Análisis para la Selección de Tienda para el Sr. Juan](#-informe-final-análisis-para-la-selección-de-tienda-para-el-sr-juan)
  - [🤝 Personas Contribuyentes](#-personas-contribuyentes)
  - [👨‍💻 Personas Desarrolladoras / Autor](#-personas-desarrolladoras--autor)
  - [⚖️ Licencia](#️-licencia)
  - [✅ Siguientes pasos (opcional — te puedo ayudar a)](#-siguientes-pasos-opcional--te-puedo-ayudar-a)

---

## 📙 Descripción del Proyecto

`AluraStoreLatam` es un notebook de análisis exploratorio de datos (EDA) y análisis geoespacial, diseñado para comparar el desempeño de cuatro tiendas `(tienda_1 … tienda_4)`, con el objetivo de entregar un **Informe Final** que apoye la decisión del Sr. Juan sobre cuál tienda seleccionar para un nuevo emprendimiento.

---

## 💻 Entorno: Google Colab

Este notebook está pensado para ejecutarse fácilmente en **Google Colab** (ideal para reproducibilidad y acceso sin instalar dependencias locales). También puede ejecutarse localmente en Jupyter Notebook / JupyterLab si prefieres.

**Abrir en Colab**: añade el enlace directo a Colab desde tu repo (botón *Open in Colab* en la portada) o abre `AluraStoreLatam.ipynb` desde GitHub > `Open in Colab`.

---

## 🗂️ Jerarquía / Flujo del Notebook (orden exacto)

1. **Importación de datos**  
2. **Informe Final: Análisis para la Selección de Tienda para el Sr. Juan**  
3. **Desarrollo**  
   - 3.1 Análisis de facturación  
   - 3.2 Ventas por categoría  
   - 3.3 Calificación promedio de la tienda  
   - 3.4 Productos más y menos vendidos  
   - 3.5 Envío promedio por tienda  
4. **Conclusión y Recomendación**  
5. **Extra: Exploración Geográfica de las Ventas** (plus)  
   - 5.1 Mapa de Calor (Heatmap) de Ventas por Tienda  
   - 5.2 Mapa Interactivo de Ventas por Ciudad  
   - 5.3 Patrones Geográficos y su Impacto en el Rendimiento de las Tiendas  
6. **Conclusión** (resumen final)

> Nota: los principales puntos de análisis son los 5 del "Desarrollo". La sección "Extra" es un valor agregado para profundizar en geografía y patrones.

---

## 🔍 Desarrollo — 5 puntos principales (detallado)

A continuación se describe brevemente qué hace cada uno de los 5 puntos principales del análisis (estos constituyen el núcleo del *deliverable*):

1. **Análisis de facturación**  
   - Agregaciones por tienda y por periodo (día / semana / mes).  
   - Series temporales y facturación acumulada para detectar tendencias y estacionalidad.  
   - KPIs: facturación total, ticket promedio, crecimiento interperiodo.

2. **Ventas por categoría**  
   - Distribución de ventas por categoría (share y evolución temporal).  
   - Identificación de categorías con mayor contribución y categorías en declive.

3. **Calificación promedio de la tienda**  
   - Cálculo de rating promedio y análisis de su relación con ventas y devoluciones.  
   - Detección de outliers (tiendas o productos con ratings anómalos).

4. **Productos más y menos vendidos**  
   - Listados Top N / Bottom N por unidades y por facturación.  
   - Visualizaciones para priorizar promociones o bajas de catálogo.

5. **Envío promedio por tienda**  
   - Métrica de costo/tiempo de envío promedio y su efecto en la conversión.  
   - Comparación entre tiendas para diagnóstico operativo.

---

## ✨ Extra (Plus): Exploración Geográfica

El módulo geoespacial es un plus que aporta contexto territorial a las decisiones:

- **Mapa de Calor (Heatmap) de Ventas por Tienda** — patrones de densidad, puntos calientes de demanda.  
- **Mapa Interactivo de Ventas por Ciudad** — agregados por ciudad con popups y métricas.  
- **Patrones Geográficos y su Impacto** — interpretación de cómo la localización afecta la facturación, envíos y calificaciones.

---

## 🧠 Conceptos de programación destacados (por qué importan para el análisis)

Para realizar un análisis eficiente es esencial dominar conceptos básicos de programación que se aplican directamente en este notebook:

- **Manipulación de datos (variables y estructuras)**: las variables permiten almacenar y procesar información dinámicamente; DataFrames y listas facilitan el filtrado y la agregación.  
- **Condicionales (`if` / `else`)**: permiten implementar lógica de negocio (p. ej. clasificar transacciones, detectar anomalías según umbrales de facturación o rating).  
- **Funciones**: modularizan cálculos y gráficas, haciendo el código más legible y reutilizable (evitan duplicación).  
- **Bucle `for`**: útil para generar series de gráficos, iterar sobre conjuntos de tiendas o categorías y procesar lotes de archivos.  
- **Listas y colecciones**: facilitan la manipulación de colecciones grandes (productos, ciudades, periodos).

---

## ▶️ Cómo ejecutar (Colab y local)

### Abrir en Colab (recomendado)
1. Sube el notebook `AluraStoreLatam.ipynb` a tu repo en GitHub.  
2. En la página del notebook en GitHub, haz clic en **Open in Colab** o utiliza este formato de URL:  
   `https://colab.research.google.com/github.com/FerPaye01/Challenge-Store/blob/main/AluraStoreLatam.ipynb`  
3. En Colab: instala dependencias en la primera celda (si no están instaladas) y ejecuta.

Ejemplo de celda para Colab (ejecutar al inicio):
```
# Instala dependencias necesarias (Colab)
!pip install pandas numpy matplotlib plotly scipy pyproj contextily adjustText matplotlib-scalebar
```

### Ejecutar localmente (Jupyter)

```
# crear entorno
python -m venv .venv
source .venv/bin/activate    # Linux / macOS
.venv\Scripts\activate       # Windows

# instalar dependencias
pip install -r requirements.txt

# ejecutar notebook
jupyter notebook AluraStoreLatam.ipynb
```


### Exportar resultados

*   En Colab: File > Download > Download .ipynb o Download .py / Download .html.

*   Localmente: usa jupyter nbconvert si quieres ejecutar/convertir en batch.




## 📦 Dependencias / requirements.txt sugerido

Guarda este contenido en requirements.txt:
``` 
pandas>=1.3
numpy>=1.21
matplotlib>=3.4
plotly>=5.0
scipy>=1.7
pyproj>=3.0
contextily>=1.2
adjustText>=0.7
matplotlib-scalebar>=0.7
```


> En Colab muchas librerías (pandas, numpy, matplotlib) ya vienen preinstaladas; instala las restantes según necesites.

## 📝 Informe Final: Análisis para la Selección de Tienda para el Sr. Juan

El notebook contiene una sección llamada "Informe Final: Análisis para la Selección de Tienda para el Sr. Juan" donde se sintetizan los hallazgos principales: comparativa de facturación, índices de satisfacción (rating), rendimiento por categoría y recomendaciones operativas y estratégicas (apertura/cierre/optimización logística). Esta sección está lista para extraer como un resumen ejecutivo para presentar al cliente.

## 🤝 Personas Contribuyentes
- Luzdila Lopez — documentación: Git & GitHub
- Ingrid Silva — buenas prácticas (README)
- Bruno Souza — soporte en instalación de Git
- Camila Alves — configuración de Git y redacción del README
- Bruno Divino — introducción a Open Source
- Paulo Silveira — uso de Markdown
- Álvaro Camacho - Instructor del curso
- Equipo de Instructores de Alura Latam (continuar agregando)
- Wilfredo Rojas - Información del Challenge


## 👨‍💻 Personas Desarrolladoras / Autor

- Oscar Fernando Paye Cahui - Autor
  - 🐙 GitHub: https://www.linkedin.com/in/oscar-paye01/
  - 💼 LinkedIn: https://github.com/FerPaye01

## ⚖️ Licencia

Este proyecto está bajo la licencia  [MIT](./LICENSE).   – consulta el archivo LICENSE para más detalles.

## ✅ Siguientes pasos (opcional — te puedo ayudar a)

*   Generar requirements.txt y LICENSE como archivos del repo.

*   Crear un botón Open in Colab en la portada del README.

*   Exportar una versión InformeFinal_Resumen.pdf o HTML lista para enviar al Sr. Juan.

*   Convertir secciones clave a una mini-app (Streamlit) para explorar visualizaciones interactivas.




