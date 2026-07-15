# Diseño: Web "Reflexiones sobre la muerte y resumen de las leyes de Avelut (duelo)"

**Fecha:** 2026-07-15
**Estado:** Aprobado por el usuario

## Propósito

Digitalizar el folleto físico del Rabinato de la Comunidad Judía de Madrid
("Reflexiones sobre la muerte y resumen de las leyes de Avelut (duelo)", del
Rab. Moshé Bendahan) como una página web compartible con los familiares de los
fallecidos. El usuario confirma que cuenta con autorización para difundirlo.

## Requisitos

1. **Fidelidad absoluta al original.** Transcripción literal de las 25 fotos
   (portada, índice, páginas 1–22, contraportada). No se inventa ni añade
   información. Se respetan la convención "D-s" y las transliteraciones tal
   como aparecen. Cualquier palabra ilegible se consulta al usuario, no se
   supone.
2. **Sin datos añadidos.** No se incluyen contactos ni contenido que no esté
   en las fotos. Créditos y autoría, tal como figuran en el folleto.
3. **Una sola página** con el índice original como menú de navegación por
   anclas.
4. **Publicación** en GitHub Pages, repo público `leyes-de-avelut` de la
   cuenta `alanmo1910`.

## Solución técnica

- Un único `index.html` estático con CSS embebido; sin frameworks ni build.
- JavaScript mínimo opcional (botón "volver al índice"). Funciona sin JS.
- `lang="es"`, HTML semántico (`nav`, `section`, jerarquía de encabezados).
- Estética sobria: fondo crema, tipografía serif, sin imágenes decorativas.
  Media query de impresión.
- Estructura del contenido: portada → índice navegable → Primera parte
  (4 secciones de reflexión) → Segunda parte (leyes en listas numeradas) →
  oraciones del aniversario → pie con el crédito de la contraportada.

## Flujo de trabajo

1. Enderezar las fotos HEIC (sips) y releerlas a alta resolución.
2. Transcribir página a página; marcar dudas para consulta.
3. Componer `index.html`; revisar contra las fotos.
4. Crear repo público, push, activar GitHub Pages, verificar URL en vivo.

## Fuera de alcance

Buscadores internos, varias páginas, otros idiomas, formularios, analítica.
