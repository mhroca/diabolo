# DiaBolo — Instrucciones para generar el APK

## Contenido del paquete
```
diabolo/
├── index.html          ← App principal
├── manifest.json       ← Configuración PWA
├── sw.js               ← Service worker (modo offline)
├── favicon.ico         ← Ícono del sitio
├── screenshot.png      ← Captura para la tienda
├── icons/
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-384x384.png
│   └── icon-512x512.png
└── README.md
```

---

## PASO 1 — Subir a GitHub Pages (gratis)

1. Entrá a https://github.com y creá una cuenta (si no tenés)
2. Clic en **"New repository"**
3. Nombre: `diabolo` — marcá **Public** — clic **Create**
4. En la página del repo, clic en **"uploading an existing file"**
5. **Arrastrá TODOS los archivos y la carpeta `icons/`** al área de subida
6. Clic **"Commit changes"**
7. Andá a **Settings → Pages**
8. En "Source" seleccioná **"Deploy from a branch"** → branch **main** → folder **/ (root)**
9. Clic **Save**
10. Esperá 1-2 minutos → tu URL será: `https://TU_USUARIO.github.io/diabolo`

---

## PASO 2 — Generar el APK con PWABuilder

1. Entrá a https://www.pwabuilder.com
2. Pegá tu URL de GitHub Pages: `https://TU_USUARIO.github.io/diabolo`
3. Clic **"Start"** — PWABuilder analiza tu app
4. Cuando termine, clic en **"Android"**
5. Clic **"Generate Package"**
6. Descargás un archivo `.zip` con el APK adentro

---

## PASO 3 — Instalar el APK en tu Android

### Opción A — Instalar directamente (sin Play Store)
1. Pasá el APK a tu teléfono (por WhatsApp, cable USB, Google Drive, etc.)
2. En Android: **Ajustes → Seguridad → Instalar apps desconocidas** → activar para tu app de archivos
3. Abrí el APK y tocá **Instalar**

### Opción B — Publicar en Play Store
1. En PWABuilder, además del APK también descargás un **AAB (Android App Bundle)**
2. Creás cuenta en Google Play Console (pago único de U$D 25)
3. Subís el AAB y seguís el proceso de publicación

---

## Notas importantes
- La app funciona **100% offline** una vez instalada
- Los datos se guardan localmente en el teléfono
- Para actualizar la app, simplemente actualizás los archivos en GitHub

---

*Recordá siempre validar las dosis calculadas con tu médico o diabetólogo.*
