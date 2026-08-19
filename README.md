# CVY26_001 · Project Convoy — hoja de exports

Hoja de specs para el equipo que saca los exports de **Project Convoy** (show code `CVY_026`).

👉 **https://santiagotereso.github.io/convoy-exports/**

Para cada archivo que hay que entregar dice el formato, el nombre exacto y por dónde se sube
(SharePoint o Aspera). Elegís el episodio en el desplegable de arriba y los 11 nombres de archivo
se rearman solos, listos para copiar.

## Qué cubre

| | Sección | Archivos | Canal |
|---|---|---|---|
| 1 | Video | Master ProRes, Textless ProRes, Screener H.264, Screener H.264 con BITC | SharePoint |
| 2 | Gráficos | GFX collect | Aspera |
| 3 | Audio — stems | Full mix, Dialog, M&E, Music, SFX | Aspera |
| 4 | Captions | .SRT | SharePoint |

## Notas

- El time code de los cuatro videos **arranca en 00:00:00:00**, y el BITC del screener tiene que
  coincidir frame a frame con el master.
- `Version` y `LanguageCode` están fijos en `V1` / `ENG`. Si hay que reentregar un episodio
  corregido, avisen y se cambia acá para todos.
- Los tokens subrayados en punteado naranja están deducidos del patrón del Filename Generator de
  Mattel y quedan a confirmar con el cliente. No bloquean el export.
- Los títulos de los 8 episodios salen del
  [convoy_breakdown](https://lucilatr.github.io/convoy-breakdown/convoy_breakdown.html) y están
  fijos en el HTML, así que la página funciona sin internet.

Los contactos nominales de Mattel **no están en esta página**: pedíselos a producción antes del
primer envío.

## Editar

Es un solo `index.html` sin dependencias — se abre con doble click y se edita a mano. Los datos
viven en los arrays `ITEMS` y `SECTIONS` al principio del `<script>`; los títulos de episodio en
`EP_TITLES`. Al pushear a `main`, GitHub Pages republica solo.
