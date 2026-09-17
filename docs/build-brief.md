# Build Brief

## Problem
Los principiantes adultos de guitarra abandonan por frustración: no saben si están tocando bien (falta de feedback), el contenido de YouTube es pasivo y la teoría tradicional aburre. Sin corrección ni hábito, dejan de practicar en pocas semanas.

## Current Workaround / Existing System
Vídeos de YouTube y tablaturas/acordes gratuitos. Es gratis y abundante, pero no escucha al usuario, no corrige y no crea hábito. Existen apps con feedback (Yousician, Simply Guitar, Fender Play), pero el usuario objetivo del descubrimiento no las usa.

## Target Users
Principiante adulto sin experiencia previa, motivación de hobby, practica en casa con guitarra acústica y el móvil. Un único practicante local por dispositivo en el MVP.

## Goals
- Dar feedback fiable y en tiempo real de si se toca la nota/acorde correcto.
- Crear hábito diario mediante gamificación (racha, XP, árbol de habilidades).
- Enseñar con tablatura interactiva, sin exigir teoría previa.
- Aportar valor de IA más allá del feedback: tutor, generación de contenido y progresión adaptativa.

## Non-Goals
- Pentagrama (notación estándar) y rutas de género/rol.
- Visión por computadora (postura/técnica).
- Canciones comerciales con licencia.
- Cuentas, sincronización y backend propio.
- Monetización en el MVP.

## MVP Slice
**Tesis:** un principiante adulto practica una lección corta con su guitarra y el móvil hace de profesor: escucha, corrige en tiempo real sobre tablatura y le da una razón para volver mañana.

**Flujo end-to-end:** abrir → afinar → nodo → ejercicio de tablatura con feedback en vivo → la IA ajusta la progresión → recompensa (XP/racha) → tutor.

**Incluye**
- Onboarding mínimo: permiso de micrófono.
- Afinador previo al ejercicio.
- Árbol de habilidades simple (1 módulo con nodos desbloqueables).
- Ejercicios sobre tablatura con detección de audio en tiempo real (notas y acordes abiertos).
- Rotación semanal de nota raíz y escala.
- Progresión adaptativa automática.
- Feedback visual inmediato: correcto / incorrecto / fuera de tiempo.
- Gamificación: XP, racha diaria, nodos.
- Tutor IA conversacional (nube).
- Generación de backing tracks simples.

**Excluye**
- Pentagrama y rutas de género/rol.
- Visión por computadora.
- Canciones comerciales con licencia.
- Cuentas, sincronización, backend propio.

## Validation Plan
- **Técnica:** el motor de audio detecta notas y acordes abiertos por micrófono en dispositivos reales, con latencia aceptable.
- **De uso:** un principiante completa un nodo en una sesión sin ayuda y entiende qué falló.
- **De hábito:** el usuario vuelve al día siguiente y mantiene la racha.
- **De IA:** el tutor responde dudas básicas y la progresión adaptativa cambia el siguiente ejercicio según los resultados.

## Success Criteria
- Precisión alta en notas monofónicas y aceptable en acordes abiertos.
- Latencia de feedback percibida como inmediata.
- El vertical slice completo funciona sin backend propio.
- El usuario completa el primer nodo y vuelve al día siguiente.

## Notes
- Ámbito de curso: los documentos del proyecto se escriben en Español.
- Riesgo de sobrealcance: 4 frentes de IA (audio, tutor, generación, progresión) en el MVP.
