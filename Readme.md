# RetainHub: Sistema Inteligente de Alerta Temprana

## Descripción del Proyecto
RetainHub es una solución analítica avanzada diseñada para el sector e-commerce[cite: 1, 120]. [cite_start]El proyecto aborda el alto costo de adquisición de clientes, donde captar un nuevo usuario es 5 veces más caro que retenerlo. 

El sistema identifica la "pérdida silenciosa" de clientes (Churn) analizando el comportamiento histórico de compra y navegación. Mediante un modelo predictivo de clasificación, RetainHub genera un puntaje de riesgo (0-100%) y un listado de los 100 clientes más críticos, permitiendo que los equipos de marketing actúen proactivamente con ofertas personalizadas para recuperar hasta un 25% de los ingresos en riesgo.

## Objetivo
Construir un modelo predictivo de clasificación para identificar clientes con alta probabilidad de abandono (Churn) y reducir la tasa de rotación mediante campañas de marketing dirigidas..

## Integrantes y Roles
* **Carlos Suárez Sánchez:** Responsable de Datos y ETL (Carga, limpieza y transformación)
* **Ángela María Baena Alba:** Ingeniería de Características (Métricas RFM y preparación de variables)
* **Mariano Correa Carballo:** Científico de Datos (Modelado, algoritmos y gestión de desequilibrio)
* **Rodrigo Núñez Gómez:** Analista de Negocios y Presentación (Visualización, reporte y entorno Colab)

## Arquitectura Resumida
El sistema se estructura como un pipeline de datos lineal ejecutado en la nube:
1. **Ingesta:** Carga de ficheros CSV o bases de datos con el historial de compras de fuentes como Kaggle u Online Retail.
2. **Ingeniería de Características:** Creación de métricas de comportamiento como RFM (Recencia, Frecuencia y Valor Monetario)
3. **Modelado ML:** Entrenamiento de algoritmos de clasificación (Random Forest o Regresión Logística) con técnicas de balanceo de datos.
4. **Salida/Dashboard:** Reporte estático del "Top 100" de clientes en riesgo y visualización de patrones de abandono.

## Tecnologías
* **Lenguaje:** Python.
* **Entorno de desarrollo:** Google Colab / Jupyter Notebooks.
* **Librerías principales:** * **Pandas:** Procesamiento de datos tabulares.
    * **Scikit-learn:** Implementación de modelos ML.
    * **PyCaret:** Herramienta de Auto-ML (Plan B para agilizar el modelado).
 
## Organización del repositorio
Se utilizará un flujo de trabajo basado en ramas (branches) por integrante para evitar conflictos en el código principal ( main). Las entregas parciales se consolidarán en la carpeta src/.

### Estructura de Alfombras Recomendada
Esta es la disposición de archivos que deben aparecer en el repositorio:

```text
RetainHub/
├── docs/
│   └── Fase0_Presentacion_y_Viabilidad.pdf  # Documento actual del proyecto
├── src/
│   ├── cleaning.py        # Tareas del Integrante 1
│   ├── engineering.py     # Tareas del Integrante 2
│   └── modeling.ipynb     # Tareas del Integrante 3 (Notebook Colab)
├── data/
│   └── .gitkeep           # Para mantener la carpeta en Git sin subir datasets pesados
├── environment/
│   └── requirements.txt   # Librerías necesarias (Pandas, Scikit-learn, PyCaret)
├── README.md              # Información general del proyecto
└── .gitignore             # Filtro de archivos no deseados
```

## Cómo ejecutar (Instalación Inicial)
*Nota: El sistema se encuentra actualmente en fase de desarrollo (Semana 1)*

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/Rodrigmezz/Grupo1.git](https://github.com/Rodrigmezz/Grupo1.git)
