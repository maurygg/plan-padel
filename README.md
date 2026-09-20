# Plan Pádel

App de seguimiento del plan de preparación física para pádel (12 semanas, Prof. Martín Ferreras).

Un solo archivo HTML sin dependencias: `docs/index.html`. Los registros de entrenamiento se guardan
en el navegador de cada persona (localStorage) — no hay servidor ni base de datos.

El botón **Copiar link para Martín** genera una URL que lleva el informe comprimido en el fragmento
(`#r=...`): quien la abre ve ese informe en solo lectura, sin que se toquen sus propios datos.
