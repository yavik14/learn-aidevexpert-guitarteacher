Aquí tienes la **especificación completa del MVP para diseño de prototipo móvil (UI/UX)**, estructurada directamente para definir las pantallas, flujos y componentes necesarios en herramientas de prototipado como Figma:

# Especificación del MVP para Prototipado UI/UX (App Móvil iOS / Android) 1

## 1\. Visión General del Producto

1. **Idea central:** App móvil que enseña a tocar la guitarra mediante ejercicios progresivos guiados por IA en tiempo real y gamificación de alta retención 1-3.  
2. **Problema a resolver:** Altas tasas de abandono en principiantes debido a la frustración, falta de feedback sobre si están tocando correctamente y aburrimiento con la teoría musical tradicional 3-5.  
3. **Diferenciadores Clave de Interfaz:**  
4. **Feedback de audio en tiempo real:** Indicadores visuales inmediatos de precisión en notas y acordes 2, 6, 7\.  
5. **Pentagrama gamificado \+ Tablatura:** Interfaz de notación dual interactiva 8, 9\.  
6. **Motor de Gamificación:** Estructura estilo *Duolingo* (árbol de habilidades, racha diaria, XP, ligas) 2, 3, 8\.  
7. **Rutas de Género y Roles:** Selector de especialización (Guitarra Rítmica vs. Lead / Rock, Country, Flamenco).

## 2\. Mapa de Pantallas y Estructura de Navegación

### Pantalla 1: Home / Árbol de Aprendizaje (*Skill Tree*)

* **Propósito:** Pantalla principal de navegación y progresión diaria.  
* **Componentes UI:**  
* **Header superior:** Contador de Racha (🔥 días), Puntos de Experiencia (⚡ XP), Vidas/Corazones (❤️) y Nivel actual.  
* **Mapa de Nodos (Skill Tree):** Nodos circulares interconectados que representan lecciones y módulos desbloqueables.  
* *Estado de nodo:* Bloqueado 🔒, Disponible ⭐, Completado ✅, Lección Legendaria 👑.  
* **Selector de Ruta / Género (Dropdown o Tab):** Permite cambiar entre la ruta general (Tronco Común) o especializaciones (*Country, Flamenco, Rock/Pop, Rítmica vs. Lead*).  
* **Botón flotante "Práctica Rápida / Tutor IA":** Acceso directo al asistente adaptativo.

### Pantalla 2: Lobby de Lección / Vista Previa

* **Propósito:** Preparar al usuario antes de iniciar una sesión de práctica.  
* **Componentes UI:**  
* **Título y objetivo pedagógico:** (Ej: *"Reconocimiento de Acorde Sol Mayor (G) y cambios rítmicos"*).  
* **Brazalete de Recompensa:** Muestra los XP y gemas a ganar.  
* **Checklist de afinación rápida:** Mini-widget que utiliza el micrófono para verificar la afinación antes de empezar.  
* **Botón primario:** "¡Empezar Lección\!".

### Pantalla 3: Interfaz de Juego y Ejercicio Principal (HUD con IA)

* **Propósito:** Espacio interactivo donde el usuario toca la guitarra física mientras la app escucha 2, 6\.  
* **Componentes UI:**  
* **Área de Notación Dual (Centro):**  
* Alternador de vista: *Pentagrama (Notación Estándar)*, *Tablatura*, o *Vista Dual Combinada* 8, 9\.  
* Cursor de tiempo en cascada o línea de desplazamiento (desplazamiento de izquierda a derecha o vertical).  
* **Overlay de Feedback de Audio en Tiempo Real (IA):**  
* *Verde / Brillo:* Nota/Acorde correcto tocado a tiempo.  
* *Rojo / Agitación:* Nota incorrecta o traste equivocado.  
* *Amarillo / Indicador de Timing:* Nota correcta pero fuera de compás (late/early).  
* **Panel de Control Inferior:**  
* Botón de Pausa / Ajuste de Tempo (Metrónomo integrado).  
* Control de pistas (*Backing track* volumen / guitarra solo).

### Pantalla 4: Tutor IA Conversacional y Explicación Teórica

* **Propósito:** Tutor de voz/texto para resolver dudas, explicar conceptos de teoría musical o ajustar la dificultad 2, 7\.  
* **Componentes UI:**  
* **Avatar del Tutor IA:** Indicador visual de escucha/habla (onda de audio animada).  
* **Chat interactivo:** Mensajes breves explicativos con fragmentos de acordes o diagramas de diapasón incrustados.  
* **Sugerencia adaptativa:** Tarjetas con respuestas rápidas (ej: *"¿Por qué me duele el dedo al hacer cejilla?"*, *"Muéstrame este acorde más despacio"*).

### Pantalla 5: Pantalla de Resultados y Recompensa

* **Propósito:** Feedback al finalizar el ejercicio y refuerzo positivo.  
* **Componentes UI:**  
* **Gráfico de Precisión:** % de notas/acordes acertados y precisión rítmica.  
* **Animación de Recompensa:** Conteo de XP ganados, actualización de racha (🔥) y barra de nivel subiendo.  
* **Resumen de Errores:** Lista de acordes o notas a reforzar para la repetición espaciada (*spaced repetition*) 2, 7\.  
* **Botones:** "Continuar" | "Repetir Ejercicio".

## 3\. Flujos de Usuario Clave para Prototipar

\[Flujo A: Onboarding & Test Inicial\]  
Inicio ➔ Selección de Metas ➔ Permiso de Micrófono ➔ Test de Nivel Adaptativo ➔ Asignación de Nodo Inicial

\[Flujo B: Bucle de Lección Diaria\]  
Home/Skill Tree ➔ Click en Nodo ➔ Calibración de Afinación ➔ HUD Ejercicio (Lectura \+ Audio IA) ➔ Recompensa/XP

\[Flujo C: Tutoría Adaptativa\]  
Dificultad detectada alta (3 fallos seguidos) ➔ Pop-up de Tutor IA ➔ Demostración interactiva a menor tempo ➔ Reintento

## 4\. Alcance del MVP (Qué incluir y qué omitir en los diseños)

### 🟢 DENTRO del prototipo del MVP 2, 8, 9:

1. **Detección de audio para:** Reconocimiento de acordes abiertos, cambios cronometrados, ritmo con metrónomo/backing tracks y notas en notación dual 2, 8, 9\.  
2. **Gamificación completa:** Sistema de racha (streaks), XP, vidas (corazones), metas diarias y árbol de habilidades 2, 3, 8\.  
3. **Módulos de Notación Dual:** Ejercicios interactivos en tablatura y pentagrama 8, 9\.  
4. **Rutas iniciales:** Selección de rol (Rítmica vs. Lead) y catálogo básico por géneros.

### 🔴 FUERA del prototipo del MVP (Futuras versiones / I+D) 2, 7, 10:

1. **Visión por Computadora:** Sin cámaras para evaluar postura o mano de trasteo 2, 7\.  
2. **Canciones con Licencia Comercial:** Utilizar únicamente temas de dominio público o backing tracks generados/propios para evitar costes de copyright 6, 10\.

🎯 ¿Te gustaría que preparemos un documento o informe detallado con esta especificación de producto para guardarlo o exportarlo directamente a tu equipo de diseño?  
