# ContaIA Beta — Escritorio (Windows)

Repositorio de la beta de escritorio de ContaIA: descarga, características y uso. El código de la app vive en [hubgunter4-ops/contaia-practicas-ia](https://github.com/hubgunter4-ops/contaia-practicas-ia).

## Descarga

- **Versión:** 0.1.0-beta.1
- **Archivo:** `Contaia-Setup-0.1.0-beta.1.exe`
- **Descarga:** https://github.com/hubgunter4-ops/contaia-practicas-ia/releases/download/v0.1.0-beta.1/Contaia-Setup-0.1.0-beta.1.exe
- **Release:** https://github.com/hubgunter4-ops/contaia-practicas-ia/releases/tag/v0.1.0-beta.1
- **Tamaño:** 161.662.764 bytes (154,2 MiB)
- **SHA-256:** `62dae6af0803b2b6a67c0a17a65b64214e9ba6813c34d8f891b31e311ae5affb`

Verifica el archivo descargado antes de instalarlo. En PowerShell:

```powershell
Get-FileHash .\Contaia-Setup-0.1.0-beta.1.exe -Algorithm SHA256
```

El hash debe coincidir con el de arriba.

> El repositorio principal es privado: el enlace de descarga solo funciona para quien tiene acceso a él. Sin sesión, GitHub devuelve 404.

## Características

- **Solo herramientas, sin cursos.** La beta de escritorio no incluye Aprende; eso queda solo en la web.
- Herramientas con sus conexiones reales: Analizador CFDI, Pólizas sugeridas, Conciliación bancaria, DIOT, Nómina y Monitor fiscal.
- Asistente Nora con sus conexiones a Anam, Vercel (AI Gateway / Functions) y Supabase.
- Base de datos propia para escritorio: proyecto Supabase **NoraCFDI-Escritorio**, separada de la web/PWA (NoraCFDI).
- **Sin captcha.** El programa de escritorio es local, no un clon de la página como la PWA, así que no lleva captcha.
- Nora es una burbuja animada, no una foto humana.
- Instalador NSIS con atajos de escritorio y menú inicio.

## Uso

1. Descarga el instalador del enlace de arriba.
2. Ejecuta `Contaia-Setup-0.1.0-beta.1.exe` y sigue el instalador (puedes elegir la carpeta de instalación).
3. Abre ContaIA desde el escritorio o el menú inicio.
4. Inicia sesión con tu cuenta. Las herramientas trabajan contra la base de escritorio (NoraCFDI-Escritorio).

### Requisitos

- Windows 10 u 11, 64 bits.
- Conexión a internet para las herramientas que usan Anam, Vercel y Supabase.

### Notas de la beta

- El instalador **no está firmado**: Windows puede mostrar una advertencia de SmartScreen. Es esperado en esta beta.
- La instalación en Windows aún no se ha probado en un equipo real; la app se verificó arrancando y sirviendo en Linux.
- No se empaquetan claves reales en el programa; las conexiones usan variables de entorno del servidor local.
