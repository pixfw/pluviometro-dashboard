# pluviometro-dashboard

Dashboard estático (HTML + Chart.js) que muestra los datos del pluviómetro
consumiendo la API del Worker (`pluviometro-worker`).

## Configuración
Antes de desplegar, edita `config.js` con la URL real de tu Worker:

```js
const API_BASE = "https://pluviometro-worker.TU-SUBDOMINIO.workers.dev";
```

## Desplegar en Cloudflare Pages
1. En el dashboard de Cloudflare → Workers & Pages → Create → Pages →
   conecta este repositorio.
2. Framework preset: **None**.
3. Build command: (vacío, es estático).
4. Build output directory: `/` (la raíz del repo).
5. Deploy.

Cada push a la rama principal republicará el sitio automáticamente.
