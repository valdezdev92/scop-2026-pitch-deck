# Proyectos SCOP 2026 — Panorama de Obra Pública

Presentación web independiente (22 diapositivas a pantalla completa) sobre los
**Proyectos SCOP 2026** del Gobierno del Estado de Chihuahua. El núcleo del deck son
las **9 obras de infraestructura vial** —6 pasos a desnivel en Chihuahua capital y
3 en Ciudad Juárez—, cada una con su propia slide (imagen, datos técnicos, impacto y
estatus). Después se presenta el resto de la cartera (espacios públicos, conectividad,
infraestructura social, auxilio carretero). Estética dark-mode premium (estilo
Linear / Stripe) con acento cian/teal e identidad técnica de ingeniería.

> No modifica la presentación original (`../presentacion.html`). Es un proyecto en paralelo.

## Cómo abrirla

Abre **`index.html`** directamente en cualquier navegador (doble clic). No requiere
servidor ni instalación. Funciona en laptop, proyector e iPad.

> Si abres con `file://` y alguna imagen no cargara, sirve la carpeta con un
> servidor estático simple:
> ```bash
> cd pitch-deck
> python3 -m http.server 8000   # luego visita http://localhost:8000
> ```

## Cómo navegar

| Acción | Control |
|--------|---------|
| Avanzar | `→` · `↓` · `Espacio` · rueda del ratón · botón ❯ · swipe izquierda (iPad) |
| Retroceder | `←` · `↑` · rueda hacia arriba · botón ❮ · swipe derecha |
| Ir al inicio / fin | `Home` / `End` |
| Saltar a una sección | clic en los puntos inferiores |

Arriba a la derecha hay un indicador de progreso (`03 / 10`) y una barra superior.

## Las 22 diapositivas

**Apertura**
1. **Portada** — "Nueve obras que mueven a Chihuahua".
2. **Visión general** — "No es solo infraestructura, es calidad de vida" + los 6 ejes.

**Los 6 pasos a desnivel de Chihuahua (uno por slide)**
3. **Intro Puentes Chihuahua** — Estrategia por zonas: Oriente, Norte, Suroeste.
4. **Paso 01 — Fuerza Aérea / Palestina** (Superior · +$280 M · +20,000 veh.).
5. **Paso 02 — Juan Pablo II / Quinta Real** (Superior · +$160 M · +15,000 veh.).
6. **Paso 03 — Tecnológico / Los Arcos** (Inferior · $183.6 M · +43,000 veh.).
7. **Paso 04 — Tecnológico / Av. Desarrollo** (Superior · $200.7 M · +35,000 veh.).
8. **Paso 05 — Tecnológico / G. Prieto Luján** (Superior · $200.7 M · +40,000 veh.).
9. **Paso 06 — Silvestre Terrazas / Calle 120** (Inferior · $126 M · +12,000 veh.).

**Vialidad estratégica de Chihuahua**
10. **Prolongación Av. Teófilo Borunda — Labor de Terrazas** (+2 km · +$17 M).

**Los 3 pasos a desnivel de Ciudad Juárez (uno por slide)**
11. **Intro Ciudad Juárez** — 3 pasos sobre Av. Las Torres ($420 M, BRT 4).
12. **Juárez Paso 01 — Talamás Camandari** ($180 M · Jul 2026–Feb 2027).
13. **Juárez Paso 02 — Tomás Fernández** ($120 M · Sep 2026–Jun 2027).
14. **Juárez Paso 03 — Valle del Sol** ($120 M · Sep 2026–Mar 2027).

**Información complementaria de los documentos**
15. **Juárez · inversión histórica** — +$1,754 M global, BRT II, +30 calles, El Mezquital.
16. **Juárez · obras en proceso y conservación** — proceso + bacheo + calles + 7 parques.
17. **Espacios públicos** — Unidad Deportiva "Pistolas Meneses" + parques (Chihuahua).
18. **Vialidades estratégicas** — Periférico de la Juventud (+33,000 m²).
19. **Conectividad regional** — Puentes regionales, corredores y mantenimiento.
20. **Infraestructura social** — Salud (hospitales) + cultura/gobierno.
21. **Auxilio Carretero** — Operativo Semana Santa 2026: 56 rescates, sin costo.
22. **Momento actual / Cierre** — Tres frentes simultáneos + cita institucional.

> **Fuentes:** Guion General de Entrevista, Cartera de Obras y Ficha Informativa
> de Ciudad Juárez (SCOP 2026). El estatus de los puentes de Chihuahua refleja la
> etapa del guion (licitación / proceso / cartera).

## Cómo editar el contenido

- **Textos:** edita directamente el HTML. Cada slide está marcada con un comentario
  `<!-- ===== NN · NOMBRE ===== -->` para ubicarla rápido.
- **Colores / tipografía:** todo vive en las variables CSS dentro de `:root`
  (al inicio del `<style>`). Cambia `--teal` para mover el acento de toda la
  presentación, o `--bg` para el fondo.
- **Imágenes:** están en `assets/` con nombres `pN-render.*` (render aéreo) y
  `pN-tec.*` (diseño técnico). Sustituye un archivo manteniendo el nombre para
  reemplazar la imagen sin tocar el código.
- **Cifras de la tabla / KPIs:** son texto plano en las slides 7 y 9; edítalas ahí.

## Estructura

```
pitch-deck/
├── index.html      # presentación completa (CSS + JS inline, sin dependencias)
├── README.md       # este archivo
└── assets/         # 15 imágenes de las obras
```
