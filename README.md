# presupuestos

Presupuestos comerciales de Nova Domus, publicados con GitHub Pages en
`https://novadomus-cba.github.io/presupuestos/`.

| Ruta | Qué es | URL |
|---|---|---|
| `index.html` | Página pública de cualquier presupuesto del panel comercial | `/presupuestos/?id={ID}` |
| `pc-AAAA-NNN/index.html` | Presupuesto con HTML propio | `/presupuestos/pc-AAAA-NNN/` |
| `assets/` | Logo y recursos compartidos | — |

## Cómo se publica un PC con HTML propio

1. Una carpeta por presupuesto, en minúsculas: `pc-AAAA-NNN/index.html`, un solo archivo con todo
   embebido y el número `PC-AAAA-NNN` visible en el encabezado.
2. Agustín publica directo en `main`. El resto del equipo trabaja en una rama `pc/AAAA-NNN` y abre
   un pull request; `main` está protegido y lo aprueba Agustín.
3. Un PR de un PC no toca `index.html` ni `assets/`: son la página de todos los links de cliente.
4. Antes de mandar el link: build de Pages en `built` y la URL abierta mostrando el número.
5. Sin tokens: se publica con la app Claude o con el login propio en Claude Code. Si no se puede
   pushear, se para y se avisa.

Este repo es **público**: nada de costos, márgenes, comisiones ni proveedores en archivos, commits
o pull requests.

Los links emitidos antes del 19/11/2026 apuntan a `novadomuscba.github.io/presupuestos/`, que
redirige acá conservando ruta, `?id=` y `#`.
