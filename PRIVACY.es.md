# Política de privacidad

**Charty** es publicado por Pascal Peltriaux.

**Fecha de entrada en vigor:** 1 de junio de 2026

---

## Resumen

Charty no recopila nada. Sin cuentas. Sin analíticas. Sin anuncios. Sin SDK de terceros. Tus datos se quedan en tu dispositivo.

---

## Qué datos se recopilan

**Ninguno.** Charty no recopila, almacena ni transmite ningún dato personal, dato de uso o identificador de dispositivo a ningún servidor.

Específicamente, Charty **no**:

- Crea cuentas de usuario
- Rastrea uso, comportamiento o interacciones
- Muestra anuncios
- Usa SDK de analíticas de terceros (Google Analytics, Firebase, Mixpanel, etc.)
- Incluye píxeles de seguimiento
- Hace peticiones de red para telemetría, informes de fallos o «llamadas a casa»
- Vende, intercambia ni comparte datos con ninguna parte (porque no hay datos que compartir)

Esto está garantizado por el sandbox de iOS de Apple y por la ausencia de cualquier código de red o SDK de terceros en la app. Puedes verificarlo en la ficha de App Store: bajo «Privacidad de la app», Charty declara «Ningún dato recopilado».

## Qué se queda en tu dispositivo

Charty almacena lo siguiente localmente, en tu iPhone/iPad, usando el framework SwiftData de Apple:

- Las rutinas, tareas y horarios que creas
- El nombre de tu hijo/a y (opcionalmente) una imagen de avatar que elijas
- Las recompensas que defines y el saldo de puntos actual
- El historial de sesiones (qué rutinas se completaron, cuándo, puntos ganados)
- Las preferencias (sonido, vibraciones, animaciones, hash del PIN parental, preferencia biométrica)
- Fotos personalizadas de tareas, si decides añadir alguna desde tu biblioteca de Fotos

Todo esto vive en tu dispositivo. Nada sale de tu dispositivo a menos que **tú** lo exportes explícitamente.

## Cosas que puedes hacer que implican que los datos salgan de la app

Las siguientes funciones entregan datos a **iOS mismo**, que los enruta bajo tu control. Charty nunca ve ni almacena el resultado:

- **Imprimir o compartir como PDF** — Charty genera un PDF localmente y presenta la hoja para compartir de iOS. Tú decides si quieres usar AirPrint, guardar en Archivos, enviar por correo, mensajería, etc.
- **Exportar sesiones como CSV** — Mismo patrón: archivo generado localmente, hoja para compartir que se lo entrega a la app que elijas.
- **Sincronización con iCloud** (opcional, desactivada por defecto) — Cuando se activa en Ajustes, tus datos se sincronizan a través de la **base de datos privada** de CloudKit, cifrada por Apple y vinculada a tu propia cuenta de iCloud. El desarrollador de Charty no puede leer tu base de datos privada de iCloud. La sincronización es opcional.

## Privacidad de los niños

Charty está diseñado para niños, principalmente de 4 a 10 años, incluyendo niños con discapacidades del desarrollo como el trastorno del espectro autista (TEA).

Cumplimos con COPPA (EE. UU.) y GDPR-K (UE) **por diseño**: no recopilamos ningún dato — ni de niños ni de adultos — por lo que no hay nada que consentir, nada que procesar, nada que eliminar.

El bloqueo parental (PIN de 4 a 6 dígitos o Face ID / Touch ID) garantiza que solo los adultos puedan cambiar los Ajustes, editar rutinas o reiniciar el saldo de puntos.

## Cámara y Fotos

Si tocas «Elegir foto» para el icono de una tarea o para la recompensa del rompecabezas de imagen, iOS muestra su selector de fotos estándar. La foto elegida se **copia** al sandbox local de la app (redimensionada y comprimida en JPEG para el caso del rompecabezas). Las fotos nunca salen de tu dispositivo.

Charty no solicita acceso a la cámara. Si quieres usar una foto nueva, tómala primero con la app Fotos y luego selecciónala mediante el selector de fotos.

## Face ID / Touch ID

Si activas el desbloqueo biométrico para el bloqueo parental, la autenticación la gestiona enteramente el sistema local Face ID / Touch ID de Apple. Los datos biométricos nunca salen del Secure Enclave de tu dispositivo, y Charty nunca los ve — solo recibimos una devolución «éxito» o «fallo» de parte de iOS.

## Notificaciones

Charty programa notificaciones **locales** para los recordatorios de rutinas diarias. Las gestiona iOS y no implican ningún servidor. Puedes desactivarlas por rutina, o globalmente mediante Ajustes iOS → Notificaciones → Charty.

## Acceso a la red

Charty **no hace** ninguna petición de red, salvo la sincronización con iCloud si la has activado explícitamente (que pasa por la propia infraestructura de iCloud de Apple). La app no tiene URLs integradas, ni puntos de telemetría, ni configuración remota, ni SDK de publicidad, ni SDK de analítica, ni informador de fallos. En modo Avión, Charty funciona idénticamente (la sincronización con iCloud simplemente se pausa hasta que vuelva la conexión).

## Compras

Charty es gratis de descargar, con un desbloqueo único opcional, «Charty Plus». Las compras las gestiona **íntegramente la App Store / StoreKit de Apple** — Charty nunca ve tu nombre, tu tarjeta de pago ni tu ID de Apple. La app solo guarda un indicador local de si Plus está desbloqueado; ese indicador se deriva del recibo de Apple en el dispositivo y, si activas la sincronización con iCloud, puede viajar por tu propia base de datos privada de iCloud. Charty no recopila ni envía a su desarrollador ningún dato de compra o pago. La declaración «Ningún dato recopilado» de la App Store sigue siendo válida.

## Cambios en esta política

Si esta política cambia, la nueva versión reemplaza este archivo en el repositorio público. Los cambios importantes se indicarán al principio con una nueva fecha de entrada en vigor. Como no se recopilan datos, no hay datos históricos que migrar o reutilizar.

## Contacto

📧 **Correo:** ppeltriaux@gmail.com

Preguntas, preocupaciones o solicitudes de verificación independiente bienvenidas.
