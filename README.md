# Penta Padel

Gestor de torneos de pádel — single-page web app.

## Stack

- HTML/CSS/JS vanilla (single file `index.html`)
- Firebase Realtime Database para sincronización en tiempo real
- `localStorage` como fallback offline
- SheetJS (`xlsx`) para exportar a Excel

## Ejecución local

Abrir `index.html` en el navegador, o servirlo con cualquier servidor estático:

```bash
npx serve .
```

## Deploy

Deploy estático en Vercel. No requiere build.

## Datos

- `jugadores` y `torneos` se persisten en Firebase Realtime Database (`penta-padel-default-rtdb`).
- Si Firebase no está disponible, la app cae a `localStorage` y sigue funcionando offline.
- Backup manual: botón "Exportar" (descarga JSON) / "Importar" (restaura desde JSON).

## Pendiente

- [ ] Autenticación (Firebase Auth)
- [ ] Reglas de seguridad en Firebase Realtime Database (actualmente abiertas)
- [ ] Dominio custom
