📊 Sistema de Autodiagnóstico de Competencias Digitales (DigComp 2.2)

Trabajo de Fin de Grado (TFG)

Autor: Raúl Molina García

Universidad: Universidad de Castilla-La Mancha (UCLM)

📖 Sobre el Proyecto

Este proyecto consiste en el diseño e implementación de una herramienta de autodiagnóstico que permite a los usuarios evaluar su nivel en las 21 competencias digitales definidas en el marco europeo DigComp 2.2.

Basándose en los materiales, bancos de preguntas y actividades del proyecto DigitALL, se ha desarrollado un sistema automatizado que ofrece retroalimentación inmediata, adaptando el cuestionario a los seis niveles de competencia (A1–C2) y proponiendo mejoras personalizadas.

🎯 Objetivos Principales

Cuestionario Adaptativo: Evaluación integral que abarca desde el nivel básico (A1) hasta el altamente especializado (C2).

Corrección Automática: Generación de informes personalizados de resultados (exportables a PDF).

Recomendaciones de Formación: Vinculación directa entre los resultados obtenidos y recursos de mejora.

Validación: Herramienta evaluada mediante pruebas piloto de usabilidad.

🛠️ Stack Tecnológico (PERN)

El proyecto está construido bajo la arquitectura PERN:

Frontend:

React (v19) con Vite

React Router DOM para el enrutamiento.

Lucide React para la iconografía.

jsPDF para la generación de informes en PDF.

Backend:

Node.js & Express

PostgreSQL (paquete pg) para la persistencia de datos.

nodemailer para el envío de correos.

multer para la gestión de archivos.

🚀 Instalación y Configuración

Sigue estos pasos para levantar el proyecto en tu entorno local.

Prerrequisitos

Node.js (v18 o superior recomendado)

PostgreSQL instalado y en ejecución.

1. Clonar el repositorio

git clone https://github.com/rmg0707/Test-de-autodiagnostico-de-competencias-digitales-TFG.git
cd Test-de-autodiagnostico-de-competencias-digitales-TFG


2. Configuración del Backend

cd backend
# Instalar dependencias
npm install


Crea un archivo .env en la raíz de la carpeta backend con tus credenciales de base de datos y configuración (ajusta según tus necesidades):

PORT=3000
DB_USER=tu_usuario_pg
DB_PASSWORD=tu_contraseña_pg
DB_HOST=localhost
DB_PORT=5432
DB_NAME=digcomp_db


Inicia el servidor en modo desarrollo:

npm run dev


3. Configuración del Frontend

En una nueva terminal, navega a la carpeta del frontend:

cd frontend
# Instalar dependencias
npm install


Inicia la aplicación de React:

npm run dev


La aplicación estará disponible por defecto en http://localhost:5173.

📝 Metodología

Estudio exhaustivo del marco DigComp y recursos DigitALL.

Revisión del estado del arte en plataformas de autoevaluación.

Diseño pedagógico y técnico del modelo de cuestionario (preguntas, saltos lógicos, feedback).

Implementación full-stack del sistema y base de datos.

Despliegue en entorno de pruebas piloto y análisis de resultados de la muestra de usuarios.

⚖️ Licencia

Este proyecto ha sido desarrollado con fines académicos como Trabajo de Fin de Grado en la Universidad de Castilla-La Mancha (UCLM).
