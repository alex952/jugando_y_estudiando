# Jugando y estudiando

Pequeñas aplicaciones web estáticas (HTML + CSS + JS, sin dependencias) para repasar con los niños.

## Estructura

```
index.html            # portada que lista las apps
apps.json             # catálogo de apps (la portada lo lee)
apps/<nombre>/        # una carpeta por app, con su index.html
```

## Añadir una app nueva

1. Crea `apps/<nombre>/index.html` (autocontenida).
2. Añade una entrada en `apps.json` (`folder`, `title`, `emoji`, `description`, `topic`).
3. Haz commit y push: GitHub Pages se actualiza solo.

## Publicar con GitHub Pages

Settings → Pages → *Deploy from a branch* → rama `main`, carpeta `/ (root)`.

## Probar en local

`python3 -m http.server` y abrir http://localhost:8000 (hace falta servidor por el `fetch` de `apps.json`).

## Apps

- **Dados de multiplicar** — tira dos dados y multiplica.
