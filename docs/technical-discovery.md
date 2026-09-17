# Technical Discovery

## Product Surface
App móvil nativa Android e iOS, con código compartido mediante Kotlin Multiplatform.

## Candidate Stack
- KMP para la lógica compartida.
- UI única con Compose Multiplatform (ver ADR 0001).
- Audio y detección con código nativo por plataforma (expect/actual).
- Persistencia local KMP (SQLDelight o similar).
- Tutor y generación vía API de LLM en la nube (ver ADR 0002).

## Data and Storage
- Todo local en el dispositivo; sin backend propio.
- Progreso, racha, XP y resultados en base de datos local.

## Integrations
- API de LLM en la nube para tutor y generación de contenido.
- Sin autenticación de usuario; acceso mediante clave/endpoint del producto.

## Authentication and Authorization
- No aplica en el MVP (sin cuentas ni roles).

## Deployment and Operations
- Distribución vía Google Play y App Store.
- Sin servidores propios; dependencia de un proveedor de LLM.

## Testing and Verification
- Tests unitarios de lógica compartida (progresión, racha, XP).
- Tests del motor de audio con muestras conocidas.
- Tests de UI Compose y pruebas manuales en dispositivos reales (Android + iOS).

## Observability
- Logging y reporte de crashes a nivel de plataforma; sin telemetría propia en el MVP.

## Constraints
- Permiso de micrófono obligatorio.
- Latencia mínima en el feedback: la detección corre on-device.
- Tutor y generación requieren internet y generan coste por uso.
- La detección polifónica (acordes) por micrófono es la parte más frágil.
