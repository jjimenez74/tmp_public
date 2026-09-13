# 🎁 Amigo Secreto 2026 - Sistema Web

Aplicación para sorteo de Amigo Secreto completamente controlado y con panel administrativo.

---

## 📦 Archivos Incluidos

```
amigo-secreto/
├── index.html           ← Página principal (donde entra cada persona)
├── admin.html           ← Panel administrativo (solo para ti)
├── amigos.json          ← Base de datos con los 42 amigos
├── LISTA_URLS.xlsx      ← URLs para copiar-pegar en WhatsApp
└── README.md            ← Este archivo
```

---

## 🚀 Instalación en GitHub Pages

### Paso 1: Preparar tu repositorio
1. En GitHub, crea un nuevo repositorio público llamado `amigo-secreto` (o usa uno existente)
2. Copia estos 3 archivos a la carpeta raíz:
   - `index.html`
   - `admin.html`
   - `amigos.json`

### Paso 2: Configurar GitHub Pages
1. Ve a Settings → Pages
2. Selecciona "Deploy from a branch"
3. Elige rama "main" y carpeta "root"
4. ¡Listo! GitHub publicará automáticamente

### Paso 3: Tu URL será
```
https://tunombre.github.io/amigo-secreto/
```
(Reemplaza `tunombre` con tu usuario de GitHub)

---

## 📋 Cómo Usar

### Para los Participantes:

1. **Reemplaza `tunombre` en todas las URLs** de LISTA_URLS.xlsx
   
2. **Envía mensaje privado a cada persona** en WhatsApp:
   ```
   Hola Paula ❤️
   
   Aquí te dejo el enlace donde podrás descubrir quién es tu Amigo Secreto 🎁🤫
   
   Recuerda que es muy secreto, así que guarda bien el misterio y no le cuentes a nadie. 😜❤️
   
   👇 Descubre tu Amigo Secreto:
   https://tunombre.github.io/amigo-secreto/?id=paula_6
   
   ¡Que disfrutes! 🎉
   ```

3. **Cada persona entra a su link personalizado:**
   - Se muestra una animación de "sorteo"
   - Se genera un número random (para que vean que fue sorteado)
   - Se revela el amigo secreto asignado
   - El número se usa para verificación ("Este es mi número de sorteo")

### Para Ti (Administrador):

1. **Accede al panel:** `https://tunombre.github.io/amigo-secreto/admin.html`

2. **Ingresa la contraseña:** `1234` (puedes cambiarla en admin.html)

3. **Verás:**
   - ✅ Quién abrió cada sobre (nombre + hora + número)
   - ⏳ Quién aún no abre
   - 📊 Porcentaje de participación
   - 📥 Botón para descargar los datos en JSON
   - 🗑️ Botón para reiniciar todo

---

## 🔧 Personalización

### Cambiar Contraseña del Admin

En `admin.html`, busca esta línea (arriba del todo):

```javascript
const PASSWORD = "1234"; // ← Cambia el número aquí
```

Reemplaza `"1234"` por la que quieras.

### Cambiar la Contraseña Admin

Ejemplo: si quieres contraseña `"micontraseña2026"`:

```javascript
const PASSWORD = "micontraseña2026";
```

### Modificar los Amigos

Si necesitas editar quién es amigo de quién:
1. Abre `amigos.json`
2. Busca el nombre
3. Cambia el valor en `"amigo_secreto"`
4. Guarda

Ejemplo:
```json
{
  "id": "paula_6",
  "nombre": "Paula",
  "amigo_secreto": "Camila"  ← Cambia aquí
}
```

---

## 📊 Panel Admin - Qué Ves

```
👁️ Panel de Control - Amigo Secreto 2026

📊 STATS:
   42 Aperturas
   100% Completado

📬 APERTURAS RECIENTES:
   Paula (paula_6)
   Hora: 14:32:15
   Random: 78932
   ✓ Visto

📭 PENDIENTES:
   Camila (camila_5)
   Espera: Paula

[🔄 Refrescar] [📥 Descargar] [🗑️ Reiniciar] [🚪 Salir]
```

---

## 🔐 Seguridad

- ✅ No hay backend, todo es local en el navegador
- ✅ Los datos se guardan en `localStorage`
- ✅ Solo tú ves el admin con contraseña
- ✅ El número random es único por sesión
- ✅ Cada persona solo ve su propio sobre

---

## 📱 Funciona en

- ✅ Navegadores de escritorio (Chrome, Firefox, Safari, Edge)
- ✅ Mobile (iPhone, Android)
- ✅ Tablets
- ✅ Sin necesidad de instalar nada

---

## 🆘 Solución de Problemas

### "No funciona el enlace"
- Verifica que reemplazaste `tunombre` por tu usuario de GitHub
- Espera 2-3 minutos después de publicar (GitHub tarda un poco)

### "El admin no muestra datos"
- Presiona F5 para refrescar
- Abre el navegador en modo incógnito
- Los datos se guardan en cada navegador (no en la nube)

### "Necesito cambiar la lista de amigos"
- Edita `amigos.json`
- Sube los cambios
- Presiona Ctrl+Shift+R en el navegador para limpiar caché

### "Olvidé la contraseña del admin"
- Abre `admin.html` con un editor
- Busca `const PASSWORD =`
- Cambia a lo que quieras
- Sube los cambios

---

## 💡 Tips

1. **Envía los mensajes desde tu teléfono** (más personal)
2. **Hazlo todo en el mismo día** (para que no se filtre)
3. **Guarda el panel admin abierto** para ver quién abre en tiempo real
4. **Descarga los datos al final** (por si acaso)
5. **El número random es solo para credibilidad** - explica que es el "número de sorteo" de cada persona

---

## 🎉 ¡Que lo Disfrutes!

```
         🎁
        /  \
       /    \
      /      \
     /________\
     |_________|
      |       |
      | AMIGO |
      |SECRETO|
      |_______|
```

---

**Creado con ❤️ para tu Amigo Secreto 2026**

Version: 1.0 | Last Update: 2026-09-12
