# Manual de Usuario - Teclado Sofle (ZMK Firmware)

Bienvenido al manual de referencia de tu teclado dividido **Sofle** con microcontroladores nRF52840, pantallas OLED y retroiluminación RGB Underglow.

---

## 🎛️ Funciones de los Encoders (Perillas)

El teclado cuenta con dos encoders rotatorios con funciones personalizadas para control multimedia y del sistema:

### Encoder Izquierdo
* **Girar:** Sube / Baja el volumen (`C_VOL_UP` / `C_VOL_DN`).
* **Presionar 3 veces rápidas:** Enciende o apaga la iluminación **RGB Underglow** (`RGB_TOG`).

### Encoder Derecho
* **Girar:** Sube / Baja página (`PG_UP` / `PG_DN`).
* **Presionar 1 vez:** Silencia / Activa el audio (**Mute** `C_MUTE`).
* **Presionar 3 veces rápidas:** Enciende o apaga ambas **pantallas OLED** (`EXT_POWER`).

---

## 📑 Distribución de Capas (Layers)

### 1. Capa Base (`default`)
Es la capa estándar QWERTY para el uso diario de escritura. Incluye el acceso directo a los encoders y teclas multimedia básicas en las esquinas inferiores.

### 2. Capa Lower (`lower`)
Se activa manteniendo presionada la tecla **Lower**. Convierte la mitad superior y derecha en un bloque de funciones y símbolos avanzados:
* **Fila superior:** Teclas de función de `F1` a `F11`.
* **Símbolos:** Acceso rápido a exclamación (`!`), arroba (`@`), numeral (`#`), corchetes, llaves y tuberías (`|`).

### 3. Capa Raise (`raise`)
Se activa manteniendo presionada la tecla **Raise**. Está enfocada en navegación, edición y conectividad Bluetooth:
* **Conectividad:** `BT_CLR` (limpiar emparejamientos) y selección de perfiles Bluetooth (`BT_SEL 0` al `4`).
* **Navegación:** Flechas de dirección (`Arriba`, `Abajo`, `Izquierda`, `Derecha`), `PGUP`, `PGDN`, `HOME`, `END`, `DEL` y `BSPC`.
* **Edición:** Comandos rápidos de Deshacer, Cortar, Copiar y Pegar (`K_UNDO`, `K_CUT`, `K_COPY`, `K_PASTE`).

### 4. Capa Adjust (`adjust`) [Automática]
Se activa de forma automática manteniendo presionadas **simultáneamente las teclas Lower y Raise**. Es el panel de control de hardware y luces:
* **Bluetooth:** Gestión de perfiles en la fila superior.
* **Energía y Pantallas:** `EXT_POWER` para alternar la energía general.
* **Control RGB Completo:**
  * `RGB_TOG`: Encender/Apagar luces.
  * `RGB_BRI` / `RGB_BRD`: Subir / Bajar brillo.
  * `RGB_HUI` / `RGB_HUD`: Cambiar tono de color.
  * `RGB_SAI` / `RGB_SAD`: Subir / Bajar saturación.
  * `RGB_EFF`: Cambiar efecto de animación RGB.

---

## ⚡ Comandos Rápidos Clave

| Acción | Método |
| :--- | :--- |
| **Silenciar Audio** | 1 clic en encoder derecho |
| **Apagar/Encender Pantallas** | 3 clics en encoder derecho |
| **Apagar/Encender RGB** | 3 clics en encoder izquierdo |
| **Entrar a Modo Ajustes** | Mantener `Lower` + `Raise` |
