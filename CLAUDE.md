# Proyecto: Página de Ventas de Servicios Web — origen.ia

## Objetivo
Landing page de ventas de alta conversión para **origen.ia**, una agencia de diseño web
ubicada en Marcos Paz, Buenos Aires. El sitio vende 3 planes web para negocios locales.

## Concepto visual: Naturaleza + Tecnología
El nombre "origen" y la ciudad del árbol (Marcos Paz) definen toda la estética.
La metáfora es un árbol que crece con raíces de circuito PCB: naturaleza orgánica
con estructura digital. Este concepto atraviesa el copy, los nombres de planes,
los íconos, los SVG decorativos y la paleta de color.

## Stack
HTML5 + CSS3 + JavaScript vanilla. Sin frameworks, sin dependencias externas (excepto
Google Fonts vía CDN). Todo el código en un único `index.html`.

---

## Datos del negocio (usar exactamente estos — no inventar)

- **Nombre del negocio:** origen.ia
- **Teléfono / WhatsApp:** 1161436720 → `https://wa.me/541161436720`
- **Instagram:** @origenn.ia → `https://instagram.com/origenn.ia`
- **Ubicación:** Marcos Paz, Buenos Aires, Argentina (servicio en todo el país)
- **Precios:**
  - Plan Semilla (Landing) → $150.000 ARS
  - Plan Raíz (Landing Premium) → $300.000 ARS
  - Plan Bosque (E-commerce) → $500.000 ARS

---

## Diseño y estética — OBLIGATORIO

### Paleta de color
- **Fondo principal:** `#FBFAF4` (papel crema cálido, modo claro)
- **Fondo secundario:** `#F2EFE3` / `#E8E4D2` para secciones alternadas
- **Tinta principal:** `#0E2A1E` (verde oscuro casi negro)
- **Tinta suave:** `#1F3A2C`
- **Verde bosque:** `#2B5D45` (moss, textos secundarios y labels)
- **Verde hoja:** `#2E8B57` (acento principal, hojas del árbol, botones primarios)
- **Teal circuito:** `#2C8B85` (acento tecnológico — raíces PCB, bordes activos)
- **Variante brillante:** `#4ade80` (hover, highlights de hojas)
- **Líneas:** `rgba(14,42,30,0.14)` / fuerte `rgba(14,42,30,0.32)`
- **Muted:** `#5B7165`

Dark mode (toggle disponible): invertir a fondos oscuros `#0B1A12` / `#0E2018`,
verde brillante `#4ade80`, teal `#2dd4bf`.

### Tipografía
- **Serif:** `Instrument Serif` (títulos, manifiestos, precios)
- **Sans:** `Manrope` (cuerpo, labels, navegación)
- **Mono:** `JetBrains Mono` (badges, etiquetas, números de sección)
- Google Fonts con `display=swap`.

### Reglas visuales
- Mobile-first. Responsive en todos los breakpoints (980px y 600px).
- Secciones con padding 100-140px desktop, 60-80px mobile.
- Cards de servicios: fondo papel, borde `1px solid var(--line)`, lift en hover +
  borde verde hoja, esquinas decorativas que aparecen en hover.
- El árbol SVG con raíces estilo PCB es el elemento visual central del hero.
- Separadores de sección: SVG de raíces onduladas (`#roots` symbol).
- Scroll reveal con IntersectionObserver en todos los bloques de contenido.
- Sin colores corporativos azules, sin flat design genérico, sin paleta oscura/neón.

---

## Secciones — ESTRUCTURA ACTUAL DEL SITIO

### NAV
- Logo + nombre `origen.ia` con punto verde.
- Links: Manifiesto, Servicios, Proceso, Trabajos, Preguntas.
- CTA: botón "Empezar proyecto →" → WhatsApp general.
- Toggle dark/dark mode (animación cinematic de cortina + luna/sol).
- Hamburger en mobile.

### 1. HERO (`#top`)
- Número de sección: no aplica (es el hero).
- Árbol SVG animado con raíces PCB a la derecha.
- Partículas flotantes en canvas (fondo sutil).
- H1 serif grande: problema del cliente → solución.
- Subtítulo 1-2 líneas con beneficio directo.
- 2 CTAs: "Quiero mi página →" (WhatsApp) + "Ver precios" (ghost).
- Stats debajo: indicadores de entrega, calidad, cobertura.
- Hint de scroll animado.

### 2. MANIFIESTO (`#manifiesto`)
- Etiqueta: `01 · Manifiesto`
- Grid 2 col: label sticky izquierda + texto largo derecha.
- Texto editorial serif grande: historia del negocio, por qué nació en Marcos Paz,
  qué significa la metáfora del árbol, el problema que resuelven.
- Firma monoespaciada al pie.

### 3. SERVICIOS (`#servicios`)
- Etiqueta: `02 · Servicios`
- 3 cards en grid: Plan Semilla / Plan Raíz / Plan Bosque.
- Plan Raíz es el destacado (`.featured`, fondo tinta, badge "Más elegido").
- Cada card: número, ícono SVG temático, nombre, descripción, lista de incluye,
  precio `$XXX.000 / proyecto`, CTA propio → WhatsApp con texto pre-armado.

  | Plan   | Precio       | Incluye                                                                   |
  |--------|--------------|---------------------------------------------------------------------------|
  | Semilla | $150.000 ARS | 1 página, formulario contacto, mobile, entrega 7 días hábiles            |
  | Raíz   | $300.000 ARS | Hasta 5 secciones, animaciones, SEO on-page, entrega 14 días hábiles     |
  | Bosque | $500.000 ARS | E-commerce completo, MercadoPago, panel gestión, entrega 21 días hábiles |

### 4. PROCESO (`#proceso`)
- Etiqueta: `03 · Proceso`
- 4 pasos en grid horizontal: Sembrar / Enraizar / Ramificar / Florecer.
- Cada paso: número grande decorativo, nombre, descripción, dot animado.
- Metáfora de estaciones para hablar de las etapas del proyecto.

### 5. TRABAJOS (`#trabajos`)
- Etiqueta: `04 · Trabajos`
- Grid asimétrico: caso principal tall izquierda + columna derecha (wide + 2 coming soon).
- Cada trabajo: imagen real del sitio, overlay en hover, nombre, tag de rubro,
  descripción del resultado, link "Ver sitio →".
- Coming soon cards: invitación a contactar.

  **Caso 1 — Vértigo Vapes**
  - URL: `https://vertigovapes.netlify.app`
  - Imagen: archivo local `screenshot-vertigo.jpg` (o thum.io como fallback)
  - Rubro: Vapeadores
  - Resultado: catálogo online 24hs, consultas WhatsApp automáticas.

  **Caso 2 — Pizzería del Amor**
  - URL: `https://pizzeriadelamor.netlify.app`
  - Imagen: archivo local `screenshot-pizzeria.jpg` (o thum.io como fallback)
  - Rubro: Gastronomía
  - Resultado: menú online, clientes nuevos que los encontraron en la web.

  > Si las imágenes locales no existen, usar thum.io:
  > `https://image.thum.io/get/width/800/crop/500/https://[URL]`

### 6. TESTIMONIOS (`#testimonios`)
- Etiqueta: `05 · Testimonios`
- Placeholder mientras no hay testimonios reales: 2 cards con invitación a ser el primero.
- Cuando haya testimonios: quote serif grande + autor con avatar inicial + rol/empresa.

### 7. STRIP CTA (sin id propio)
- Fondo tinta oscura, texto en papel.
- Mensaje de urgencia: cupos limitados por mes.
- CTA principal → WhatsApp.
- 4 datos rápidos: tiempo de respuesta, entrega Semilla, anticipo, zona.

### 8. FAQ (`#faq`)
- Etiqueta: `06 · Preguntas` (o el número que corresponda)
- Acordeón interactivo.
- Preguntas:
  1. ¿En cuánto tiempo entregan la página?
  2. ¿El precio incluye dominio y hosting?
  3. ¿Puedo pedir cambios después de la entrega?
  4. ¿Trabajan con cuotas o planes de pago?
  5. ¿Necesito saber de tecnología para manejar mi web?
  6. ¿Qué diferencia Semilla de Raíz?
  7. ¿Atienden solo en Marcos Paz o también en otras zonas?

### 9. CONTACTO (`#contacto`)
- Etiqueta: `07 · Contacto` (o el número que corresponda)
- Grid 2 col: aside con datos + formulario.
- Formulario envía a WhatsApp con los datos precargados.
- Datos: WhatsApp, Instagram @origenn.ia, Estudio Marcos Paz, Horario Lun–Sáb 9-20h.

### 10. FOOTER
- Logo + descripción corta.
- Columnas: Estudio, Servicios, Hablemos.
- Copyline: `© 2026 origen.ia — Marcos Paz, Buenos Aires`
- Sin mapa, sin newsletter, sin links muertos.

---

## WhatsApp links

```
https://wa.me/541161436720?text=[MENSAJE]
```

| Destino       | Texto pre-armado                                      |
|---------------|-------------------------------------------------------|
| Plan Semilla  | `Hola%2C+quiero+info+sobre+el+plan+Semilla`          |
| Plan Raíz     | `Hola%2C+quiero+info+sobre+el+plan+Ra%C3%ADz`        |
| Plan Bosque   | `Hola%2C+quiero+info+sobre+el+plan+Bosque`           |
| General       | `Hola%2C+quiero+una+p%C3%A1gina+web+para+mi+negocio` |
| Disponibilidad| `Hola%2C+quiero+saber+si+tienen+lugar+este+mes`      |

---

## Copywriting — REGLAS DURAS

- Tono: directo, confiable, sin exagerar. Como el mejor vendedor del barrio.
- La metáfora del árbol/naturaleza se usa en el copy pero sin forzarla ni abusar.
- El dolor antes de la solución: nombrar el problema antes de ofrecer la respuesta.
- Verbos de acción en CTAs: "Quiero mi página", "Empezar Semilla", "Hablar con un asesor".
- No usar: "soluciones integrales", "equipo de expertos", "compromiso con la calidad".
- Cero texto genérico. Cada línea habla del cliente, su negocio, su zona.

---

## Animaciones

- Hero: fade+slide en entrada, árbol SVG con stroke-dashoffset animado (draw-on),
  hojas con `leafPop` (scale desde 0), partículas canvas flotantes.
- Dark mode: transición cinematic de cortina con clip-path + estrellas/luna o sol.
- Cards servicios: hover lift + borde verde + esquinas decorativas.
- Proceso: dot animado + número con fade al hacer scroll.
- Secciones: scroll-reveal con IntersectionObserver + stagger en grids.
- FAQ: acordeón con stagger reveal + max-height transition.
- Sin librerías de animación externas. CSS animations + JS vanilla puro.

---

## SEO

- Meta title: incluir "páginas web", "Marcos Paz", "Buenos Aires".
- Meta description orientada a conversión.
- Un solo H1 en el hero, headings semánticos en el resto.
- Alt text en todas las imágenes.
- Schema markup `LocalBusiness` con los datos del negocio.
- OG tags y Twitter Card completos.
- Canonical URL: actualizar cuando el dominio esté activo.

---

## Performance

- Imágenes locales en JPG/WebP con `loading="lazy"` y dimensiones explícitas.
- Google Fonts con `display=swap` y `preconnect`.
- CSS crítico inline (todo el CSS está en el mismo archivo HTML).
- Sin JavaScript bloqueante en el `<head>`.
- Target: Lighthouse ≥ 90 en mobile.

---

## Bugs conocidos a corregir

1. **Contadores hero**: el JS sobreescribe las stats con números que no coinciden
   con los labels. Corregir o eliminar el countUp.
2. **Numeración duplicada**: Trabajos y Testimonios usan el mismo número "04 ·".
   Ajustar la secuencia: Trabajos 04, Testimonios 05, Strip sin número, FAQ 06, Contacto 07.
3. **Imágenes de trabajos**: verificar que `screenshot-vertigo.jpg` y
   `screenshot-pizzeria.jpg` existan. Si no, cambiar a URLs thum.io.
