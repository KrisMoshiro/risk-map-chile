# 🌍 Risk Map Iquique

![Deploy](https://img.shields.io/github/deployments/krismoshiro/risk-map-iquique-front/github-pages?label=Deploy&style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

**Servicio para la visualización interactiva de zonas críticas de accidentes en la Región de Tarapacá, Chile**  
Repositorio principal del proyecto de investigación basado en minería de datos y visualización geográfica.

🔗 **Demo:** [https://krismoshiro.github.io/risk-map-iquique-front/](https://krismoshiro.github.io/risk-map-iquique-front/)

---

## 🧩 Estructura del Proyecto

El proyecto completo se compone de tres repositorios conectados:

- **Frontend:** [`risk-map-iquique-front`](https://github.com/krismoshiro/risk-map-iquique-front)  
- **Backend:** [`risk-map-iquique-back`](https://github.com/vistor05/Risk_Map_Iquique_Back)  
- **Datos:** [`risk-map-iquique-data`](https://github.com/krismoshiro/risk-map-iquique-data)  

---

## 📌 Objetivo del Proyecto

Analizar los accidentes de tránsito en la Región de Tarapacá entre los años **2010 y 2023**, utilizando **minería de datos** para identificar zonas de mayor riesgo y permitir una **visualización geográfica clara** de estos puntos críticos.

### Problemas Abordados

- Datos disponibles como reportes, no como mapas interactivos.
- Falta de accesibilidad y visualización geoespacial.
- Limitaciones en uso de datos para toma de decisiones.

### Impacto Esperado

- Identificación de zonas críticas.
- Apoyo a decisiones urbanas y de seguridad vial.
- Visualización accesible para autoridades y ciudadanía.

---

## ⚙️ Tecnologías Utilizadas

### Frontend

- [React 19](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [Material UI](https://mui.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Framer Motion](https://www.framer.com/motion/)
- [Vite](https://vitejs.dev/)
- [GitHub Pages](https://pages.github.com/)

### Backend & Data Processing

- [Python](https://www.python.org/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [pandas](https://pandas.pydata.org/)
- [folium](https://python-visualization.github.io/folium/)
- [DBSCAN](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html)

---

## 📄 Documentación

### API REST

👉 La documentación completa de la API está disponible en Swagger:  
🔗 [https://risk-map-iquique-back.onrender.com/docs](https://risk-map-iquique-back.onrender.com/docs)

### Minería de Datos en Python

📍 Enlace a documentación técnica  
🔗( próximamente disponible... )

---

## 🧠 Proceso de Minería de Datos

### 1. Comprensión del Negocio

- Datos públicos de siniestros viales de **Carabineros de Chile** y **CONASET**.
- Foco en accidentes con geolocalización en la región de Tarapacá.

### 2. Preparación de los Datos

- Limpieza y transformación de registros.
- Geocodificación: conversión a latitud y longitud.

### 3. Modelado

- Aplicación del algoritmo **DBSCAN** para segmentación espacial.
- Agrupación de siniestros en zonas críticas.
- Clustering por:
  - **Tramos horarios:** 00-06, 06-12, 12-19, 19-00.
  - **Gravedad:** Muertos, graves, menos graves, leves, ilesos.

### 4. Evaluación

- Validación visual con mapas generados con **Folium**.
- Comparación con conocimiento empírico de zonas de riesgo.
- Futuras mejoras: uso de métricas como silueta o codo.

---

## 🖥️ Instalación y Uso

### Clonar los Repositorios

```bash
git clone https://github.com/krismoshiro/risk-map-iquique-front.git
git clone https://github.com/vistor05/Risk_Map_Iquique_Back.git
git clone https://github.com/krismoshiro/risk-map-iquique-data.git
```
### Frontend
```bash
cd risk-map-iquique-front
npm install
npm run dev
```
### Backend
```bash
cd ../Risk_Map_Iquique_Back
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```
### 👥 Créditos
Proyecto desarrollado por:

Christian Hernández – @krismoshiro
Victor Muñoz – @vistor05
