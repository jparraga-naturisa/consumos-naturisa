# Consumos Naturisa

Dashboards de consumos de Naturisa, publicados con GitHub Pages:

- **Consumos Insumos** — `consumos-insumos/consumos-insumos.html`
- **Consumos Combustible** — `consumos-combustible/consumos-combustible.html`

Se cambia de uno a otro con el selector de la barra superior. Cada dashboard sube y lee su propio Excel (tablas `consumo_insumos` y `consumo_combustible` en D1, vía el worker `naturisa-proxy`).

## Correr en local

Requiere Python 3. Ejecutar el `.bat` de cada carpeta (o `python comun/server.py consumos-insumos/consumos-insumos.html 3001`). El servidor local hace de proxy hacia el worker y el gateway, y sirve los demás archivos del repositorio para que el selector de app funcione.
