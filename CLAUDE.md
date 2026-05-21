# Proyecto: Página de Ventas de Servicios Web

## Objetivo
Construir una landing page de ventas de alta conversión para una agencia de diseño web
ubicada en Zona Oeste, Buenos Aires. El sitio vende 3 servicios: Landing Page, Landing
Premium y E-commerce.

## Stack
HTML5 + CSS3 + JavaScript vanilla. Sin frameworks, sin dependencias externas (excepto
fuentes de Google Fonts e íconos de Lucide o similar vía CDN).

## Workflow de construcción — SEGUIR EN ESTE ORDEN

1. Invocar `/frontend-design` para construir la estructura HTML/CSS/JS completa.
2. Invocar `/animate` para agregar animaciones y micro-interacciones.
3. Invocar `/skill-creator:seo-audit` para optimizar el SEO on-page.
4. Invocar `/skill-creator:web-performance-audit` para auditar y corregir performance.

No saltear pasos. Cada skill construye sobre el resultado del anterior.

---

## Datos del negocio (usar exactamente estos — no inventar)

- **Nombre del negocio:** Black Rose IA
- **Teléfono / WhatsApp:** 1161436720
- **Instagram:** [INSTAGRAM] ← reemplazar cuando el usuario lo defina
- **Ubicación:** Zona Oeste, Buenos Aires, Argentina
- **Precios:**
  - Landing Page → $150.000 ARS
  - Landing Premium → $300.000 ARS
  - E-commerce → $500.000 ARS

---

## Diseño y estética — OBLIGATORIO

- Paleta: fondo negro profundo `#080808` o `#0a0a0a`. Acentos metálicos/eléctricos:
  plateado `#c0c0c0` / `#e8e8e8` con destellos blancos `#ffffff`, y un acento
  eléctrico secundario en cian eléctrico `#00e5ff` o violeta neón `#a855f7` para
  highlights, borders activos y glows — nunca como color de fondo.
- Efecto metálico en textos clave: gradiente `linear-gradient(135deg, #c0c0c0, #ffffff, #a0a0a0)`
  con `background-clip: text` para títulos principales.
- Tipografía: sans-serif moderna — `Inter`, `Syne` o `Space Grotesk` (Google Fonts).
- Espaciado ajustado y denso: secciones compactas, padding reducido, que transmita
  energía y densidad de información — no diseño "aireado" de agencia genérica.
  Usar padding vertical de secciones de 60-80px max en desktop, no 120px+.
- Mobile-first. Responsive en todos los breakpoints.
- Glassmorphism sutil o bordes con glow metálico/eléctrico para las cards de servicios.
- Ningún color pastel, beige, crema ni tono corporativo.

---

## Secciones — ESTRUCTURA OBLIGATORIA

### 1. HERO
- Ocupa 100vh.
- Titular impactante orientado a la venta: el problema del cliente + la solución.
  Ejemplo de tono: "Tu negocio necesita una presencia online que venda, no una
  página que exista." — NO usar este ejemplo textualmente, crear algo original.
- Subtítulo: 1-2 líneas que refuercen el beneficio inmediato.
- 2 CTAs: primario ("Quiero mi página" → WhatsApp) y secundario ("Ver servicios").
- Elemento visual de fondo: gradiente animado, partículas o grid futurista — algo
  que dé profundidad sin tapar el texto.
- Badge o prueba social pequeña cerca del CTA ("Ya confiaron en nosotros X negocios
  de zona oeste" — adaptar al dato real cuando el usuario lo provea).

### 2. POR QUÉ TENER UNA PÁGINA WEB (beneficios reales)
- Título de sección fuerte, no genérico.
- 4-6 beneficios concretos orientados al dueño de negocio de zona oeste/AMBA:
  presencia 24/7, más ventas, credibilidad frente a la competencia, alcance más
  allá del barrio, automatizar consultas. Sin frases tipo "mejora tu presencia
  digital" — ir al hueso: cuánto pierde sin página, qué gana con una.
- Formato: grid de cards con ícono + título + descripción corta.

### 3. SERVICIOS
Tres cards en formato comparativo o grid:

| Servicio        | Precio          | Incluye                                                                             |
|-----------------|-----------------|-------------------------------------------------------------------------------------|
| Landing Page    | $150.000 ARS    | 1 página, secciones básicas, formulario de contacto, adaptación mobile              |
| Landing Premium | $300.000 ARS    | Todo lo anterior + animaciones avanzadas, SEO on-page, hasta 5 secciones custom    |
| E-commerce      | $500.000 ARS    | Tienda online completa, carrito, pasarela de pago, panel de gestión                 |

- Cada card con un CTA propio → WhatsApp con mensaje pre-armado por servicio.
- Marcar visualmente cuál es el más elegido (badge "Popular" en Landing Premium).
- NO poner "Precio a consultar" — los precios van claros.

### 4. CASOS DE ÉXITO
- Título: "Negocios que ya confían en nosotros" o equivalente.
- Formato: cards con imagen de preview del sitio real, nombre del negocio, rubro
  y un resultado concreto/descripción. Cada card incluye un botón "Ver sitio" que
  abre el link en nueva pestaña.
- Para las imágenes de preview usar el servicio thum.io (sin API key, gratuito):
  ```
  https://image.thum.io/get/width/800/crop/500/https://[URL-DEL-SITIO]
  ```
- Casos reales:

  **Caso 1 — Vértigo Vapes**
  - URL: https://vertigovapes.netlify.app
  - Imagen: `https://image.thum.io/get/width/800/crop/500/https://vertigovapes.netlify.app`
  - Rubro: Venta de vaporizadores
  - Descripción breve orientada al resultado: algo concreto sobre presencia online,
    consultas por WhatsApp, o visibilidad local — redactar en tono vendedor.

  **Caso 2 — Pizzería del Amor**
  - URL: https://pizzeriadelamor.netlify.app
  - Imagen: `https://image.thum.io/get/width/800/crop/500/https://pizzeriadelamor.netlify.app`
  - Rubro: Gastronomía / pizzería
  - Descripción breve orientada al resultado: pedidos online, presencia en zona,
    diferenciación frente a la competencia — redactar en tono vendedor.

- Las imágenes deben tener bordes redondeados, overlay sutil al hover, y el estilo
  dark/metálico del resto del sitio (frame o borde con glow).
- Botón "Ver sitio →" en cada card con `target="_blank" rel="noopener"`.

### 5. PREGUNTAS FRECUENTES (FAQ)
Acordeón interactivo. Incluir estas preguntas con respuestas en tono directo, sin jerga técnica:

1. ¿En cuánto tiempo entregan la página?
2. ¿El precio incluye dominio y hosting?
3. ¿Puedo pedir cambios después de la entrega?
4. ¿Trabajan con cuotas o planes de pago?
5. ¿Necesito saber de tecnología para manejar mi página?
6. ¿Qué diferencia hay entre la Landing y la Landing Premium?
7. ¿Atienden solo en zona oeste o también otras zonas?

### 6. CTA FINAL / CONTACTO
- Sección de cierre antes del footer.
- Mensaje de urgencia o escasez real ("Cupos limitados por mes" o similar).
- Botón grande → WhatsApp directo al 1161436720.
- Link a Instagram → [INSTAGRAM].

### 7. FOOTER
- **Black Rose IA** — teléfono 1161436720 — Instagram [INSTAGRAM].
- Zona Oeste, Buenos Aires.
- Año actual.
- Sin bloat: sin mapa, sin newsletter, sin links muertos.

---

## Copywriting — REGLAS DURAS

- Cero texto genérico. Cada línea debe hablar del cliente, su negocio, su zona.
- Tono: directo, confiable, sin exagerar. Como el mejor vendedor del barrio, no
  como una multinacional.
- El dolor antes de la solución: nombrar el problema que tiene el lector antes de
  ofrecer lo que vendemos.
- Verbos de acción en los CTAs: "Quiero mi página", "Hablar con un asesor",
  "Ver precios", "Empezar ahora".
- No usar: "soluciones integrales", "equipo de expertos", "compromiso con la
  calidad", ni ningún cliché de agencia.

---

## WhatsApp links

Usar este formato para todos los CTAs:

```
https://wa.me/541161436720?text=[MENSAJE_PREARMADO]
```

Mensajes por servicio:
- Landing:    `Hola%2C+quiero+info+sobre+la+Landing+Page`
- Premium:    `Hola%2C+quiero+info+sobre+la+Landing+Premium`
- E-commerce: `Hola%2C+quiero+info+sobre+el+E-commerce`
- General:    `Hola%2C+quiero+una+p%C3%A1gina+web+para+mi+negocio`

---

## Animaciones (guía para /animate)

- Hero: entrada con fade+slide del texto, loop sutil en el fondo.
- Cards de servicios: hover con lift + glow del borde metálico.
- Secciones: scroll-reveal con IntersectionObserver — nada que bloquee el render.
- FAQ: acordeón con transición suave (max-height o transform).
- Sin librerías de animación >50kb. CSS animations + JS vanilla.

---

## SEO (guía para /skill-creator:seo-audit)

- Meta title: incluir "páginas web", "zona oeste", "Buenos Aires".
- Meta description orientada a conversión, no a descripción.
- Un solo H1 en el hero, headings semánticos en el resto.
- Alt text en todas las imágenes.
- Schema markup `LocalBusiness` con los datos del negocio.
- OG tags completos para compartir en redes.

---

## Performance (guía para /skill-creator:web-performance-audit)

- Imágenes en WebP o reemplazar con SVG/gradientes cuando sea posible.
- Google Fonts con `display=swap`.
- CSS crítico inline para el above-the-fold.
- Sin JavaScript bloqueante en el `<head>`.
- Target: Lighthouse ≥ 90 en mobile.
