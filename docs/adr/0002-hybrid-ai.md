# ADR 0002: IA híbrida (audio on-device + LLM en nube)

## Status
Accepted

## Context
El MVP usa IA para cuatro cosas: evaluar el audio en tiempo real, tutor conversacional, generación de contenido y progresión adaptativa. Hay que decidir dónde se ejecuta cada una, considerando latencia, privacidad, coste y que el MVP no tiene backend propio.

## Decision
Ejecutar la detección de audio en el dispositivo (on-device) y el tutor, la generación de contenido y la progresión adaptativa mediante una API de LLM en la nube.

## Alternatives Considered
- **Todo on-device:** privacidad y sin coste por uso, pero los modelos pequeños limitan la calidad del tutor y la generación.
- **Todo en nube:** mayor calidad, pero la detección en tiempo real sufre latencia y depende de la conexión, justo lo crítico para el feedback.
- **Sin IA generativa en el MVP:** reduce alcance y coste, pero elimina diferenciadores pedidos explícitamente.

## Consequences
- El feedback en tiempo real no depende de internet.
- El tutor y la generación requieren conexión y generan coste por tokens.
- Hay que resolver la distribución de la clave del LLM sin backend propio (ver riesgos).
- La progresión adaptativa funciona solo con conexión en el MVP.
