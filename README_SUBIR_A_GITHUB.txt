# Herramienta Digital EV - Versión Universidad Mayor v13

Esta versión está construida sobre la v12 y agrega una capa académica para Escuela de Enfermería / Universidad Mayor.

## Qué incluye

- Pantalla obligatoria de perfil académico al ingresar.
- Registro local del perfil académico.
- Registro en Supabase de:
  - ingresos académicos
  - consultas de medicamentos
  - comentarios por medicamento
  - resultados de quiz
- Branding Universidad Mayor usando logo proporcionado por el usuario.
- Colores sobrios inspirados en identidad universitaria: azul profundo, rojo, dorado y verde.
- Se elimina el banner de piloto/bloqueo por fecha.
- Mantiene:
  - medicamentos completos
  - fichas clínicas
  - calculadora antimicrobianos / otros con concentración máxima
  - KCl
  - sueros hipertónicos
  - PDF descargables
  - PWA instalable
  - Supabase ready

## Cómo subir a GitHub

1. Descomprime este ZIP.
2. Sube todo el contenido a la raíz del repositorio `tabledemedicamentos`.
3. No subas la carpeta completa dentro del repo; el archivo `index.html` debe quedar en la raíz.
4. Revisa `supabase-config.js` y pega tus claves si no están.
5. Ejecuta el contenido de `supabase_setup.sql` en Supabase SQL Editor.
6. Abre la página con `?v=13` para evitar caché.

## Supabase

Ejecuta `supabase_setup.sql`. Este archivo crea/agrega:

- consultas_medicamentos con campos académicos.
- ingresos_academicos.
- comentarios_medicamentos.
- quiz_resultados.

## Importante

No se modificaron las tablas originales de preparación/dilución. Solo se agregó capa académica: perfil, explicación breve, comentarios, quiz y calculadora de bomba cuando hay configuración disponible.
