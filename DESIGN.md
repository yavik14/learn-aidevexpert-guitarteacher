---
name: Guitarra con IA
description: App de aprendizaje de guitarra juguetona para adultos sobre una base minimalista, con la tablatura como protagonista.
designAssets:
  sourceOfTruth: []
  generatedConcepts: []
colors:
  primary: "#FF6B35"
  secondary: "#1F6F8B"
  accent: "#F2C94C"
  background: "#FFFFFF"
  surface: "#F5F5F2"
  text: "#1A1A1A"
  success: "#2E9E5B"
  error: "#D64545"
  warning: "#E0A100"
typography:
  h1:
    fontFamily: system-ui
    fontSize: 28
    fontWeight: 700
  h2:
    fontFamily: system-ui
    fontSize: 22
    fontWeight: 700
  body:
    fontFamily: system-ui
    fontSize: 16
    fontWeight: 400
  caption:
    fontFamily: system-ui
    fontSize: 13
    fontWeight: 400
rounded:
  sm: 8
  md: 16
  lg: 24
spacing:
  sm: 8
  md: 16
  lg: 24
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.md}"
  node-available:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.text}"
    rounded: "{rounded.lg}"
  node-completed:
    backgroundColor: "{colors.success}"
    textColor: "#FFFFFF"
    rounded: "{rounded.lg}"
---

# Design Direction

## Overview
Personalidad "juguetona para adultos" sobre una base minimalista. La energía viene del progreso (racha, XP, nodos) y del feedback; el resto de la interfaz se mantiene limpia y sin ruido para centrar la atención en la tablatura y las indicaciones.

## Existing Design Assets
Ninguno. Se parte de cero.

## Generated Concept Images
Ninguna. No se han generado conceptos con IA.

## Product Feel
- Vibrante al celebrar avances, discreta durante la práctica.
- Nunca infantil: sin mascotas ni estética preescolar.
- La tablatura y las indicaciones son el foco visual; el cromo desaparece.

## Colors
- Primario `#FF6B35` (naranja): energía, acción, botones principales.
- Secundario `#1F6F8B` (azul petróleo): elementos informativos y enlaces.
- Acento `#F2C94C` (ámbar): XP, racha y logros.
- Fondos neutros `#FFFFFF` / `#F5F5F2` para el ambiente minimalista.
- Semánticos: verde `#2E9E5B`, rojo `#D64545`, ámbar `#E0A100` para el feedback.

## Typography
Sans-serif del sistema para rendimiento y familiaridad. Jerarquía clara: títulos en negrita, cuerpo legible, captions para metadatos. Números de racha/XP con peso alto.

## Layout
- Márgenes y espaciado generosos (base 8).
- Una acción principal por pantalla.
- Durante el ejercicio, la tablatura ocupa el centro y los controles quedan en la parte inferior.

## Shapes
- Esquinas redondeadas (8/16/24). Los nodos del árbol son formas redondeadas; el estado se distingue por color **y** forma/icono.

## Components
- `button-primary`: acción principal.
- `node`: nodo del árbol en estados bloqueado / disponible / en progreso / completado.
- `streak-chip`: racha y XP en cabecera.
- `exercise-card`: resumen y objetivos de un ejercicio.
- `tablature-grid`: rejilla de tablatura con cursor de tiempo y marcadores de feedback.

## Core Screens
1. **Home / Árbol de habilidades** — nodos, racha, XP.
2. **Afinador** — estado de cada cuerda antes de empezar.
3. **Ejercicio (HUD)** — tablatura, feedback en vivo, tempo.
4. **Resultados** — precisión, XP ganado, errores a reforzar.
5. **Tutor IA** — chat con explicaciones y diagramas.

## Responsive Baseline
- Móvil vertical como referencia principal.
- Adaptable a pantallas grandes y tablets sin cambiar la jerarquía.

## Accessibility Baseline
- Contraste mínimo AA.
- Soporte de tamaño de texto dinámico.
- El feedback no depende solo del color: usar icono/forma además del color.
- Áreas táctiles cómodas (mínimo ~44 pt).

## Do's and Don'ts
- **Do:** hacer visible el progreso; mantener el foco en la tablatura; celebrar sin invadir.
- **Don't:** saturar con animaciones; usar estética infantil; depender solo del color para el feedback; inventar marca o logo.

## Open Design Questions
- Paleta definitiva y modo oscuro.
- Cómo representar visualmente el timing (tarde/temprano) en la tablatura.
- Estilo del tutor (avatar, voz) y cuánto espacio ocupa durante la práctica.
