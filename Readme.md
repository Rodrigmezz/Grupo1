RetainHub: Sistema Inteligente de Alerta Temprana

Objetivo
Construir un modelo predictivo de clasificación para identificar clientes con alta probabilidad de abandono (Churn) y reducir la tasa de rotación mediante campañas de marketing dirigidas..

Miembros del Equipo

Integrante 1 : Responsable de Datos y ETL (Carga y limpieza).


Integrante 2 : Ingeniero de Características (Métricas RFM y variables).
+1


Integrante 3 : Científico de Datos (Modelado y algoritmos).


Integrante 4 : Analista de Negocios y Presentación (Visualización y entorno).
+1

Organización del Repositorio
Se utilizará un flujo de trabajo basado en ramas (branches) por integrante para evitar conflictos en el código principal ( main). Las entregas parciales se consolidarán en la carpeta src/.

3. Estructura de Alfombras Recomendada
Esta es la disposición de archivos que deben aparecer en el repositorio:

Texto sin formato
RetainHub/
├── docs/
│   └── Fase0_Presentacion_y_Viabilidad.pdf  # Documento actual del proyecto [cite: 70-155]
├── src/
│   ├── cleaning.py        # Tareas del Integrante 1 [cite: 121]
│   ├── engineering.py     # Tareas del Integrante 2 [cite: 125]
│   └── modeling.ipynb     # Tareas del Integrante 3 (Notebook Colab) [cite: 129, 138]
├── data/
│   └── .gitkeep           # Para mantener la carpeta en Git sin subir datasets pesados [cite: 105]
├── environment/
│   └── requirements.txt   # Librerías necesarias (Pandas, Scikit-learn, PyCaret) [cite: 109, 117]
├── README.md              # Información general del proyecto
└── .gitignore             # Filtro de archivos no deseados


# RetainHub: Sistema Inteligente de Alerta Temprana 🚀

## 📝 Descripción del Proyecto
[cite_start]RetainHub es una solución analítica avanzada diseñada para el sector e-commerce[cite: 1, 120]. [cite_start]El proyecto aborda el alto costo de adquisición de clientes, donde captar un nuevo usuario es 5 veces más caro que retenerlo[cite: 127]. 

[cite_start]El sistema identifica la "pérdida silenciosa" de clientes (Churn) analizando el comportamiento histórico de compra y navegación[cite: 127, 128]. [cite_start]Mediante un modelo predictivo de clasificación, RetainHub genera un puntaje de riesgo (0-100%) y un listado de los 100 clientes más críticos, permitiendo que los equipos de marketing actúen proactivamente con ofertas personalizadas para recuperar hasta un 25% de los ingresos en riesgo[cite: 128].

## 👥 Integrantes y Roles
* [cite_start]**Carlos Suárez Sánchez:** Responsable de Datos y ETL (Carga, limpieza y transformación)[cite: 122].
* [cite_start]**Ángela María Baena Alba:** Ingeniería de Características (Métricas RFM y preparación de variables)[cite: 123].
* [cite_start]**Mariano Correa Carballo:** Científico de Datos (Modelado, algoritmos y gestión de desequilibrio)[cite: 124].
* [cite_start]**Rodrigo Núñez Gómez:** Analista de Negocios y Presentación (Visualización, reporte y entorno Colab)[cite: 125].

## 🏗️ Arquitectura Resumida
[cite_start]El sistema se estructura como un pipeline de datos lineal ejecutado en la nube[cite: 139, 143]:
1. [cite_start]**Ingesta:** Carga de ficheros CSV o bases de datos con el historial de compras de fuentes como Kaggle u Online Retail[cite: 131, 153].
2. [cite_start]**Ingeniería de Características:** Creación de métricas de comportamiento como RFM (Recencia, Frecuencia y Valor Monetario)[cite: 131, 155, 156, 157].
3. [cite_start]**Modelado ML:** Entrenamiento de algoritmos de clasificación (Random Forest o Regresión Logística) con técnicas de balanceo de datos[cite: 141, 166].
4. [cite_start]**Salida/Dashboard:** Reporte estático del "Top 100" de clientes en riesgo y visualización de patrones de abandono[cite: 137, 142].



## 🛠️ Tecnologías
* [cite_start]**Lenguaje:** Python[cite: 145].
* [cite_start]**Entorno de desarrollo:** Google Colab / Jupyter Notebooks[cite: 150].
* [cite_start]**Librerías principales:** * **Pandas:** Procesamiento de datos tabulares[cite: 147, 152].
    * [cite_start]**Scikit-learn:** Implementación de modelos ML[cite: 148].
    * [cite_start]**PyCaret:** Herramienta de Auto-ML (Plan B para agilizar el modelado)[cite: 149].

## 🚀 Cómo ejecutar (Instalación Inicial)
[cite_start]*Nota: El sistema se encuentra actualmente en fase de desarrollo (Semana 1)[cite: 177, 178].*

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/Rodrigmezz/Grupo1.git](https://github.com/Rodrigmezz/Grupo1.git)