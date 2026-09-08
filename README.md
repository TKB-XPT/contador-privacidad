# Política de privacidad — Contador de Snooker y Pool

Repositorio **público** que existe por una sola razón: Google Play exige que la política de
privacidad esté en una **URL pública, activa, no geobloqueada, que no sea un PDF y que no pueda
editar cualquiera**. GitHub Pages sirve páginas sólo de repos públicos, y el código de la app es
privado — de ahí que la política viva acá y no junto al proyecto.

- Página publicada: `index.html` (GitHub Pages, rama `main`, carpeta raíz).
- Esa URL va en Play Console → **Contenido de la app → Política de privacidad**.

## Antes de tocar nada

El mismo texto vive en **tres** lugares y los tres tienen que decir lo mismo:

| Dónde | Qué es |
|---|---|
| `index.html` (este repo) | La versión publicada, la que ve Play |
| `docs/politica-privacidad-contador.md` (repo de la app) | El original en markdown |
| `lib/privacyContent.ts` (repo de la app) | El texto que se muestra **dentro** de la app |

Play exige la política en dos lugares —el campo de Play Console y dentro de la app— así que las
tres versiones son obligatorias, no copias de conveniencia. Si cambia una, cambian las tres, y se
actualiza la fecha en las tres.

Una discrepancia entre la política y el formulario de **Seguridad de los datos** de Play es de las
cosas que se detectan automáticamente y frenan una revisión.

## Cuándo hay que reescribirla entera

Cuando llegue la capa online (cuentas, ranking, perfiles). Ahí la política pasa de "no se recolecta
nada" a un tratamiento real de datos personales, hay que rehacer el formulario de Seguridad de los
datos y publicar además la URL pública de baja de cuenta. La lista completa está en
`docs/PUBLISHING.md` §6 del repo de la app.
