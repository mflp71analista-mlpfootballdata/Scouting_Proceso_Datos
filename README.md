# ⚙️ Scouting y Procesado de datos de Fútbol (Python)

Este repositorio reúne un conjunto de desarrollos en **Python** enfocados en la ingeniería de datos deportivos, estandarización de eventos multi-proveedor y creación de algoritmos de priorización y recomendación para secretarías técnicas y departamentos de analítica táctica.

---

## 🛠️ Stack Tecnológico

* **Lenguaje:** Python
* **Librerías de Procesamiento de Datos:** Pandas, NumPy
* **Estadística & Modelado:** Scikit-Learn (Estandarización Z-Score, MinMax, distancias estadísticas)
* **Visualización de Apoyo:** Matplotlib, Seaborn, Mplsoccer

---

## 📂 Módulos & Funcionalidades Técnicas

### 1. Normalización e Integración Multi-Proveedor
* **Escalado de Coordenadas XY:** Algoritmos de transformación para estandarizar las coordenadas de eventos entre distintos proveedores (Wyscout, StatsBomb, Opta), garantizando la interoperabilidad de las bases de datos.
* **Ingesta y Categorización de Eventos:** Lógica personalizada para clasificar métricas complejas (ej. *Progressive Passes*, acciones defensivas exitosas, etc.).

### 2. Algoritmos de Scoring Ponderado por Posición
* **Sistemas de Pesos Adaptativos:** Desarrollo de modelos estadísticos que asignan pesos específicos a cada métrica según la demarcación táctica del futbolista (ej. priorizar volumen de distribución en mediocentros vs. desbordes y centros en extremos).
* **Modelos de Scouting para Fichajes:** Algoritmos diseñados para la evaluación específica de posiciones clave (ej. Delanteros Centro - DEL), generando notas ponderadas globales para la priorización de incorporaciones.

### 3. Métricas Estadísticas & Normalización *per 90*
* **Estadísticas Agregadas:** Normalización de datos brutos ajustados por minutos disputados para eliminar sesgos de participación.
* **Métricas Relativas (Percentiles & Z-Score):** Evaluación comparativa de futbolistas dentro de su grupo de pares y competición.
* **Similitud entre Equipos:** Cálculo de distancias y comparativa estadística del rendimiento global a nivel colectivo.

---

## 📝 Estructura del Repositorio (Notebooks)

* `WYSCOUT_RankingPosición_pesos.ipynb`: Algoritmo general de ranking ponderado según la demarcación.
* `WYSOCUT_Scouting_Fichajes_DEL_pesos.ipynb`: Modelo de scoring y priorización de fichajes para delanteros centro.
* `WYSOCUT_Scouting_Fichajes_pesos.ipynb`: Evaluación ponderada de perfiles de mercado para scouting.
* `WYSCOUT_Cdist_entre_jugadores.ipynb`: Algoritmos de distancia matricial entre futbolistas.
* `WYSCOUT_Prediccion.ipynb` / `WYSCOUT_Prediccion_2.ipynb`: Modelos exploratorios y análisis predictivo de rendimiento.

---

🔒 *Nota: Los datos brutos y archivos de datos (.csv/.json) no se incluyen en este repositorio público para proteger la propiedad intelectual de las fuentes de datos comerciales.*
