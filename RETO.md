# Reto · Página de catas `eventos.html` (5.0)

Café Altamira organiza catas de café y necesita una página para anunciarlas e
inscribir a los asistentes. Créala **desde cero** en `eventos.html`, reutilizando
`css/estilos.css`. El verificador **no** revisa esta página: tú escribes tu propia
lista de verificación y demuestras que se cumple.

## Lo que debe tener la página

1. Mismo encabezado y navegación que `index.html` (con un enlace a `eventos.html`
   en las dos páginas y `aria-current="page"` en el de la página actual), enlace
   "Saltar al contenido", `<main>` y `<footer>`.
2. Un único `<h1>` y encabezados sin saltos de nivel.
3. **3 catas** como `<article>`, cada una con `<h3>`, una fecha en
   `<time datetime="2026-11-20T16:00">`, cupos y precio.
4. Un **formulario de inscripción** con:
   - nombre y correo con `<label>` asociado y `required`;
   - la cata elegida como grupo de `radio` dentro de `<fieldset>` con `<legend>`;
   - una casilla "Acepto el tratamiento de datos" (`checkbox` con su `label`);
   - `<button type="submit">`.
5. Al menos una imagen con `alt` descriptivo y una decorativa con `alt=""`.

## Lo que debes entregar

- `eventos.html` funcionando y enlazada desde `index.html`.
- En este mismo archivo, debajo de **Mi lista de verificación**, escribe **5 o más**
  verificaciones propias con el formato Dado / cuando / entonces y marca `[x]` las
  que comprobaste. Ejemplo:
  `- [x] Dado que estoy en el formulario, cuando presiono Tab, entonces paso por nombre, correo, cada cata y el botón, en ese orden.`
- Captura de Lighthouse (pestaña Accesibilidad) de `eventos.html` con **90 o más**,
  guardada como `evidencias/lighthouse-eventos.png`.
- `node verificar.js` sigue en 40/40 (no rompiste lo guiado).

## Rúbrica

| Criterio | Valor |
|---|---|
| Estructura semántica: landmarks, h1 único, orden de encabezados, `article` + `time` | 1.5 |
| Formulario accesible: labels, `fieldset`/`legend`, `required`, botón real, uso con teclado | 1.5 |
| Lista de verificación propia (5+, Dado/cuando/entonces) y captura de Lighthouse ≥ 90 | 1.0 |
| `index.html` sigue en 40/40 y la navegación entre páginas funciona | 1.0 |
| **Total** | **5.0** |

---

## Mi lista de verificación

- [x] Dado que la página está abierta, cuando reviso el idioma y el título del documento, entonces confirmo que está en español y tiene un título descriptivo.
- [x] Dado que la página contiene imágenes, cuando reviso sus atributos, entonces confirmo que tienen textos alternativos descriptivos.
- [x] Dado que navego por la página con el teclado, cuando avanzo entre sus elementos interactivos, entonces puedo identificar el foco y acceder al enlace para saltar al contenido.
- [x] Dado que estoy en el catálogo, cuando reviso su estructura, entonces encuentro un encabezado y tres productos organizados en artículos.
- [x] Dado que estoy en el formulario de suscripción, cuando reviso el campo de correo, entonces encuentro una etiqueta asociada y el campo está marcado como obligatorio.
- [x] Dado que llego al pie de página, cuando reviso la información de contacto, entonces encuentro la dirección, el teléfono y el horario.
- [x] Dado que ejecuto Lighthouse en `http://localhost:3000`, cuando termina el análisis, entonces obtengo 100 en rendimiento, accesibilidad, buenas prácticas y SEO.