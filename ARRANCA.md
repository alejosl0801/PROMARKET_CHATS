# ARRANCA — BRIEFING COMPLETO PARA NUEVA SESIÓN
## ProMarket Ecuador — Sistema de ventas WhatsApp
## Última actualización: 7 de junio 2026 — segunda migración de sesión

> ## INSTRUCCIÓN PARA NUEVA SESIÓN — LEER PRIMERO
>
> **LA DINÁMICA ES UNA SOLA:**
> Alejandro pega el chat → tú das el mensaje exacto a enviar → tú registras en git y haces push.
>
> **NUNCA:**
> - Preguntar "¿le respondo?" — siempre dar el mensaje directamente
> - Preguntar "¿quieres que registre?" — siempre registrar sin preguntar
> - Usar herramientas de GitHub MCP para registrar — usar git commit + push local
> - Esperar permiso para hacer commit — cada mensaje nuevo = commit inmediato
>
> **SIEMPRE:**
> - Dar el mensaje listo para copiar y pegar
> - Hacer commit + push después de cada mensaje nuevo
> - Actualizar el archivo del cliente en CHATS/ en tiempo real
> - Si llega un chat nuevo → crear archivo + dar respuesta + commit, todo junto

---

## 1. QUIÉN ES PROMARKET ECUADOR

- **Dueño:** Alejandro (Loja, Ecuador)
- **Modelo:** Dropshipping COD (contraentrega) via **Rocket.ec**
- **Cómo funciona:** Alejandro vende por WhatsApp → cliente paga al retirar en Servientrega → Rocket.ec (Guayaquil) empaqueta y envía → ProMarket cobra el margen
- **ProMarket tiene sede en Loja** ← nunca decir "somos de Guayaquil"
- **Rocket.ec** tiene la bodega física — ProMarket solo vende
- **Productos activos:**
  - Guante Robótico de Rehabilitación — $59.99 precio normal
  - Ollas de Acero Inoxidable — $49.99 precio normal (campaña pausada, solo cerrar leads existentes)
- **Canal:** WhatsApp Business + Facebook Ads

---

## 2. UNIT ECONOMICS (NÚMEROS REALES)

| Producto | Precio | Costo Rocket+envío | Margen bruto | CAC ads | Margen neto |
|---|---|---|---|---|---|
| Guante $59.99 | $59.99 | $30.67 | $29.32 | $8.49 | **$20.83** |
| Guante liq $49.99 | $49.99 | $30.67 | $19.32 | $8.49 | **$10.83** |
| Guante par $107.98 | $107.98 | $61.34 | $46.64 | $8.49 | **$38.15** |
| Ollas $49.99 | $49.99 | $27.59 | $22.40 | $18.99 | **$3.41** |

---

## 3. ESTRATEGIA DE PRECIO POR ETAPA

- **Lead nuevo / conversación activa:** $59.99 siempre
- **Lead que no respondió 24h+:** re-enganchar con $49.99 ("bajó el precio")
- **Lead frío +7 días:** $49.99 + urgencia real ("solo por hoy", "últimas unidades")
- ❌ NUNCA dar $49.99 de entrada a lead nuevo — destruye el margen

---

## 4. ESTRUCTURA DE REPOS EN GITHUB

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
SESIONES/            → resumen operativo por día
ANALISIS/patrones.md → patrones y errores
```

> **Rama activa en AMBOS repos:** `claude/magical-franklin-iCbBk`

---

## 5. ESTADO ACTUAL — 7 JUN 2026

### Ventas cerradas (total)
| Orden | Cliente | Producto | Ciudad | Estado |
|---|---|---|---|---|
| #146271 | Alex Fernando Lara Alvarez | Guante x2 $107.98 | Ambato | ✅ Entregado |
| #144356 | Blanca Rodríguez | Guante izq. M $59.99 | Quito | ✅ Reclamo resuelto 7/Jun |
| #146110 | Willman Zúñiga | Ollas $49.99 | Puyo | ✅ En tránsito |
| #146504 | Carmen Sosa | Guante x2 $107.98 | Ambato | ✅ Entregado |
| (pendiente) | Jimmy Vera Peñafiel | Guante der. $49.99 | Guayaquil/Vergeles | ⏳ Orden enviada, esperando guía |

### Chats activos ahora mismo — PRIORIDAD MÁXIMA
| Número | Archivo | Estado | Próximo paso |
|---|---|---|---|
| +593 98 656 8029 | CHATS/2026-06-07_593986568029.md | 🔥🔥 Fertisa, Guayaquil — dio sector, preguntó precio | Confirmar agencia Servientrega cerca de Fertisa → pedir datos |
| +593 96 133 9428 | CHATS/2026-06-07_593961339428.md | 🔥 Guante derecho para familiar | Esperar ciudad → confirmar agencia → pedir datos |
| kushita2016 +593 99 920 0994 | CLIENTES/+593_99_920_0994_kushita2016.md | 🔥🔥 Mensaje enviado hoy | Esperar respuesta — si no responde mañana 8am: "buenos días! 😊 ¿cómo amaneció su mamá?" |
| +593 99 412 3065 | CLIENTES/+593_99_412_3065.md | 🔥 Pregunta de pagos respondida | Esperar respuesta |
| +593 98 954 8974 | CHATS/2026-06-07_593989548974.md | 🟠 Sin respuesta tras msg duplicado | Enviar: "¿Es para usted o para un familiar? 😊" |

### Leads fríos — promo domingo YA ENVIADA a todos
- Guante: Norma, Mangu, Bettys, tu papa, ivanojeda + leads 6/6 sin respuesta
- Ollas: Wuinston, Dr. Barros, Gustavo, Sery, Rosa Torres, Carlota, Alvita, Maggi, Ita Vera, Cecilia
- Mensaje guante frío: "Hola! 😊 el guante que vimos bajó de $59.99 a $49.99 solo por hoy domingo — envío incluido ¿se anima?"
- Mensaje ollas frío: "Hola! 😊 las ollas que vimos bajaron de $49.99 a $39.99 solo por hoy domingo — envío incluido ¿se anima?"

### Leads cerrados hoy 7/Jun — no contactar
| Número | Razón |
|---|---|
| +593 96 998 3880 | Creyó que podía comprar en Servientrega directamente |
| +593 99 397 1425 | Necesita dispositivo para pie, no mano |

---

## 6. REGLAS CRÍTICAS

### Respuesta
1. **Responder en menos de 5 minutos**
2. **Primer mensaje = precio en la primera línea** — máximo 2 líneas
3. **NUNCA ignorar pregunta directa** del cliente
4. **Responder siempre los audios** — "¡Escuché! 😊 [respuesta al contenido]"
5. **Todos los mensajes empiezan con MAYÚSCULA**
6. **No repetir información ya enviada** — revisar el historial antes de responder

### Emojis
- Flujo normal → 😊 🙌
- Cliente comparte sufrimiento/enfermedad → 🙏
- ❌ NUNCA 😊 o 💛 después de frase de empatía

### Scripts clave
- **"¿de dónde son?"** → *"Tenemos bodega en Loja y llegamos a todo Ecuador 🇪🇴 — paga al retirar en Servientrega, no adelanta nada ✅"*
- **"¿en cuántos pagos?"** → *"Es un solo pago al retirar en Servientrega 😊 — paga cuando tiene el producto en sus manos ✅"*
- **"¿para quién es?"** → preguntar ANTES de ciudad — involucra emocionalmente

### Flujo correcto
```
1. Saludo + precio directo ($59.99)
2. "¿Es para usted o para un familiar?"
3. Respuesta empática si comparten situación (🙏)
4. Ciudad → sector → agencia Servientrega
5. Pedir datos: nombre / celular / dirección
6. Generar orden Rocket.ec
7. Confirmar orden + PDF
8. Guía cuando Servientrega autoriza
```

### Cierre
- "Ok gracias" / "Ya le aviso" = NO educado → responder con reserva + urgencia real
- "A la orden" sin cierre = venta perdida
- "¿le proceso?" solo cuando el cliente ya autorizó explícitamente

---

## 7. REGLA DE REGISTRO — OBLIGATORIA

- **Cada mensaje nuevo del cliente** → actualizar CHATS/ + commit + push INMEDIATO
- **Cada aprendizaje nuevo** → aprendizajes.md + ARRANCA.md + commit + push
- **Cada sesión** → SESIONES/YYYY-MM-DD.md + commit + push
- **No acumular** — en tiempo real, cada enter

---

## 8. PENDIENTES URGENTES (en orden exacto)

1. **+593 98 656 8029 (Fertisa, Guayaquil)** — confirmar agencia Servientrega cerca de Fertisa y pedir datos. ACTIVO AHORA.
2. **+593 96 133 9428** — esperar ciudad, cuando responda confirmar agencia + pedir datos
3. **kushita2016 (+593 99 920 0994)** — esperar respuesta de hoy. Si no responde: mañana 8am *"buenos días! 😊 ¿cómo amaneció su mamá? — hoy el guante bajó a $49.99 solo por hoy, envío incluido ✅"*
4. **+593 98 954 8974** — enviar: *"¿Es para usted o para un familiar? 😊"*
5. **Jimmy Vera Peñafiel** — cuando Servientrega autorice enviar guía: *"Jimmy su guante está en camino 📦 llega en 3-4 días a Servientrega Vergeles ✅"*
6. **Testimonio Alex Lara (+593 97 926 9065)** — al final del día: *"Hola Alex! 😊 ¿cómo va con el guante? nos ayudaría mucho un comentario corto de su experiencia 🙌"*
7. **Subir precio mañana lunes a $59.99** — hoy es $49.99 "solo por hoy domingo". Si no sube mañana, la urgencia muere.
8. **Corregir bot automático** — manda mensajes duplicados + cotiza precio desactualizado
9. **Fusionar rama claude/magical-franklin-iCbBk a main** en ambos repos

---

## 9. ERRORES QUE NUNCA REPETIR

1. Decir "somos de Guayaquil" — ProMarket es de **Loja**
2. 😊 o 💛 después de situación difícil — usar **🙏**
3. Mencionar % de descuento — solo precio final
4. Guión largo como primer mensaje
5. Ignorar pregunta directa del cliente
6. "A la orden" sin técnica de cierre
7. Responder audio como si no existiera
8. Urgencia falsa o extendible
9. Ficha técnica sin precio primero
10. Preguntar ciudad cuando ya la dijo
11. Mandar respuesta duplicada — revisar el historial siempre
12. Empezar mensaje con minúscula
13. Dar $49.99 a lead nuevo — solo para re-enganche 24h+
14. Registrar sin hacer commit — siempre push inmediato

---

## 11. MENSAJES LISTOS — LEADS PENDIENTES CON HISTORIAL

> Si alguno responde la promo de hoy domingo, pegar la respuesta y dar el siguiente paso.
> Si no responden hoy, esperar hasta mañana lunes 8am antes de volver a escribir.

---

### GUANTE — leads que recibieron promo hoy "bajó a $49.99 solo por hoy domingo"

**Norma Chavarría — +593 98 480 0900**
- Historial: llegó a pedir agencia, mandó 2 audios, ghosteó. Agencia confirmada en su sector.
- Si responde: *"Norma! 😊 Perfecto — me ayuda con sus datos para generarle la orden: 📌 Nombre completo 📌 Celular 📌 Dirección de referencia"*

**Mangu — +593 99 557 7529**
- Historial: preguntó por el PAR izq+der. Le dieron precio mal ($113.98). Dijo "ok gracias" y se fue.
- Si responde: *"Hola! 😊 El par sale a $99.98 con envío incluido — ¿de qué ciudad nos escribe?"*

**Bettys — +593 98 501 1737**
- Historial: preguntó "¿de qué lugar son?" y nadie respondió → ghosteó.
- Si responde: *"Somos de Loja, llegamos a todo Ecuador con Servientrega 🇪🇴 — paga al retirar, no adelanta nada ✅ ¿de qué ciudad nos escribe?"*

**"tu papa" — +593 93 976 3359**
- Historial: 2 contactos, solo respondió "Precio" una vez, nunca dio ciudad.
- Si responde: *"$49.99 con envío incluido 😊 ¿de qué ciudad nos escribe?"*

**ivanojeda — +593 98 946 0509**
- Historial: 3 contactos, NUNCA respondió nada. Casi sin esperanza.
- Si responde: *"Hola! 😊 $49.99 con envío incluido — ¿de qué ciudad nos escribe?"*
- Si no responde hoy: cierre de conversación — no volver a escribir

**+593 93 996 4634**
- Historial: solo preguntó precio 6/6, no respondió ciudad.
- Si responde: *"¿De qué ciudad nos escribe? 😊"*

**+593 97 987 1730**
- Historial: preguntó precio + garantía 6/6. Señal de compra.
- Si responde: *"¿De qué ciudad nos escribe? 😊"*

**+593 98 591 2050**
- Historial: dijo "quiero realizar mi pedido" 6/6, no respondió ciudad.
- Si responde: *"¿De qué ciudad nos escribe? 😊"*

**+593 99 727 8035**
- Historial: dijo "quiero realizar mi pedido" 6/6, no respondió ciudad.
- Si responde: *"¿De qué ciudad nos escribe? 😊"*

**+593 96 100 7773 (El Oro)**
- Historial: intermediario que va a consultar con la persona. Ciudad: El Oro.
- Si responde: *"Perfecto! 😊 En El Oro tenemos agencias disponibles — ¿en qué sector está?"*

**+593 99 412 3065 (Santo Domingo)**
- Historial: preguntó "¿en cuántos pagos?" — se respondió hoy. Esperando.
- Si responde: confirmar agencia Santo Domingo → pedir datos

---

### OLLAS — leads que recibieron promo "bajó a $39.99 solo por hoy domingo"

**Wuinston — +593 98 109 9770** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Dr. BARROS — +593 98 110 2387** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Gustavo — +593 99 615 7785** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Sery — +593 97 874 3450** / Historial: le gustó el precio, dijo "me animo y le aviso", Jipijapa hay Servientrega / Si responde: *"Sery! 😊 ¿Le genero la orden? Me ayuda con: 📌 Nombre 📌 Celular 📌 Dirección"*
**Rosa Torres — +593 98 651 6901** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Carlota — +593 99 027 6468** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Alvita — +593 93 957 7932** / Si responde: *"¿De qué ciudad nos escribe? 😊"*
**Maggi — +593 96 700 4465** / Historial: mandó audio ignorado / Si responde: *"¡Escuché! 😊 ¿De qué ciudad nos escribe?"*
**Ita Vera — +593 96 705 3789** / Historial: preguntó "¿se paga al recibir?" ignorado / Si responde: *"Sí, paga al retirar en Servientrega 😊 — no adelanta nada ✅ ¿De qué ciudad nos escribe?"*
**Cecilia — +593 98 737 1421** / Si responde: *"¿De qué ciudad nos escribe? 😊"*

1. **Bot automático tiene errores críticos:** duplica mensajes + cotiza $59.99 cuando debería ser el precio de liquidación
2. **"¿Es para usted o para un familiar?"** es la mejor pregunta de enganche — confirmado por Alejandro
3. **Leads recientes (<24h):** solo una pregunta, no mensaje completo
4. **Patrón "quiere ir a Servientrega a comprar":** explicar el modelo UNA VEZ, si no entiende cerrar
5. **Patrón "producto equivocado":** cliente de pie/tobillo → el guante no aplica → cerrar honestamente con 🙏
6. **Promo dominical ejecutada** — si mañana lunes el precio no sube a $59.99, la urgencia "solo por hoy" queda destruida
