# AVAL ERP — Notas del proyecto

## URLs
- **Live:** https://erp.avalmex.com
- **Vercel:** https://aval-erp.vercel.app
- **GitHub:** https://github.com/vromordz/aval-erp
- **Sitio principal:** https://avalmex.com (repo: github.com/vromordz/avalmex)

## Stack
- HTML estático puro (sin framework)
- Hospedado en Vercel (plan gratuito)
- Dominio en Squarespace DNS
- Formulario: Formspree `https://formspree.io/f/xaqvnlrk`

## Identidad visual
- **Fuentes:** Bebas Neue (títulos) + DM Sans (cuerpo)
- **Colores:**
  - Rojo: `#C8102E`
  - Negro: `#0A0A0A`
  - Blanco: `#F5F3EE`
  - Gris superficie: `#1A1A1A`
  - Gris2: `#2A2A2A`
  - Texto muted: `#888`
- **Estilo:** Minimalista industrial, negro/blanco/rojo, sin gradientes

## Estructura de la página (index.html)
1. **Nav** — logo + links (Módulos, Beneficios, Contacto) + CTA "Solicitar Demo" → `#demo`
2. **Back bar** — "← Regresar a avalmex.com" → https://avalmex.com
3. **Hero** — título, subtítulo, mockup de dashboard de rendimientos
4. **Strip** — ticker de certificaciones (TIF, NOM-194, HACCP, CFDI 4.0...)
5. **Módulos** (`#modulos`) — 4 cards en grid 2x2:
   - 01 Producción
   - 02 Inventarios
   - 03 Despiece
   - 04 Rendimientos
6. **Beneficios** (`#beneficios`) — lista + grid de stats (TIF, NOM, 100%, MX)
7. **Formulario demo** (`#demo`) — Formspree, campos: nombre, empresa, correo, teléfono, tipo de operación, mensaje
8. **Footer** — logo + copyright

## Módulos destacados
| # | Módulo | Tags clave |
|---|--------|-----------|
| 01 | Producción | Órdenes, formulaciones, trazabilidad por lote, control de turno |
| 02 | Inventarios | Multi-almacén, caducidades, alertas, kardex |
| 03 | Despiece | Cortes por canal, piezas obtenidas, destino de corte, vs. estándar |
| 04 | Rendimientos | Real vs. esperado, mermas, reportes por turno, por especie |

## Contacto del proyecto
- **Correo:** vromo@avalmex.com
- **WhatsApp:** +52 871 505 0753
- **Responsable:** Valdemar Romo (VROMO)

## Flujo de despliegue
```
Editar index.html localmente
  → git add .
  → git commit -m "descripción del cambio"
  → git push
  → Vercel despliega automáticamente en ~1 min
```

## Ruta local del proyecto
```
C:\Users\valdemar.romo\Downloads\PERSO_2\AVALMEX\V2\erp
```

## DNS
- Proveedor: Squarespace
- Registro: CNAME `erp` → `6e8085980e4f8422.vercel-dns-017.com`

## Conexión con avalmex.com
- En `src/app/page.tsx` del repo avalmex, la tarjeta del ERP en la sección Plataformas tiene link activo a `https://erp.avalmex.com`
- Estilo del botón: `.statusLive` en `page.module.css`

## Pendientes / ideas futuras
- [ ] Página de confirmación post-formulario
- [ ] Sección de precios o planes
- [ ] Screenshots o demo interactiva del ERP
- [ ] SEO: meta tags Open Graph para compartir en redes
- [ ] Analytics (Google Analytics o Vercel Analytics)
