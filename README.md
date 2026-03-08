# Para-Milvia

## Desarrollo local

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Compartir el link (GitHub Pages)

### Opción A: URL normal de GitHub Pages

Si no usas dominio personalizado, comparte:

`https://<usuario>.github.io/Para-Milvia/`

Para ese caso, construye con base de subcarpeta:

```bash
VITE_BASE_PATH=/Para-Milvia/ npm run build
```

### Opción B: Dominio personalizado (ejemplo: `milvia.regalo`)

Si usas dominio personalizado, comparte:

`https://milvia.regalo`

Para ese caso, construye con base raíz:

```bash
VITE_BASE_PATH=/ npm run build
```

Además, en GitHub Pages:

1. En **Settings → Pages → Custom domain**, coloca `milvia.regalo`.
2. Crea/ajusta DNS en tu proveedor:
   - `A` del dominio raíz (`@`) a los IPs de GitHub Pages.
   - `CNAME` para `www` apuntando a `<usuario>.github.io`.
3. Espera propagación DNS (puede tardar minutos u horas).
4. Activa **Enforce HTTPS** cuando deje de salir "Unavailable".

> Si dejas configurado dominio personalizado, no compartas el link `github.io/Para-Milvia/`; comparte solo tu dominio.
