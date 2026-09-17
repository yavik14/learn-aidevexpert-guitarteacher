# Context

Glosario y lenguaje compartido del proyecto. No es un PRD, ni un plan, ni un registro de decisiones.

## Glossary

### Practicante
Usuario final de la app: persona que aprende a tocar la guitarra. En el MVP hay un único practicante local por dispositivo; no existen cuentas.

### Ejercicio
Unidad mínima de práctica que el practicante ejecuta y que la app evalúa. Ejemplo: tocar una secuencia de notas de un compás sobre tablatura.

### Nodo
Unidad de progresión del árbol de habilidades. Agrupa uno o varios ejercicios con un objetivo. Tiene estados.

### Módulo
Conjunto de nodos que comparten un objetivo mayor (p. ej. "primeros acordes abiertos"). El MVP incluye un módulo.

### Árbol de habilidades
Estructura de progresión formada por módulos y nodos, con desbloqueo secuencial.

### Sesión de práctica
Una ejecución concreta de un ejercicio: afinación previa, el ejercicio en sí y sus resultados.

### Feedback de audio
Evaluación en tiempo real de lo que el practicante toca, comparado con lo esperado. Estados: correcto, incorrecto, fuera de tiempo.

### Tablatura
Notación de seis líneas que indica cuerda y traste. Es la notación principal del MVP.

### Pentagrama
Notación musical estándar. Fuera del MVP.

### Afinador
Sección previa al ejercicio que comprueba y guía la afinación de cada cuerda.

### Nota raíz
Nota que da nombre y centro tonal a un ejercicio o escala. En el MVP rota cada semana.

### Escala
Secuencia ordenada de notas a partir de una nota raíz. En el MVP rota cada semana.

### Racha
Número de días consecutivos con al menos una sesión de práctica completada.

### XP
Puntos de experiencia otorgados al completar ejercicios y nodos. Alimentan el nivel.

### Nivel
Progreso acumulado del practicante en el árbol, derivado de XP y nodos completados. Distinto de la dificultad de un ejercicio.

### Progresión adaptativa
Ajuste automático (por IA) del siguiente ejercicio o de su dificultad según el desempeño reciente.

### Tutor IA
Asistente conversacional (nube) que responde dudas y explica teoría.

### Backing track
Pista de acompañamiento generada sobre la que el practicante toca.

### Acorde abierto
Acorde ejecutado sin cejilla, usando cuerdas al aire. Candidato principal del MVP.

### Ruta
Especialización por género (Rock, Country, Flamenco) o rol (rítmica vs lead). Fuera del MVP.

## Rejected / Ambiguous Terms

### Lección
Usar `Nodo` o `Ejercicio` según corresponda. "Lección" mezcla unidad de progresión y unidad de práctica.

### Amigable (tablatura)
Usar `Tablatura interactiva`. "Amigable" no describe una propiedad verificable.

### Admin
No aplica: el MVP no tiene roles ni administración.
