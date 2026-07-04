# Cómo publicar una nueva build de prueba

Este repo nunca commitea binarios. Cada versión se sube como *asset* de un
GitHub Release, generado desde los archivos ya compilados en el repo privado
de código fuente (`Monster-MediaPlayer/builds/`).

## Requisitos
- `gh` autenticado (`gh auth status`).
- Los instaladores TRIAL de la versión ya compilados en
  `../Monster-MediaPlayer/builds/`.

## Pasos

```bash
cd "MonsterHack-MediaPlayer-Beta"

VERSION=1.18.1   # sin la "v"
SRC="../Monster-MediaPlayer/builds"

gh release create "v$VERSION" \
  --title "v$VERSION (beta / trial 30 días)" \
  --notes "Ver CHANGELOG.md y README.md para detalle de esta versión." \
  --latest \
  "$SRC/MonsterHack MediaPlayer_${VERSION}_x64-setup_TRIAL-30dias.exe" \
  "$SRC/MonsterHack MediaPlayer_${VERSION}_x64_en-US_TRIAL-30dias.msi" \
  "$SRC/MonsterHack-MediaPlayer_${VERSION}_TRIAL-30dias.apk"
```

Si para esa versión falta alguna plataforma (p. ej. no hay build de Windows
todavía), omite esa línea del comando.

Después de crear el release:
1. Actualiza la tabla de `README.md` (columna Windows/Android) y `CHANGELOG.md`
   con la fila de la nueva versión.
2. Commitea esos dos archivos (`git add README.md CHANGELOG.md && git commit -m "docs: v$VERSION"`).
