# README - Evaluación Parcial 3
## Login Seguro y Base de Datos Temática Libre con Supabase
## Descripción del proyecto
Este repositorio contiene el desarrollo de un sistema de autenticación seguro para usuarios, conectado a una base de datos en SUPABASE, que permite visualizar estadisticas de videojuegos mediante gráficos de barras y de torta.
El sistema incluye:
- Un formulario de login con validación y hash de contraseñas.
- Una página de bienvenida con gráficos generados por Chart.js.
- Consultas SQL avanzadas en Supabase para obtener y procesar los datos.
## Tecnologías utilizadas
- Frontend: HTML, Tailwind CSS, JavaScript.
- Librerias: SweetAlert2 (para mensajes), CryptoJS (para hash), Chart.js (para gráficos)
- Backend: Supabase (base de datos)
## Módulo de Autenticación
- Login: Validación de credenciales contra la tabla usuarios en Supabase.
- Seguridad: Las contraseñas se almacenan con hash SHA-256 irreversible.
- Mensajes: Feedback visual con SweetAlert2 para errores y éxito.
## Base de Datos en Supabase
El modelo relacional incluye al menos 5 tablas relacionadas con videojuegos, como:
- usuarios: Almacena credenciales de acceso.
- videojuegos: Contiene información de títulos y precios.
- plataformas: Relaciona videojuegos con sus plataformas disponibles.
- Otras tablas según la temática (ej: generos, desarrolladores).
##Consultas SQL Avanzadas
- JOIN: Para combinar datos de videojuegos y plataformas.
- CASE: Clasificación condicional de videojuegos por precio.
- HAVING: Filtrado de agregados (ej: plataformas con más de X juegos).
- Vista (VIEW): vw_videojuegos_por_plataforma para gráficos.
- Función almacenada (FUNCTION): Calcula estadísticas personalizadas.
- Trigger: Actualiza automáticamente fechas de modificación.
## Frontend y Visualización
- Login: Diseño responsivo con Tailwind CSS.
- Dashboard: Muestra dos gráficos:
  - Gráfico de barras: Precios de videojuegos.
  - Gráfico de dona: Cantidad de videojuegos por plataforma.
## Instalación y Uso
- Clonar repositorio: git clone https://github.com/Mayckol2005/SQL.git
- Abrir index.html en tu navegador para acceder al login.
- Ingresa credenciales válidas (registradas previamente en Supabase).
  - Usuario: cliente@gmail.com 
  - Contraseña: 123456
## Información del Proyecto
- Desarrollado por:
  - Mayckol Mardones
  - Carlos Moil
- Asignatura: Base de Datos Aplicada 001D
- Fecha de entrega: 26-06-2025
