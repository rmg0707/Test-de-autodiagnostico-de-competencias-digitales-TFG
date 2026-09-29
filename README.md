# 📊 Sistema de Autodiagnóstico de Competencias Digitales (DigComp 2.2)

[![Universidad](https://img.shields.io/badge/Universidad-UCLM-red.svg)](https://www.uclm.es/)
[![Estado](https://img.shields.io/badge/Estado-Finalizado-success.svg)]()
[![React](https://img.shields.io/badge/Frontend-React_19-blue.svg)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Backend-Node.js_&_Express-green.svg)](https://nodejs.org/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791.svg)](https://www.postgresql.org/)

**Trabajo de Fin de Grado (TFG)**
* **Autor:** Raúl Molina García
* **Universidad:** Universidad de Castilla-La Mancha (UCLM)

---

## 📖 Sobre el Proyecto

Este proyecto consiste en el diseño e implementación de una herramienta de autodiagnóstico que permite a los usuarios evaluar su nivel en las 21 competencias digitales definidas en el **marco europeo DigComp 2.2**. 

Basándose en los materiales, bancos de preguntas y actividades del proyecto *DigitALL*, se ha desarrollado un sistema automatizado que ofrece retroalimentación inmediata, adaptando el cuestionario a los seis niveles de competencia (A1–C2) y proponiendo mejoras personalizadas.

### 🎯 Objetivos Principales
- **Cuestionario Adaptativo:** Evaluación integral que abarca desde el nivel básico (A1) hasta el altamente especializado (C2).
- **Corrección Automática:** Generación de informes personalizados de resultados (exportables a PDF).
- **Recomendaciones de Formación:** Vinculación directa entre los resultados obtenidos y recursos de mejora.
- **Validación:** Herramienta evaluada mediante pruebas piloto de usabilidad.

---

## 🛠️ Stack Tecnológico (PERN)

El proyecto está construido bajo la arquitectura PERN:

**Frontend:**
- [React (v19)](https://react.dev/) con [Vite](https://vitejs.dev/)
- [React Router DOM](https://reactrouter.com/) para el enrutamiento.
- [Lucide React](https://lucide.dev/) para la iconografía.
- [jsPDF](https://parall.ax/products/jspdf) para la generación de informes en PDF.

**Backend:**
- [Node.js](https://nodejs.org/) & [Express](https://expressjs.com/)
- [PostgreSQL](https://www.postgresql.org/) (paquete `pg`) para la persistencia de datos.
- `nodemailer` para el envío de correos.
- `multer` para la gestión de archivos.

---

## 🚀 Instalación y Configuración

Sigue estos pasos para levantar el proyecto en tu entorno local.

### Prerrequisitos
- [Node.js](https://nodejs.org/) (v18 o superior recomendado)
- [PostgreSQL](https://www.postgresql.org/) instalado y en ejecución.

### 1. Clonar el repositorio
```bash
git clone https://github.com/rmg0707/Test-de-autodiagnostico-de-competencias-digitales-TFG.git
cd Test-de-autodiagnostico-de-competencias-digitales-TFG
```

### 2. Configuración del Backend
```bash
cd backend
# Instalar dependencias
npm install
```
Crea un archivo `.env` en la raíz de la carpeta `backend` con tus credenciales de base de datos y configuración (ajusta según tus necesidades):
```env
PORT=3000
DB_USER=tu_usuario_pg
DB_PASSWORD=tu_contraseña_pg
DB_HOST=localhost
DB_PORT=5432
DB_NAME=digcomp_db
```
Inicia el servidor en modo desarrollo:
```bash
npm run dev
```

### 3. Configuración del Frontend
En una nueva terminal, navega a la carpeta del frontend:
```bash
cd frontend
# Instalar dependencias
npm install
```
Inicia la aplicación de React:
```bash
npm run dev
```
La aplicación estará disponible por defecto en `http://localhost:5173`.

---

## 📝 Metodología
1. Estudio exhaustivo del marco DigComp y recursos DigitALL.
2. Revisión del estado del arte en plataformas de autoevaluación ya existentes.
3. Diseño pedagógico y técnico del modelo de cuestionario (preguntas, saltos lógicos, feedback).
4. Implementación full-stack del sistema y base de datos.
5. Despliegue y análisis de resultados de la muestra de usuarios reales.

---

## ⚖️ Licencia
Este proyecto ha sido desarrollado con fines académicos como Trabajo de Fin de Grado en la Universidad de Castilla-La Mancha (UCLM).
