# Domain Model

## Core Concepts
- Practicante
- Árbol de habilidades → Módulo → Nodo → Ejercicio
- Sesión de práctica → Resultado
- Racha, XP, Nivel
- Afinación (Afinador)
- Escala semanal (nota raíz + escala)
- Backing track
- Conversación con el Tutor IA
- Progresión adaptativa

## Relationships
- Un Practicante tiene un Árbol de habilidades y un Progreso local.
- Un Módulo contiene Nodos; un Nodo contiene Ejercicios.
- Una Sesión de práctica pertenece a un Nodo y produce Resultados.
- Los Resultados alimentan la Progresión adaptativa, el XP y la Racha.
- La Escala semanal parametriza los Ejercicios de la semana.
- El Tutor IA puede generar contenido (ejercicios, backing tracks) que una Sesión referencia.

## States and Lifecycles
- **Nodo:** bloqueado → disponible → en progreso → completado.
- **Sesión:** iniciada → afinando → en ejercicio → completada | abandonada.
- **Resultado de nota/acorde:** correcto | incorrecto | fuera de tiempo.
- **Racha:** activa (practicó hoy) | en riesgo (no ha practicado hoy) | rota (pasó un día sin práctica).
- **Escala semanal:** definida → activa → renovada.
- **Backing track:** generado → disponible | descartado.

## Important Scenarios
1. **Practicar:** iniciar sesión → afinar → tocar → recibir feedback → terminar → ganar XP.
2. **Mantener racha:** completar al menos una sesión al día.
3. **Rotación semanal:** al cambiar la semana se fija nueva nota raíz y escala y se ajustan los ejercicios.
4. **Preguntar al tutor:** abrir chat, preguntar y recibir explicación con diagramas.
5. **Ajuste adaptativo:** tras varios fallos, la IA baja dificultad o cambia de ejercicio.

## Edge Cases
- Micrófono denegado o no disponible → no se puede practicar.
- Afinación no conseguida → advertir o bloquear antes del ejercicio.
- Sin internet → tutor y generación no disponibles; audio y práctica sí.
- Ruido ambiental → detección poco fiable; mostrar aviso.
- Abandono de sesión a medias → no cuenta para racha ni otorga XP completo.
- Cambio de día/huso horario → definir cuándo "cambia el día" para la racha.
- Guitarra mal afinada como causa de fallos → el afinador lo detecta.
