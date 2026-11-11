# ESI Areté · Aplicación de caracterización y currículo individualizado

Aplicación web React + Vite construida a partir de `Matriz_preguntas_app_ESI_TEA.xlsx`.

## Qué incluye
- Bienvenida e información institucional basada en la matriz.
- Consentimiento del adulto, registro con código y rol, autorización del acudiente y asentimiento del estudiante.
- 16 preguntas para educadores y 6 preguntas visuales para estudiantes.
- Generación de niveles y ruta para los 10 temas, alertas y ajustes.
- Planificación de dos sesiones de 50 minutos por tema activo, usando las 6 fases de la hoja `Sesiones de 50 min`.
- Descarga local de PDF para equipo y versión resumida para familia.
- Sin base de datos, autenticación, `localStorage` ni envío de respuestas a un servidor. Las respuestas viven únicamente en memoria durante la sesión del navegador.

## Ejecutar en local
Requiere Node.js 20 o superior.

```bash
npm install
npm run dev
```

## Publicar en GitHub Pages
1. Crea un repositorio y sube el contenido de esta carpeta a la rama `main`.
2. En GitHub, abre **Settings → Pages** y selecciona **GitHub Actions** como fuente.
3. El flujo `.github/workflows/deploy.yml` compilará y publicará el sitio en cada `push` a `main`.

## PDF de autorización
El PDF oficial no venía incluido en el material recibido. Cuando el colegio lo entregue, copia el archivo a `public/Autorizacion_acudiente.pdf`. El enlace de descarga ya está preparado.

## Consideraciones de uso
- La herramienta genera una propuesta pedagógica, no un diagnóstico ni una decisión clínica.
- Las preguntas omitidas o pasadas no se convierten en respuestas negativas.
- T7 exige verificación manual de la Puerta 2. T9 exige verificar que T5 ya fue trabajado y T10 exige verificar que T4 ya fue trabajado.
- Las casillas de verificación de progresión son decisiones del equipo durante esa sesión y no se guardan al recargar.
- Los textos de consentimiento y protección de datos son borradores de la matriz y deben revisarse con la supervisión y el colegio antes de un piloto real.
