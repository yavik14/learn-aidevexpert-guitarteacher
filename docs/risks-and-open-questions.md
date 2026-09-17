# Risks and Open Questions

## Blocking Next Phase
- Precisión real de detección de acordes abiertos por micrófono en dispositivos variados.
- Elección de librería/modelo de detección de audio on-device y su viabilidad en Android e iOS.
- Cómo distribuir y proteger la clave del LLM sin backend propio.

## Implementation-Time Questions
- Definir la rotación semanal (calendario, zona horaria, cuándo cambia la semana).
- Definir umbrales de la progresión adaptativa (nº de fallos, ventana, acciones).
- Formato exacto de la tablatura interactiva y sincronización temporal.
- Modelo de datos local y estrategia de migraciones.
- Cómo se generan los backing tracks (proveedor, formato, almacenamiento).

## Later / Not MVP
- Pentagrama y rutas de género/rol.
- Visión por computadora.
- Cuentas y sincronización multidispositivo.
- Monetización/suscripción.

## Assumptions
- El usuario tiene guitarra (acústica) y un móvil con micrófono.
- Practica en un entorno con ruido moderado.
- La detección monofónica puede ser fiable; la de acordes, aceptable.

## Risks
- **Sobrealcance:** 4 frentes de IA (audio, tutor, generación, progresión) en el MVP.
- **Detección poco fiable:** provocaría frustración, justo lo que se quiere evitar.
- **Dependencia de nube:** coste por tokens y experiencia offline incompleta.
- **Gamificación mal calibrada:** que fomente "jugar" más que aprender.
- **Copyright:** si se introducen canciones sin licencia.

## Research Tasks
- Benchmark de detección de pitch/acordes on-device (precisión y latencia) en KMP.
- Comparar proveedores de LLM en nube y coste por usuario activo.
- Revisar prácticas de gamificación y notación en apps líderes (ver docs de gamificación).
