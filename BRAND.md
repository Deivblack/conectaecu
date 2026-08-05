# Manual de Marca — ConectaECU

**Versión 1.0 · 2026**

---

## 1. La marca en una frase

ConectaECU no mueve dinero. Conecta personas.

Somos un tablón de confianza donde ecuatorianos en Estados Unidos y sus familias en Ecuador se encuentran para intercambiar dólares de forma local, sin comisiones internacionales. La marca debe transmitir **confianza, cercanía y simplicidad** — nunca la frialdad de un banco ni el ruido de una app financiera saturada.

### Principios de marca

1. **Claridad antes que persuasión.** Explicamos, no vendemos. El producto se entiende en una frase.
2. **Confianza visible.** Verificación, reputación y transparencia son el centro, no un detalle.
3. **De la comunidad, para la comunidad.** El tono es humano y directo, como alguien de confianza que te recomienda algo que ya usa.
4. **Sobriedad ecuatoriana.** El origen se siente en acentos discretos, nunca en banderas ni clichés.

---

## 2. Logotipo

El logotipo combina el nombre en dos pesos: **Conecta** en peso medio y **ECU** en peso fuerte, señalando el destino. No se separan.

```
Conecta ECU
```

Junto al texto, un símbolo de enlace: dos nodos unidos por un puente — la representación del "match" entre dos personas, que es el mecanismo real del producto.

### Usos correctos
- Sobre fondo blanco o Arena (preferido).
- Sobre Azul Profundo, en blanco, para piezas de alto contraste.
- Mantener un área de resguardo igual a la altura de la "C" en todos los lados.

### Usos incorrectos
- No deformar, rotar ni aplicar sombras.
- No cambiar los colores del símbolo.
- No colocar sobre imágenes con poco contraste.
- No añadir la bandera de Ecuador como parte del logo.

---

## 3. Color

Paleta deliberadamente corta. El blanco y el espacio en blanco son el material principal; el color se usa con disciplina.

| Rol | Nombre | HEX | Uso |
|-----|--------|-----|-----|
| Primario | Azul Profundo | `#12324F` | Texto principal, encabezados, botón primario, símbolo |
| Acento | Azul Enlace | `#2E6FB8` | Enlaces, estados hover, detalles de interacción |
| Cálido | Dorado Andes | `#E5A83B` | Acento único y escaso: subrayados, íconos de confianza |
| Fondo | Arena | `#F7F5F0` | Fondo de secciones alternas, tarjetas |
| Neutro | Gris Niebla | `#6B7683` | Texto secundario, captions |
| Base | Blanco | `#FFFFFF` | Fondo principal |

**Regla del acento cálido:** el Dorado Andes nunca ocupa bloques grandes. Aparece en trazos finos, íconos pequeños o un subrayado — es el guiño ecuatoriano, no el protagonista. Si una pantalla tiene más de tres apariciones del dorado, sobra alguna.

### Contraste
Todo texto sobre fondo cumple WCAG AA. Azul Profundo sobre Blanco y sobre Arena está validado para cuerpo de texto.

---

## 4. Tipografía

Dos familias, ambas de Google Fonts (libres, fáciles de migrar a cualquier hosting).

| Rol | Tipografía | Uso |
|-----|-----------|-----|
| Display | **Fraunces** (serif, opsz alto) | Titulares grandes. Aporta carácter humano y cálido sin perder seriedad. Usar con moderación. |
| Cuerpo / UI | **Inter** | Todo el texto corrido, botones, formularios, etiquetas. Neutra, legible, moderna. |

### Escala tipográfica
- Display XL — 3.5rem / peso 400 (Fraunces)
- Display L — 2.25rem / peso 400 (Fraunces)
- Título — 1.5rem / peso 600 (Inter)
- Cuerpo — 1.0625rem / peso 400 (Inter)
- Caption — 0.875rem / peso 500 (Inter, Gris Niebla)

Titulares en *sentence case*, nunca en mayúsculas completas. Los números de teléfono, montos y datos siempre en Inter.

---

## 5. Voz y tono

Hablamos como alguien de confianza de la comunidad: claro, cálido, sin tecnicismos.

**Sí decimos:**
- "No movemos tu dinero. Te conectamos con personas que ya lo hacen."
- "Personas ecuatorianas verificadas."
- "Sin comisiones internacionales."

**No decimos:**
- "Solución fintech de compensación P2P" (jerga).
- "La mejor plataforma del mercado" (venta vacía).
- Nada que prometa custodia de fondos o que suene a remesadora.

### Reglas de escritura
- Verbos en activo. El botón dice lo que pasa: "Crear mi cuenta", no "Enviar".
- Frases cortas. Una idea por frase.
- El origen (Ecuador) se nombra con orgullo, sin folclore forzado.

---

## 6. Fotografía e iconografía

- **Íconos:** línea fina, esquinas suaves, un solo color (Azul Profundo o Dorado Andes para íconos de confianza). Estilo consistente en todo el sitio.
- **Fotografía:** personas reales, luz natural, momentos cotidianos (una llamada a la familia, un mercado). Evitar stock corporativo genérico de manos y monedas.
- **Ilustración del "match":** el recurso visual insignia — dos nodos unidos — puede animarse sutilmente para representar la conexión.

---

## 7. Elemento insignia

El **puente de conexión**: dos puntos (una persona en EE. UU., una en Ecuador) unidos por un trazo. Representa literalmente el producto. Se usa en el logo, como marca de agua sutil en la sección "cómo funciona", y como transición entre estados. Es lo que hace memorable a la marca sin recurrir a la bandera.

---

## 8. Aplicación digital — reglas rápidas

- Botones con radio de 10px, sin sombras duras.
- Espaciado generoso: las secciones respiran. El aire es parte de la marca.
- Movimiento discreto: apariciones suaves al hacer scroll, hover sutil. Respetar `prefers-reduced-motion`.
- Mobile primero: la comunidad usa el teléfono. Todo debe funcionar y verse bien en pantalla pequeña.
