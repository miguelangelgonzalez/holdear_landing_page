# Holdear

> Tu portafolio argentino, finalmente en un solo lugar.

Landing page para Holdear, una plataforma SaaS para centralizar y trackear inversiones argentinas: bonos, CEDEARs, acciones de USA y crypto.

## 🎯 Qué es Holdear

Holdear resuelve el problema de los inversores argentinos que tienen sus activos dispersos en múltiples brokers y exchanges. La plataforma permite:

- Centralizar bonos argentinos, CEDEARs, US stocks y crypto
- Calcular automáticamente el precio promedio de compra (incluyendo comisiones)
- Ver el P&L real en ARS y USD
- Tipo de cambio MEP actualizado automáticamente

## 📁 Estructura del proyecto

```
holdear_app/
├── index.html    # Landing page completa (HTML + CSS + JS)
└── Readme.md     # Este archivo
```

## 🚀 Cómo correr localmente

### Opción 1: Python (recomendado)
```bash
cd holdear_app
python3 -m http.server 8080
```
Abrir http://localhost:8080

### Opción 2: Node.js
```bash
npx serve .
```

### Opción 3: Abrir directamente
Hacer doble clic en `index.html` para abrirlo en el navegador.

## 🎨 Design System

### Colores
| Nombre | Hex | Uso |
|--------|-----|-----|
| Background | `#0d0d0d` | Fondo principal |
| Surface | `#141414` | Cards, modales |
| Primary (Lime) | `#c8f542` | CTAs, highlights |
| Green | `#4ade80` | Ganancias, éxito |
| Red | `#f87171` | Pérdidas, errores |
| Blue | `#60a5fa` | US Stocks |
| Purple | `#a78bfa` | CEDEARs |
| Orange | `#fb923c` | Bonos AR |
| Yellow | `#facc15` | Crypto |

### Tipografías
- **Display:** Space Grotesk
- **Body:** Inter
- **Monospace:** JetBrains Mono

## 💰 Planes

| Plan | Precio | Características |
|------|--------|-----------------|
| Esencial | USD $8/mes | 20 activos, dashboard completo, MEP, P&L |
| Pro | USD $12/mes | Ilimitado + Excel export + alertas + soporte |

## 📧 Waitlist

El producto está en desarrollo. La landing incluye un modal de waitlist para capturar emails de usuarios interesados.

Por ahora los emails se loguean en consola. Para conectar con un backend, modificar la función de submit en el `<script>`:

```javascript
waitlistForm.addEventListener('submit', (e) => {
    e.preventDefault();
    const email = emailInput.value;
    
    // TODO: Enviar a tu API
    fetch('/api/waitlist', {
        method: 'POST',
        body: JSON.stringify({ email })
    });
});
```

## 📱 Responsive

La landing es completamente responsive y se adapta a:
- Desktop (1200px+)
- Tablet (768px - 1024px)
- Mobile (< 768px)

## 🛠 Tecnologías

- HTML5
- CSS3 (variables, grid, flexbox, animaciones)
- JavaScript vanilla
- Google Fonts (Space Grotesk, Inter, JetBrains Mono)

---

**Estado:** 🚧 En desarrollo

**Contacto:** [Agregar email o link]
