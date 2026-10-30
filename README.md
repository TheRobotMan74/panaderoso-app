# Recetas Panaderoso

App instalable (PWA) del editor de recetas de Panaderoso. Es una página estática que habla con
el Apps Script de la hoja "Panaderoso Control V2" por su URL `/exec`:

- `GET  /exec?accion=recetas` → `{ ok, datos }` (insumos, productos, recetas, listas)
- `POST /exec` con `{ accion: 'guardarReceta' | 'borrarReceta' | 'agregarInsumo', arg }` → `{ ok, datos }`

La URL `/exec` se pega en la app (botón ⚙️) y solo se guarda en ese aparato; no está en este repo.
