# 💸 Mis Finanzas

App web personal de finanzas (PEN y USD): dashboard, cuentas, gastos en segundos, gastos fijos con pagos pendientes, metas con planificador (viaje, vivienda, auto, emergencia, independencia financiera), Investment Hub, asistente, reportes y patrimonio.

Todo vive en un solo archivo (`index.html`) sin dependencias que instalar.

## ▶️ Cómo usarla

**Opción 1 · En tu compu (lo más rápido)**
Descarga el repositorio y haz doble clic en `index.html`.

**Opción 2 · Con un servidor local (activa el modo app instalable)**
```bash
npx serve .
# o
python3 -m http.server 8080
```
Abre `http://localhost:3000` (o `:8080`).

**Opción 3 · En internet con GitHub Pages (para usarla en el celular)**
1. Settings → Pages → *Deploy from a branch* → rama `main`, carpeta `/ (root)` → Save.
2. En ~1 minuto estará en `https://<tu-usuario>.github.io/mis-finanzas/`.
3. En el celular: Safari → Compartir → *Agregar a pantalla de inicio* · Chrome → ⋮ → *Instalar app*.

> GitHub Pages gratis requiere que el repositorio sea público. El código no contiene ningún dato tuyo: tus saldos y movimientos se guardan en tu navegador, nunca en GitHub.

## 💾 Dónde se guardan tus datos

| Dónde la abres | Almacenamiento |
|---|---|
| Dentro de claude.ai (artifact) | Base de datos privada de tu cuenta, sincroniza celular y laptop |
| GitHub Pages / local | `localStorage` de ese navegador |

Para pasar datos de un dispositivo a otro: **Ajustes → Copiar respaldo** y luego **Importar respaldo** en el otro.

## 🔐 Privacidad
- PIN de 4 dígitos (PBKDF2-SHA-256) y bloqueo automático por inactividad.
- Sin analítica ni servidores propios.
- Gmail, Google Calendar y “Pregúntale a Claude” solo funcionan dentro de claude.ai (usan tus conectores).

## 📚 Referencias de precios
Las estimaciones de viaje, dúplex y auto están en el objeto `REF` de `index.html`, con fuente y fecha (15-nov-2026). Son referencias, no cotizaciones.
