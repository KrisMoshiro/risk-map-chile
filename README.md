<p align="center">
  <img src="https://github.com/user-attachments/assets/522291a8-8273-4e93-b8dd-95406795ccb7" alt="Risk Map Iquique Banner" width="400"/>
</p>

# 🌍 Risk Map Chile

![Deploy](https://img.shields.io/github/deployments/krismoshiro/risk-map-iquique-front/github-pages?label=Deploy&style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

**Visualización interactiva de zonas críticas de accidentes en la Región de Tarapacá, Chile.**  
Repositorio principal del proyecto de investigación basado en minería de datos y visualización geográfica.

🔗 **Demo:** [https://krismoshiro.github.io/risk-map-iquique-front/](https://krismoshiro.github.io/risk-map-iquique-front/)

![image](https://github.com/user-attachments/assets/0e33f5b9-6817-40a3-8ca8-db425d9f2f23)

---

## 🧩 Estructura del Proyecto

El proyecto completo se compone de tres repositorios conectados:

- **Frontend:** [`risk-map-chile-front`](https://github.com/krismoshiro/risk-map-chile-front)
- **Backend:** [`risk-map-chile-back`](https://github.com/vistor05/risk_map_chile_back) 
- **Datos:** [`risk-map-chile-data`](https://github.com/krismoshiro/risk-map-chile-data)

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

## 🖥️ Instalación y Uso

### Clonar los Repositorios

```bash
git clone https://github.com/krismoshiro/risk-map-chile-front.git
git clone https://github.com/vistor05/risk_map_chile_back.git
git clone https://github.com/krismoshiro/risk-map-chile-data.git
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
