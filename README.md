# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## CI/CD

- `CI`: ejecuta `npm ci`, `npm run check` y `npm run build` en pushes y pull requests.
- `Deploy to GitHub Pages`: publica automaticamente el proyecto en GitHub Pages cuando hay cambios en `main`.

Para GitHub Pages este proyecto usa `@sveltejs/adapter-static` y el workflow de despliegue compila con `BASE_PATH=/actividadcorteIII`.

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
