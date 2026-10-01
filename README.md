# Plan Pádel

App de seguimiento del plan de preparación física para pádel (12 semanas, Prof. Martín Ferreras).

Un solo archivo HTML sin dependencias: `docs/index.html`. Los registros de entrenamiento se guardan
en el navegador de cada persona (localStorage) — no hay servidor ni base de datos.

El botón **Copiar link para Martín** genera una URL que lleva el informe comprimido en el fragmento
(`#r=...`): quien la abre ve ese informe en solo lectura, sin que se toquen sus propios datos.

## Link fijo para Martín (`#informe`)

`#informe` lee `docs/datos.json`. La app lo publica sola (API de GitHub) cada vez que se cierra un
día, la semana o un partido, con un token fine-grained que vive solo en el teléfono de Mauro
(Progreso → Publicar para Martín; permiso Contents: Read and write, solo este repo).

**Ojo al tocar el repo a mano:** la app hace commits a `main`. Antes de cualquier push, `git pull --rebase`.
