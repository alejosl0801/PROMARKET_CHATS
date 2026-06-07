# ARRANCA — BRIEFING COMPLETO PARA NUEVA SESIÓN
## ProMarket Ecuador — Sistema de ventas WhatsApp

> **INSTRUCCIÓN PARA NUEVA SESIÓN:**  
> Lee este archivo completo antes de hacer cualquier cosa. Luego lee `SESIONES/` para ver el último día trabajado. Luego pregunta: "¿llegó algún chat nuevo?"

---

## 1. QUIÉN ES PROMARKET ECUADOR

- **Dueño:** Alejandro (Loja, Ecuador)
- **Modelo:** Dropshipping COD (contraentrega) via **Rocket.ec**
- **Cómo funciona:** Alejandro vende por WhatsApp → cliente paga al retirar en Servientrega → Rocket.ec (Guayaquil) empaqueta y envía → ProMarket cobra el margen
- **ProMarket tiene sede en Loja** ← nunca decir "somos de Guayaquil"
- **Rocket.ec** tiene la bodega física — ProMarket solo vende
- **Productos activos:**
  - Guante Robótico de Rehabilitación ($59.99 precio normal / $49.99 liquidación)
  - Ollas de Acero Inoxidable ($49.99 precio normal / $39.99 liquidación) — campaña pausada
- **Canal:** WhatsApp Business + Facebook Ads

---

## 2. UNIT ECONOMICS (NÚMEROS REALES)

| Producto | Precio | Costo Rocket+envío | Margen bruto | CAC ads | Margen neto |
|---|---|---|---|---|---|
| Guante $59.99 | $59.99 | $30.67 | $29.32 | $8.49 | **$20.83** |
| Guante liq $49.99 | $49.99 | $30.67 | $19.32 | $8.49 | **$10.83** |
| Guante par $107.98 | $107.98 | $61.34 | $46.64 | $8.49 | **$38.15** |
| Ollas $49.99 | $49.99 | $27.59 | $22.40 | $18.99 | **$3.41** |

> Liquidación destruye el margen. Usar SOLO para leads fríos +7 días sin respuesta. NUNCA para leads nuevos.

---

## 3. ESTRUCTURA DE REPOS EN GITHUB

### `alejosl0801/promarket-ordenes` — El cerebro del negocio
```
CEREBRO/
  01_empresa.md      → datos empresa, script de confianza
  02_camila.md       → personalidad, reglas de respuesta, emojis
  03_guiones.md      → scripts de venta por producto
  04_productos.md    → catálogo y specs
  05_objeciones.md   → manejo de objeciones
  06_campanas.md     → campañas Facebook activas
  07_reglas.md       → reglas operativas críticas
  08_clientes.md     → registro de clientes con estado
VENTAS/
  aprendizajes.md    → todos los aprendizajes acumulados
  analisis_rentabilidad.md → análisis profundo con datos reales
CLIENTES/            → un archivo por lead (31 archivos)
```

### `alejosl0801/PROMARKET_CHATS` — Sistema de logging de chats
```
ARRANCA.md           → este archivo (leer primero)
CHATS/               → un archivo por cliente WhatsApp
  YYYY-MM-DD_número.md
SESIONES/            → resumen operativo por día
  YYYY-MM-DD.md
ANALISIS/
  patrones.md        → patrones y errores actualizados
```

> **Rama activa en AMBOS repos:** `claude/magical-franklin-iCbBk`  
> Siempre hacer push a esa rama. Nunca push a main sin autorización explícita.

---

## 4. ESTADO ACTUAL (actualizado 7 Jun 2026)

### Ventas cerradas (total)
| Orden | Cliente | Producto | Ciudad | Estado |
|---|---|---|---|---|
| #146271 | Alex Fernando Lara Alvarez | Guante x2 $107.98 | Ambato | ✅ Entregado |
| #144356 | Blanca Rodríguez | Guante izq. M $59.99 | Quito | ✅ Reclamo resuelto 7/Jun |
| #146110 | Willman Zúñiga | Ollas $49.99 | Puyo | ✅ En tránsito |
| #146504 | Carmen Sosa | Guante x2 $107.98 | Ambato | ✅ Entregado |
| (pendiente) | Jimmy Vera Peñafiel | Guante der. $49.99 | Guayaquil/Vergeles | ⏳ Orden enviada, esperando guía |

### Leads activos hoy 7/Jun — prioridad alta
| Cliente | Número | Producto | Estado | Acción pendiente |
|---|---|---|---|---|
| kushita2016 | +593 99 920 0994 | Guante (mamá, Pelileo) | 🔥🔥 Msg enviado hoy | Esperando respuesta |
| +593 98 656 8029 | — | Guante (Guayaquil) | 🔥 Esperando sector | Cuando responda → confirmar agencia → pedir datos |
| +593 98 954 8974 | — | Guante | 🟠 Sin respuesta tras msg duplicado | Enviar: "¿es para usted o para un familiar? 😊" |
| +593 99 412 3065 | — | Guante (Santo Domingo) | 🔥 Pregunta de pagos respondida hoy | Esperando respuesta |
| Mangu | +593 99 557 7529 | Guante par | 🟠 Promo enviada hoy | Esperando respuesta |
| +593 96 100 7773 | — | Guante (El Oro) | 🟡 Promo enviada hoy | Esperando respuesta |
| Mendez | +593 98 887 6692 | Ollas $39.99 | 🔥 Esperando ciudad | Esperar respuesta |

### Leads fríos — promo domingo (ya escritos 5/6, escribir hoy 7/6)
Guante: Norma (+593 98 480 0900), Mangu (+593 99 557 7529), Bettys (+593 98 501 1737), tu papa (+593 93 976 3359), ivanojeda (+593 98 946 0509)  
Ollas: Wuinston, Dr. Barros, Gustavo, Sery, Rosa Torres, Carlota, Alvita, Maggi, Ita Vera, Cecilia

### Leads cerrados sin venta (NO contactar)
Rosa Carranza, Rose, Gregorio Barzallo — dijeron NO explícito

---

## 5. REGLAS CRÍTICAS (las más importantes)

### Respuesta
1. **Responder en menos de 5 minutos** — factor #1 de conversión. Más de 30 min = venta perdida.
2. **Primer mensaje = precio en la primera línea** — máximo 2 líneas. Sin explicar Servientrega.
3. **NUNCA ignorar pregunta directa** del cliente. Si preguntó algo, responderlo ANTES de avanzar.
4. **Responder siempre los audios** — "¡escuché! 😊 [respuesta al contenido]"

### Emojis por contexto emocional
- Flujo normal → 😊 🙌
- Cliente comparte sufrimiento/enfermedad → 🙏
- Cierre emotivo cálido (solo Camila) → 💛
- ❌ NUNCA 😊 o 💛 después de "qué difícil" o frase de empatía

### Scripts de confianza
- **"¿de dónde son?"** → *"tenemos bodega en Loja y llegamos a todo Ecuador 🇪🇴 — paga al retirar en Servientrega, no adelanta nada ✅"*
- **"¿en cuántos pagos?"** → *"es un solo pago al retirar en Servientrega 😊 — paga cuando tiene el producto en sus manos ✅"*
- **"¿Puedo revisar antes de pagar?"** → *"paga justo al momento de retirarlo en Servientrega 😊 — si algo no está bien, no lo retira"*

### Descuentos
- **NUNCA mencionar % de descuento** — genera desconfianza
- Solo precio final: "$59.99 con envío incluido"
- Liquidación ($49.99) SOLO para leads fríos +7 días sin respuesta

### Cierre
- "Ok gracias" / "Ya le aviso" = NO educado. Responder: *"claro! solo le cuento que el envío incluido es solo hasta [fecha real] 😊 ¿le reservo una unidad mientras decide?"*
- "a la orden" sin técnica de cierre = venta perdida

---

## 6. FLUJO CORRECTO DE VENTA

```
1. Saludo + precio directo en 1 línea
2. "¿es para usted o para un familiar?" ← ANTES de preguntar ciudad
3. Respuesta empática si comparten situación difícil (🙏)
4. Confirmar ciudad → mostrar agencia Servientrega
5. Pedir datos: nombre / celular / dirección referencia
6. Generar orden con Rocket.ec
7. Confirmar orden + enviar PDF al cliente
8. Enviar guía cuando Servientrega autoriza
```

---

## 7. CÓMO FUNCIONA ESTE SISTEMA DE SESIONES

### Cuándo guardar
- Después de cada chat nuevo → crear/actualizar `CHATS/YYYY-MM-DD_número.md`
- Al final de cada día → actualizar/crear `SESIONES/YYYY-MM-DD.md`
- Al aprender algo nuevo → guardar en `promarket-ordenes/VENTAS/aprendizajes.md`
- Al corregir error → actualizar el archivo correspondiente en `CEREBRO/`
- Siempre: commit + push a `claude/magical-franklin-iCbBk` en AMBOS repos

### Cómo migrar de sesión
1. Al final de la sesión → actualizar este `ARRANCA.md` con estado actual
2. Commit + push de todo
3. Nueva sesión: leer `ARRANCA.md` → leer última `SESIONES/` → preguntar si hay chats nuevos

### Archivos de referencia rápida
- Reglas completas: `promarket-ordenes/CEREBRO/07_reglas.md`
- Objeciones: `promarket-ordenes/CEREBRO/05_objeciones.md`
- Guiones: `promarket-ordenes/CEREBRO/03_guiones.md`
- Todos los leads: `promarket-ordenes/CLIENTES/` (31 archivos)
- Análisis rentabilidad: `promarket-ordenes/VENTAS/analisis_rentabilidad.md`

---

## 7b. REGLA DE REGISTRO — OBLIGATORIA

- Después de **cada mensaje nuevo** de un cliente → actualizar CHATS/ + commit + push inmediato
- Después de **cada aprendizaje nuevo** → actualizar aprendizajes.md + ARRANCA.md + commit + push
- Después de **cada sesión** → actualizar SESIONES/YYYY-MM-DD.md + commit + push
- **No acumular nunca** — registrar en tiempo real, cada enter del usuario

---

## 8. PENDIENTES URGENTES (en orden)

1. **kushita2016** — esperar respuesta, si no responde hoy escribir mañana 8/6 a las 8am con: *"buenos días! 😊 ¿cómo amaneció su mamá? — el guante sigue disponible ✅"*
2. **+593 99 412 3065 (Santo Domingo)** — responder pregunta de pagos que fue ignorada: *"es un solo pago al retirar en Servientrega 😊 — no adelanta nada ✅ ¿cuál agencia le queda más cerca?"*
3. **Jimmy Vera Peñafiel** — cuando Servientrega autorice: enviar guía + *"Jimmy su guante está en camino 📦 llega en 3-4 días a Servientrega Vergeles ✅"*
4. **Testimonio** — escribir a Alex Lara (+593 97 926 9065) o Carmen Sosa (+593 99 965 2705): *"hola Alex! 😊 ¿cómo va con el guante? nos ayudaría mucho un comentario corto de su experiencia 🙌"*
5. **Promo domingo** — enviar a todos los leads fríos con mensaje correcto (ver sección 4)

---

## 9. ERRORES QUE NUNCA REPETIR

1. Decir "somos de Guayaquil" — ProMarket es de **Loja**
2. Emoji 😊 o 💛 después de situación difícil — usar **🙏**
3. Mencionar 75% de descuento — **solo precio final**
4. Guión largo como primer mensaje — **precio en la primera línea**
5. Ignorar pregunta directa del cliente — **responderla siempre primero**
6. "A la orden" sin técnica de cierre — **siempre contraatacar**
7. Responder audio como si no existiera — **"¡escuché! 😊"**
8. Urgencia falsa ("extendimos hasta mañana") — **solo urgencia real**
9. Ficha técnica sin precio primero — **precio → luego ficha si pide**
10. Preguntar ciudad cuando ya la dijo — **revisar el historial antes**
