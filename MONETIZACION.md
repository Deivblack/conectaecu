# Monetización — ConectaECU

Guía breve de la estrategia y de cómo activar los cobros en la landing.

---

## Estrategia recomendada, por fases

El pilar de ingresos es la **suscripción (freemium → mensual)**, que ya estás construyendo con Stripe. Es recurrente, predecible y está alineada con el valor real: cobrar por *conectar*, no por mover dinero.

| Fase | Usuarios | Enfoque de ingresos |
|------|----------|---------------------|
| **Arranque** | 0–50 | Casi cero ingresos. Donación voluntaria opcional solo para cubrir hosting (~$5–12/mes). Sin publicidad. |
| **Tracción** | 50–300 | Motor principal: freemium → suscripción mensual (Stripe). Este es el pilar. |
| **Escala** | 300+ | Recién aquí, publicidad — pero como **directorio de negocios ecuatorianos verificados**, no banners. Suma confianza en vez de restarla, y conecta con tu proyecto Todos Somos Ecuador. |

### Por qué no publicidad ni donaciones como pilar
- **Publicidad con poco tráfico** no se vende bien (el anunciante no ve retorno) y un banner de terceros en un sitio sobre dinero **erosiona la confianza**, que es justo tu producto.
- **Donaciones** no escalan ni son predecibles. Sirven para cubrir costos al inicio, no para sostener el proyecto.

---

## Dos variantes de landing incluidas

- `index.html` — versión base, limpia, con CTA único al registro.
- `index-planes.html` — **esta variante**: añade la sección de **Planes** (el pilar) y una franja discreta de **Donación** (Stripe + Zelle). Es la recomendada como página principal cuando actives la monetización.

Para usar la variante de planes como principal en GitHub Pages, renómbrala:
```bash
mv index.html index-simple.html
mv index-planes.html index.html
```

---

## Activar los cobros (sin escribir código)

La landing usa **Stripe Payment Links**: enlaces que creas en el dashboard de Stripe y pegas en los botones. No requieren backend.

### 1. Suscripciones mensuales (los dos planes de pago)
1. Entra a **dashboard.stripe.com → Payment Links → New**.
2. Elige **Producto/Suscripción**, crea el producto "Plan Frecuente" con precio **recurrente mensual**.
3. Copia el enlace generado.
4. En `index-planes.html`, busca `PEGA_AQUI_TU_STRIPE_LINK_MENSUAL` y reemplázalo por ese enlace.
5. Repite para el plan "Sin límites" → `PEGA_AQUI_TU_STRIPE_LINK_PREMIUM`.

> Nota: los precios `$4.99` y `$9.99` son de referencia. Ajústalos a tu estrategia (en la landing y en Stripe deben coincidir).

### 2. Donación con tarjeta
1. En Payment Links → New, elige **"El cliente elige cuánto pagar"** (ideal para donaciones).
2. En Opciones avanzadas, cambia el botón de "Pagar" a **"Donar"**.
3. Copia el enlace y reemplaza `PEGA_AQUI_TU_STRIPE_LINK_DONACION`.

> Importante: la donación de **monto libre solo funciona como pago único**, no recurrente. Si quieres donación mensual, crea un producto recurrente con montos fijos. Si eres nuevo en Stripe, pueden pedirte una verificación adicional antes de habilitar donaciones.

### 3. Donación por Zelle
Zelle no tiene enlace web, así que el botón muestra tu dato de contacto al hacer clic. En `index-planes.html` busca:
```html
data-zelle="tu-correo-zelle@ejemplo.com"
```
y reemplázalo por tu correo o teléfono registrado en Zelle.

---

## Comisiones a tener en cuenta
Stripe cobra su tarifa estándar (aprox. **2.9% + $0.30** por transacción en EE. UU.). Zelle no cobra comisión, pero es manual (no hay confirmación automática ni recibo). Considera esto al fijar precios.
