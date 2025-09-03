# Batabit (Práctica Mobile First & Responsive Design)

Proyecto estático realizado como práctica del curso de Platzi sobre Mobile First y Responsive Design. El objetivo es construir una landing page responsive optimizada desde mobile hacia desktop, aplicando buenas prácticas de layout, escalabilidad visual y accesibilidad básica.

## Tecnologías
- HTML5: [index.html](index.html)
- CSS (arquitectura simple por breakpoint):
  - Mobile First: [CSS/mobile.css](CSS/mobile.css)
  - Tablet ≥768px: [CSS/tablet.css](CSS/tablet.css)
  - Desktop ≥1024px: [CSS/desktop.css](CSS/desktop.css)
- Fuente: Google Fonts (DM Sans)
- Sin JS (enfoque en maquetación responsive)

## Estrategia Responsive
- Enfoque Mobile First (estilos base en [CSS/mobile.css](CSS/mobile.css))
- Mejora progresiva con media queries min-width: 768px (tablet), 1024px (desktop)
- Uso de unidades relativas (clamp(), %, flex, grid) para escalabilidad
- Tokenización con variables CSS (colors, spacing, radii, shadows, tipografía)

## Secciones Principales
1. Hero (branding, mensaje y CTA flotante anclado visualmente entre header y main)
2. Tasas de cambio (scroll horizontal en mobile con cards: monedas y comisiones)
3. Value Proposition (sección oscura + icono flotante superpuesto)
4. Promo Banner (imagen de fondo con overlay y degradado adaptativo)
5. Pricing (scroll horizontal en mobile; destacada tarjeta “Recomendado”)
6. Footer (navegación secundaria + branding)

## Patrones Implementados
- Scroll horizontal con snap en listas: tasas y pricing
- Grid y Flex combinados según contexto
- Uso de clamp() para tamaños fluidos (ej. badge e imagen decorativa)
- Badges y elementos destacados usando posicionamiento absoluto no intrusivo

## Accesibilidad
- Etiquetas semánticas: header, main, section, footer, nav, figure, time
- Texto descriptivo en imágenes significativas; alt vacío en decorativas
- Uso de aria-label / aria-labelledby en listas de tarjetas
- Enlaces y botones con estados hover/focus visibles
- Preferencia de movimiento respetada: @media (prefers-reduced-motion: reduce)

## Rendimiento y Buenas Prácticas
- Fuente cargada con preconnect
- Imágenes SVG para íconos (ligeras y escalables)
- Separación por breakpoints evita sobreescrituras excesivas
- No se incluye JS innecesario

## Cómo Ver el Proyecto
Opciones:
1. Abrir directamente: doble clic en [index.html](index.html)
2. Usar extensión Live Server (configurado puerto 5501 en [.vscode/settings.json](.vscode/settings.json))
3. Servir con un servidor simple:

## Posibles Mejoras Futuras
- Integrar datos reales vía API (criptos y comisiones)
- Modo oscuro automático (prefers-color-scheme)
- Optimización de imágenes (versiones AVIF/WebP)
- Tests visuales (regresión) y linting CSS
- Automatizar build (minificación + postcss)

## Licencia
Uso educativo. Archivo base: [package.json](package.json) con licencia ISC.

## Autoría
Práctica formativa basada en lineamientos del curso de Platzi. Adaptable
