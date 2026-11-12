# FabLabs para Android

Pronósticos de **NBA** y **NFL** de [FabLabs](https://www.fablabs.app) en tu teléfono.

> **Fase de pruebas (versiones 0.x).** La app puede tener errores y cambiar seguido. Aquí solo se publican los APK;
> el código es privado.

- **Última versión:** ver [Releases](https://github.com/FabrizioCoder/fablabs-android/releases/latest)
- **Historial de cambios:** [CHANGELOG.md](CHANGELOG.md)

---

## Qué incluye

| Función | Estado |
|---|---|
| Base de la app: pestañas NBA, NFL y Ajustes | Disponible desde 0.1.0 |
| NBA: pronósticos del día, detalle del partido, historial de jugadores, calendario y analizador | En desarrollo |
| NFL: pronósticos de la semana, detalle del partido, historial de jugadores y lesiones | En desarrollo |
| Alineaciones (NBA y NFL) | En desarrollo |
| Iniciar sesión con tu cuenta de FabLabs | En desarrollo |
| Ajustes → Notificaciones: nueva versión, pronósticos nuevos y alineaciones confirmadas | En desarrollo |
| Actualizar desde la app, sin desinstalar | En desarrollo |

Para crear una cuenta o recuperar tu contraseña, usa [www.fablabs.app](https://www.fablabs.app).

## Requisitos

- Android **7.0 o posterior**.
- Conexión a internet. Sin conexión, la app muestra lo último que descargó (cuando llegue esa función).

## Qué APK descargar

Cada versión trae un APK por tipo de procesador. Descarga **solo uno**:

| Archivo | Para |
|---|---|
| `app-arm64-v8a-release.apk` | **La mayoría de los teléfonos actuales.** Si no sabes cuál, usa este. |
| `app-armeabi-v7a-release.apk` | Teléfonos antiguos o de gama baja de 32 bits. |
| `app-x86_64-release.apk` | Emuladores en computadora. |

Si Android dice que la app «no es compatible», prueba con `armeabi-v7a`. Usa siempre el mismo tipo al actualizar.

## Instalación

1. Abre la [última versión](https://github.com/FabrizioCoder/fablabs-android/releases/latest) desde el teléfono y
   descarga el APK que te corresponde.
2. (Recomendado) Verifica la descarga, ver la siguiente sección.
3. Abre el APK. Android pedirá permitir **instalar apps de fuentes desconocidas** para tu navegador o administrador
   de archivos: permítelo, instala FabLabs y vuelve a desactivar ese permiso.
4. Si Play Protect muestra una advertencia, es porque la app no viene de la Play Store. Elige **Instalar de todas
   formas** solo si descargaste el APK de esta página.

## Verificar la descarga

Cada versión publica `SHA256SUMS.txt` con la huella de cada APK. Compara la del archivo que descargaste:

- **Windows (PowerShell):** `Get-FileHash .\app-arm64-v8a-release.apk -Algorithm SHA256`
- **macOS o Linux:** `shasum -a 256 app-arm64-v8a-release.apk`

Si la huella no coincide, **no lo instales**.

Las notas de cada versión incluyen además la **huella SHA-256 del certificado de firma**. Todas las versiones van
firmadas con el mismo certificado:

```
086e68fb7f84eeae66ac8e1fdcd4ad674590d8123679a603f4b11292fb3f9898
```
 Android rechaza instalar una actualización con una firma distinta: si al actualizar
ves un error de firma o «conflicto con un paquete existente», **no desinstales para forzarlo** y repórtalo.

## Actualizar

- **Hoy:** descarga el APK de la versión nueva y ábrelo. Se instala encima de la anterior y **conservas tus datos**.
  No desinstales antes.
- **Próximamente:** la app avisará de las versiones nuevas y podrás actualizar desde Ajustes. Android siempre te pedirá
  confirmar la instalación.
- No se puede volver a una versión anterior sin desinstalar: Android no instala un número de compilación menor.

## Permisos y privacidad

| Permiso | Para qué | Desde |
|---|---|---|
| Internet | Descargar los pronósticos de www.fablabs.app | 0.1.0 |
| Notificaciones | Solo si activas algún aviso en Ajustes | Próximamente |
| Instalar apps | Actualizar desde la app; Android te pide confirmar cada vez | Próximamente |

- Sin anuncios y sin rastreadores de terceros.
- Solo se conecta por HTTPS, y Android no hace respaldos de la app (tu sesión no se copia a otros equipos).
- Tu sesión se guardará cifrada con el almacén de claves de Android.
- Las notificaciones usarán Firebase Cloud Messaging por temas: FabLabs no guarda tu identificador de dispositivo.

## Versiones

Seguimos [Versionado Semántico](https://semver.org/lang/es/) con el formato **`X.Y.Z+N`**:

| Parte | Cambia cuando |
|---|---|
| `X` (mayor) | Hay cambios incompatibles. Mientras sea `0`, la app está en pruebas. |
| `Y` (menor) | Llegan funciones nuevas. |
| `Z` (parche) | Solo hay correcciones. |
| `N` (compilación) | Sube en **cada** versión publicada y nunca se reutiliza. Android lo usa para saber qué versión es más nueva. |

- Cada versión tiene su etiqueta `app-vX.Y.Z` y un Release con los APK, `SHA256SUMS.txt` y sus notas.
- Una versión publicada **no se modifica**. Si tiene un error, se publica otra con un número mayor.
- Todos los cambios quedan en [CHANGELOG.md](CHANGELOG.md).

## Juego responsable

FabLabs publica **pronósticos estadísticos**. No garantizan resultados ni ganancias. Contenido para mayores de 18 años.
Si apuestas, hazlo con dinero que puedas perder y pon límites.

## Reportar problemas

Abre un [issue](https://github.com/FabrizioCoder/fablabs-android/issues) con:

- la versión de la app (Ajustes) y el APK que instalaste;
- el modelo del teléfono y la versión de Android;
- qué hiciste, qué esperabas y qué pasó (con captura si puedes).

**Nunca** compartas tu contraseña ni datos de tu cuenta en un issue.

## Licencia

© FabLabs. Todos los derechos reservados. Los APK se distribuyen solo para pruebas.
