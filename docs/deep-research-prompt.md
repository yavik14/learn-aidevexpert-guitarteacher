# Deep Research Prompt — App de guitarra con IA y gamificación

> Prompt listo para usar en herramientas de deep research (ChatGPT Deep Research,
> Gemini, Perplexity, etc.). Su salida alimenta el brief de producto.

---

ROL
Actúa como un equipo combinado de investigador de producto (PM), analista de mercado,
diseñador de aprendizaje (learning designer) y estratega técnico especializado en apps
de educación musical con IA. Tu trabajo es producir un informe de investigación profundo,
con evidencia y fuentes citadas, sin suposiciones sin respaldar.

CONTEXTO
Estamos evaluando construir una app móvil que enseña a tocar la guitarra guiando al
usuario con ejercicios y acordes progresivos según su nivel. La idea es un MVP para
móvil (iOS + Android) y queremos que la inteligencia artificial sea parte central del
producto (no un añadido). Además, la experiencia debe ser gamificada al estilo Duolingo:
motivadora, con progreso diario y distintos tipos de ejercicios, incluyendo lectura de
pentagrama (notación estándar) y tablatura. El objetivo final de esta investigación es
informar un "brief" de producto: problema, usuario, propuesta de valor, alcance del MVP,
diferenciación, riesgos y modelo de negocio.

OBJETIVO
Determina si esta app puede ganar un hueco real en el mercado, para quién exactamente,
cómo debería integrarse la IA de forma defendible, cómo debería diseñarse la pedagogía y
la gamificación, y cuál sería el MVP mínimo con mayor probabilidad de éxito.

PREGUNTAS DE INVESTIGACIÓN (responde por separado y con fuentes)

1. MERCADO Y TENDENCIAS
   - Tamaño, crecimiento y segmentación del mercado de apps de aprendizaje de guitarra
     e instrumentos en general (últimos 3 años + proyección).
   - Tendencias de consumo: qué está creciendo y qué está cayendo, y por qué.
   - Barreras de entrada reales (contenido musical, licencias, audio, reputación).

2. USUARIO Y PROBLEMA
   - Perfiles de usuarios (edad, motivación, contexto, presupuesto, dispositivo).
   - Datos sobre abandono: por qué los principiantes dejan de tocar guitarra y dejan
     las apps. ¿Qué tasas de retención se reportan?
   - Jobs-to-be-done y momentos de frustración concretos que una app podría resolver.

3. COMPETENCIA
   - Analiza en profundidad: Yousician, Fender Play, Simply Guitar, Justin Guitar,
     Uberchord, Chordify, Ultimate Guitar, Rocksmith, Duolingo Music y cualquier otra
     relevante (incluidas alternativas gratuitas y YouTube).
   - Para cada una: propuesta de valor, modelo de precios, uso de IA y de gamificación,
     puntos fuertes, debilidades y reseñas negativas recurrentes (busca reviews reales).
   - Cómo gamifican y cómo enseñan notación/tablatura las líderes del sector.
   - Huecos y oportunidades de diferenciación no cubiertos hoy.

4. IA APLICADA (lo más importante)
   Evalúa viabilidad, madurez, coste y latencia de:
   - Detección/transcripción de audio en tiempo real (monofónica y polifónica) para
     evaluar si el usuario toca los acordes correctamente; estado del arte y precisión.
   - Visión por computadora para postura, mano de trasteo y técnica.
   - LLM / tutor conversacional para currículo adaptativo y explicación de teoría.
   - RAG sobre teoría musical y repertorio.
   - Generación de ejercicios, backing tracks o canciones personalizadas.
   - Aprendizaje adaptativo (spaced repetition, dificultad dinámica según desempeño).
   - Detección de errores, corrección en tiempo real y feedback auditivo/visual.
   Indica explícitamente qué es factible HOY en un MVP móvil vs. qué es I+D a futuro,
   y qué implicaciones tiene hacerlo on-device vs. en la nube (privacidad, coste, latencia).

5. PEDAGOGÍA, GAMIFICACIÓN Y TIPOS DE EJERCICIOS
   - Fundamentos de cómo se aprende guitarra: orden de aprendizaje (postura, cuerdas
     al aire, acordes abiertos, cejilla, escalas, ritmo, teoría), errores típicos.
   - Gamificación estilo Duolingo: analiza mecánicas concretas (rachas/streaks, XP,
     niveles, árbol de habilidades, ligas, vidas/corazones, metas diarias, logros,
     notificaciones, patrones de recompensa) y su evidencia real sobre retención y
     motivación. Incluye críticas y riesgos (ansiedad, castigo por fallar, fatiga).
   - Catálogo de tipos de ejercicio viables y cómo se priorizan para un MVP:
     reconocimiento de acordes, cambios de acorde cronometrados, ear training,
     ritmo con metrónomo/backing track, quiz de teoría, lectura de tablatura y
     lectura de pentagrama, tocar sobre canción, dictado, etc.
   - Uso del pentagrama (notación estándar) y de la tablatura: comparativa pedagógica,
     cuándo introducir cada uno, apps/papers que lo aborden, y cómo se puede gamificar
     la lectura de notación. ¿Conviene enseñar ambos en paralelo o secuencialmente?
   - Cómo diseñar la progresión según nivel y cómo detectar cuándo subir o bajar de nivel.
   - Métricas de aprendizaje válidas (no solo engagement): ¿cómo se mide competencia real?

6. ASPECTOS LEGALES Y DE CONTENIDO
   - Copyright de canciones, tablaturas, acordes y partituras; qué se puede y no se puede usar.
   - Privacidad: audio y video son datos sensibles; implicaciones regulatorias
     (GDPR/COPPA), especialmente si hay menores.

7. NEGOCIO
   - Modelos de monetización viables (suscripción, freemium, etc.) y benchmarks de
     precios en el sector.
   - Coste estimado de inferencia/IA por usuario activo y su impacto en márgenes.
   - Canales de adquisición que funcionan en este nicho.

8. RIESGOS Y CONTRARGUMENTOS
   - Presenta la mejor versión del argumento en CONTRA de construir esta app.
   - Riesgos técnicos, de mercado, de coste de IA, de retención y pedagógicos
     (gamificación que fomenta jugar más que aprender).

FORMATO DE SALIDA
- Informe estructurado por secciones, con una tabla comparativa de competidores
  (incluyendo columnas de IA y gamificación).
- Cada afirmación cuantitativa con su fuente y fecha (enlaces).
- Distingue claramente entre HECHO VERIFICADO, ESTIMACIÓN y OPINIÓN.
- Cierra con: 5 conclusiones clave, 3 oportunidades de diferenciación priorizadas,
  un catálogo priorizado de tipos de ejercicio para el MVP y 3 preguntas abiertas
  que el brief aún debe resolver.

CRITERIOS DE CALIDAD
- Prioriza fuentes primarias: informes de industria, stores, papers (incl. ciencia del
  aprendizaje y HCI musical), documentación técnica, reseñas de usuarios y webs oficiales.
- No inventes cifras. Si no hay dato fiable, dilo explícitamente.
- Piensa en términos de MVP y de "qué haría fracasar esto".
