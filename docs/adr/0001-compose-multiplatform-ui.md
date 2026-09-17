# ADR 0001: UI con Compose Multiplatform

## Status
Accepted

## Context
El proyecto es una app móvil Android e iOS con Kotlin Multiplatform. Hay que decidir si la UI se comparte o se implementa de forma nativa en cada plataforma. La UI incluye pantallas interactivas con tablatura y feedback en tiempo real.

## Decision
Usar una única UI en Compose Multiplatform para Android e iOS. Solo el audio y los permisos se implementan con código nativo por plataforma mediante expect/actual.

## Alternatives Considered
- **UI nativa (Jetpack Compose + SwiftUI):** mejor look nativo y acceso directo a APIs de cada plataforma, pero duplica el trabajo de UI y ralentiza el MVP.
- **Android primero, iOS después:** reduce alcance inicial, pero retrasa la promesa multiplataforma y obliga a rehacer decisiones de UI.

## Consequences
- Se acelera la construcción y el mantenimiento del MVP.
- Se asume menos "sensación nativa" en iOS.
- La capa de audio debe aislarse bien tras expect/actual para no filtrar detalles de plataforma a la UI compartida.
