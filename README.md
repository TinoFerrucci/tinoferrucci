# ¡Hola, soy Constantino Ferrucci! 👋

¡Bienvenido a mi perfil de GitHub! Soy un entusiasta del desarrollo y desde que me adentré en el mundo de la programación estoy en constante crecimiento con mi lenguaje favorito de programación, Python.

## Acerca de mí

- 🌍 Soy de la ciudad de Rosario, Santa Fe, Argentina.
- 💻 Actualmente me desempeño como AI Developer en Wiener Lab.
- 🤖 Doy clases de NLP y CV en la carrera de Inteligencia Artificial en la UNR.
- 🎓 Soy Técnico Universitario en Inteligencia Artificial (UNR).

## Tecnologías más utilizadas

### Lenguajes
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![R](https://img.shields.io/badge/r-%23276DC3.svg?style=for-the-badge&logo=r&logoColor=white)

### Frameworks
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Langchain](https://img.shields.io/static/v1?style=for-the-badge&message=LangChain&color=1C3C3C&logo=LangChain&logoColor=FFFFFF&label=)

### Bases de datos
![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)

### Versionadores de codigo
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

### Entornos de desarrollo
![PyCharm](https://img.shields.io/badge/pycharm-143?style=for-the-badge&logo=pycharm&logoColor=black&color=black&labelColor=green)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)

### Otras tecnologías
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

## Mis Proyectos Destacados

### ## [Datagentra — Analista de Datos Autónomo](https://github.com/TinoFerrucci/Datagentra)                                                                                                                                                            
Este proyecto nació como una herramienta personal para consultar bases de datos sin escribir SQL, y durante su desarrollo se convirtió en una aplicación full-stack con agente autónomo, historial de conversaciones y soporte para múltiples fuentes
 de datos.                                                                                                                                                                                                                                           
                                                                                                                                                                                                                                                     
En este proyecto se aplican:                                                                                                                                                                                                                         
                                                                
* Pipeline de Text-to-SQL con agente autónomo:                                                                                                                                                                                                       
  * Diseño e implementación de un pipeline de 5 pasos: generación de SQL, ejecución con reintentos automáticos, resumen de resultados, sugerencia de gráfico y serialización de respuesta.
  * Integración con LangChain para abstraer el proveedor LLM: compatible con OpenAI (cloud) y Ollama (local, sin costo).                                                                                                                             
  * Motor de solo lectura con bloqueo de operaciones peligrosas (`INSERT`, `UPDATE`, `DELETE`, `DROP`) a nivel de evento en SQLAlchemy.                                                                                                              
* Desarrollo de API REST con FastAPI:                                                                                                                                                                                                                
  * Arquitectura de endpoints para el pipeline de consulta, gestión de conversaciones, carga de archivos y configuración dinámica del proveedor LLM.                                                                                                 
  * Validación de modelos con Pydantic y manejo de errores con reintentos inteligentes.                                                                                                                                                              
* Frontend React + TypeScript:                                                                                                                                                                                                                       
  * Interfaz de chat completa con visualización de SQL, gráficos automáticos y resúmenes generados por el LLM.                                                                                                                                       
  * Componentes de gráficos dinámicos (bar, line, area, pie, KPI) con Recharts adaptados al tipo de datos retornado.                                                                                                                                 
  * Tema claro/oscuro persistido en `localStorage` y diseño responsive con Tailwind CSS.                                                                                                                                                             
* Memoria contextual por conversación:                                                                                                                                                                                                               
  * Persistencia de historial en SQLite con inyección de las últimas N preguntas y respuestas en el prompt del agente, habilitando preguntas de seguimiento naturales.                                                                               
* Carga y corrección de archivos:                                                                                                                                                                                                                    
  * Soporte para subir CSV y SQLite como fuentes de datos activas.                                                                                                                                                                                   
  * Motor de correcciones en lenguaje natural (renombrar columnas, eliminar campos, convertir tipos) antes de confirmar el source.                                                                                                                   
* Despliegue con Docker Compose:                                                                                                                                                                                                                     
  * Orquestación de tres servicios con dependencias y health checks: `db-init` (semillado de base de datos), `backend` y `frontend`.                                                                                                                 
  * Configuración automática de paths de base de datos según el entorno (local vs. Docker).

Este proyecto representa la integración de múltiples disciplinas en una sola aplicación cohesiva: desde el diseño de pipelines de IA y la comunicación con modelos de lenguaje, hasta el desarrollo de una API REST robusta y una interfaz de usuario moderna. La combinación de un agente autónomo con memoria contextual, ejecución segura de SQL y visualización dinámica de datos demuestra una visión end-to-end del desarrollo de software orientado a inteligencia artificial. Sentite libre de     explorar el código, levantar el proyecto con un solo comando y consultar cualquier base de datos en lenguaje natural.
  
### [Asistente inteligente basado en videojuegos](https://github.com/TinoFerrucci/NLP_Final_Project)
Este proyecto nació como un trabajo final para la asignatura Procesamiento de Lenguaje Natural, pero durante su desarrollo, se reveló como un proyecto excepcionalmente versátil y prometedor.

En este proyecto se aplican:

* Técnicas de procesamiento del lenguaje natural:
  * Empleo de técnicas de limpieza de texto para disminuir la cantidad de valores únicos de cadenas y así poder facilitar el procesamiento.
* Obtención de Datos Innovadora:
  * Utilicé técnicas de scrapping con HTML para recopilar datos relevantes.
  * Implementé una interfaz de programación de aplicaciones (API) Rest para obtener información en formato JSON.
* Vectorización y Almacenamiento Eficiente:
  * Aplicación de modelos avanzados de vectorización para representar información textual de manera efectiva.
  * Empleo de ChromaDB como una base de datos vectoriales para almacenar información, contenido e índices de documentos indexados.
* Búsqueda Semántica y Similitud de Textos:
  * Desarrollé algoritmos que permiten la búsqueda potente de similitudes semánticas entre documentos y textos, aprovechando vectores de altas dimensiones.
* Arquitectura Eficiente del Asistente:
  * Diseñé e implementé una arquitectura robusta para garantizar el funcionamiento eficiente del asistente inteligente.
* Conversaciones Contextuales y Generación de Texto:
  * Integré de manera efectiva sistemas de generación de texto de código abierto para habilitar diálogos naturales y contextualmente relevantes.
* Estudios en Agentes Inteligentes Autónomos:
  * Realicé investigaciones sobre agentes inteligentes autónomos, explorando su aplicación en el contexto de un asistente basado en problemáticas de la vida real.
* Entre otros puntos más.

Este proyecto representa mi dedicación y aplicación práctica de tecnologías avanzadas. Estas herramientas separadas son potentes y unidas proporcionan una experiencia agradable al usuario tanto es así que va más allá de un simple trabajo final. Sientete libre de explorar el código y descubrir el potencial de este asistente inteligente.

### [Predicción de lluvia en Australia](https://github.com/Shannon-21/Aprendizaje_Automatico_1)
Este proyecto nació como un desarrollo de varias instancias para la asignatura Aprendizaje Automático donde el objetivo fue desarrollar un sistema inteligente capaz de predecir a partir de datos entregados por el usuario la lluvia en Australia (si lloverá y en qué medida).

Este proyecto fue realizado en conjunto con mi compañero [Fabio Giampaoli](https://github.com/Shannon-21) en donde se tocaron los siguientes puntos:

* Análisis de datos:
  * Se visualizaron patrones y comportamiento de las variables.
  * Se trataron las variables ajustandolas a través de normalización y estandarización dependiendo su comportamiento.
* Modelos de regresión:
  * Utilización de modelos de regresión para evaluar la cantidad de lluvia.
* Modelos de clasificación:
  * Implementación de modelos de clasificación para identificar la probabilidad de lluvia.
* Redes neuronales:
  * Incorporación de arquitecturas de redes neuronales para mejorar el rendimiento y métricas a la hora de predecir.
* Optimización de hiperparametros:
  * Empleo de técnicas para la optimización de hiperparametros basandose en métricas devueltas por los modelos evaluados obteniendo de esa forma el mejor modelo para cada arquitectura implementada.
* Explicabilidad:
  * Utilización de SHAP y de sus gráficos para explicar la salida del modelo y notar así el comportamiento que pueda afectar positivamente o negativamente la predicción obtenida.
* Despliegue del Proyecto:
  * Creación de un pipeline que encapsula todo el proceso de desarrollo.
  * Implementación exitosa en la plataforma Streamlit para su accesibilidad, visualización e interactividad con la aplicación.

Este proyecto representa un esfuerzo conjunto para abordar la tarea desafiante que nos propuso la catedra de la asignatura. La inclusión de múltiples enfoques y modelos en donde se varía desde modelos de regresión hasta redes neuronales demuestra una amplia comprensión de las herramientas disponibles. Explora el código implementado y no olvides probar la aplicación para ver inmediatamente los resultados del desarrollo.

### Otros proyectos
* [Procesamiento de imagenes (Python - Trabajo grupal)](https://github.com/Shannon-21/TP_Procesamiento_Imagenes)
* [Bot de telegram de noticias (Python - Trabajo grupal)](https://github.com/Shannon-21/NLP_TP1)
* [Pronóstico deportivos (Java - Argentina Programa)](https://github.com/AlexLopezz/JAVA-Proyecto_Pronosticos-Deportivos)
* [SQLAlchemy with FastAPI (Python - Proyecto personal)](https://github.com/TinoFerrucci/sqlalchemy_with_fastapi)
* [Base de datos de un cine (SQL - Trabajo grupal)](https://github.com/Shannon-21/TUIA_BD_TP1)
* [Análisis de datos de Estadistica (R - Trabajo grupal)](https://github.com/Simon890/estadistica_tp1)
* [Bash scripting (Bash - Trabajo individual)](https://github.com/TinoFerrucci/tp-entorno)
* [CRUD de Recetas (Python - Proyecto personal)](https://github.com/TinoFerrucci/CRUDProgram)
* [Juegos básicos (Python - Proyecto personal)](https://github.com/TinoFerrucci/PythonGames)

## Contacto
¡Contactate conmigo en las siguientes redes sociales!


[![LinkedIn Logo](https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/constantino-ferrucci-7574121a9/) 
[![Gmail Logo](https://img.shields.io/badge/-Gmail-c14438?style=flat-square&logo=Gmail&logoColor=white)](mailto:constantinoferrucci@gmail.com)

---

¡Gracias por visitar mi perfil! Espero que encuentres interesantes mis proyectos y contribuciones.
