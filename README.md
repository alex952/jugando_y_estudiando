# Jugando y estudiando

Pequeñas aplicaciones web estáticas (HTML + CSS + JS, sin dependencias) para repasar con los niños.

## Estructura

```
index.html            # portada: secciones por asignatura y filtros por etiqueta
apps.json             # catálogo de apps (la portada lo lee)
apps/<nombre>/        # una carpeta por app, con su index.html
```

## Añadir una app nueva

1. Crea `apps/<nombre>/index.html` (autocontenida).
2. Añade una entrada en `apps.json`:

   ```json
   {
     "folder": "nombre",
     "title": "Título",
     "emoji": "🧩",
     "description": "Una frase.",
     "topic": "Matemáticas",
     "tags": ["Etiqueta1", "Etiqueta2"]
   }
   ```

   `topic` define la **sección** de la portada (se crea sola si es nueva, p. ej. «Lengua» o «Inglés»);
   `tags` son las etiquetas por las que se puede filtrar.
3. Haz commit y push: GitHub Pages se actualiza solo.

## Publicar con GitHub Pages

Settings → Pages → *Deploy from a branch* → rama `main`, carpeta `/ (root)`.

## Probar en local

`python3 -m http.server` y abrir http://localhost:8000 (hace falta servidor por el `fetch` de `apps.json`).

## Apps

- **Dados de multiplicar** — tira dos dados y multiplica.
- **Sumas y restas paso a paso** — columnas con o sin llevadas, de 2 a 4 cifras; modo guiado o «yo solo».
- **Tablas con cronómetro** — elige las tablas; 60 segundos o 10 preguntas, repaso de fallos y récord.
- **Mi tabla** — ver una tabla o completarla: entera o con huecos, en orden o desordenada.
- **Fracciones** — leer, pintar, comparar y fracción de un número.
