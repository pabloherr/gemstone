# Gemstone Morse Transmitter

Dos páginas para usar en sesión de rol:

- **`index.html`** — página de jugadores. Solo ven la gema titilar.
- **`dm.html`** — panel del DM. Configura mensaje, desface y velocidad.

## Cómo subir a GitHub Pages

1. Crear un repo nuevo en GitHub (ej. `gemstone-morse`)
2. Subir los dos archivos (`index.html` y `dm.html`)
3. Ir a **Settings → Pages → Source → Deploy from branch → main / (root)**
4. Guardar. En ~1 minuto queda en:
   - Jugadores: `https://TU_USUARIO.github.io/gemstone-morse/`
   - DM: `https://TU_USUARIO.github.io/gemstone-morse/dm.html`

## Uso en sesión

- Vos abrís `dm.html` en tu dispositivo
- Los jugadores abren `index.html` en sus teléfonos
- Escribís el mensaje, elegís desface y velocidad, y transmitís
- La gema titila en sus pantallas — ellos tienen que anotar los pulsos y descifrar

> **Nota:** El BroadcastChannel solo funciona entre pestañas del **mismo navegador**
> en el mismo dispositivo. Para controlar la gema en dispositivos separados
> (tu celular → celular de los jugadores), reemplazá BroadcastChannel por
> Firebase Realtime Database (el mismo proyecto `cosmere-tracker` que usás
> para el combat tracker).
