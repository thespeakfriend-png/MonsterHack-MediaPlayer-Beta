# 🎵 MonsterHack MediaPlayer — Beta pública (versiones de prueba)

Este repositorio **no contiene código fuente**. Es el punto de descarga público para las
**versiones de prueba (TRIAL, 30 días)** de MonsterHack MediaPlayer, pensado para que
usuarios externos las prueben y reporten bugs/feedback antes de un lanzamiento estable.

El código fuente vive en un repositorio privado aparte. Aquí solo se publican
instaladores firmados como *assets* de [Releases](../../releases), versión por versión.

---

## ⬇️ Descargar la última versión de prueba

Ve a la pestaña **[Releases](../../releases)** y descarga el instalador de tu plataforma
en el release marcado `latest`:

| Plataforma | Archivo | Notas |
|---|---|---|
| Windows 10/11 (64-bit) | `MonsterHack MediaPlayer_X.Y.Z_x64-setup_TRIAL-30dias.exe` | Instalador NSIS |
| Windows 10/11 (64-bit) | `MonsterHack MediaPlayer_X.Y.Z_x64_en-US_TRIAL-30dias.msi` | Instalador MSI alternativo |
| Android | `MonsterHack-MediaPlayer_X.Y.Z_TRIAL-30dias.apk` | Requiere permitir "orígenes desconocidos" |

> ⚠️ **Estas son compilaciones de prueba con vigencia de 30 días desde la instalación.**
> Pasado ese plazo la app deja de reproducir hasta instalar una versión más nueva.
> No usar para distribución final a clientes — solo para testing con beta testers.

---

## 🧭 Versiones finales estables publicadas

Solo se distribuyen aquí las versiones finales estables de cada plataforma. Builds
intermedias/de desarrollo (1.9.0–1.13.0) se retiraron del listado público.

| Versión | Windows | Android | Novedades principales |
|---|---|---|---|
| **1.18.1** | — *(pendiente de build)* | ✅ | Biblioteca persistente estilo Windows Media Player: cache de carátulas por carpeta, cache de listados por `mtime`, reconciliación de carpetas en paralelo, render de cola troceado (carga instantánea con bibliotecas grandes) |
| **1.18.0** | ✅ | ✅ | Base sobre la que se apoyó la mejora de biblioteca persistente de 1.18.1 |

> El instalador de Windows para 1.18.1 aún no se ha compilado; para Windows, 1.18.0
> es la versión estable más reciente disponible.

**Funcionalidades generales de la app** (todas las versiones): reproducción MP3/FLAC/WAV/OGG/OPUS/AAC/M4A,
ecualizador paramétrico de 10 bandas, crossfade configurable, letras sincronizadas `.lrc`,
temas Oscuro/Vidrio/AMOLED/Claro con acento de color dinámico, visualizador de espectro,
integración con teclas multimedia.

---

## 🐛 Reportar bugs / feedback

Abre un [Issue](../../issues) en este repositorio con:
- Versión instalada y plataforma (Windows/Android + versión de OS).
- Pasos para reproducir el problema.
- Capturas o logs si aplica.

---

## 🔒 Aviso

Este es software de prueba (trial) para evaluación. El código fuente y las claves de
firma son privados; este repositorio solo distribuye binarios ya compilados y firmados.
