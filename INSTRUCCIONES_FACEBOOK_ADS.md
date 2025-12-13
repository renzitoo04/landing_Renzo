# Instrucciones para Configurar Facebook Ads con Optimización de Conversiones

## ✅ Lo que ya está hecho:
1. Meta Pixel instalado en tu landing page
2. Evento "Contact" configurado para dispararse cuando alguien hace clic en el botón de WhatsApp

---

## 📋 PASO 1: Verificar que el Pixel está funcionando

1. Sube los cambios a Vercel (desde tu carpeta del proyecto):
   ```bash
   git add .
   git commit -m "Agregar Meta Pixel y evento Contact"
   git push
   ```

2. Instala la extensión de Chrome "Meta Pixel Helper": https://chrome.google.com/webstore/detail/meta-pixel-helper/

3. Visita tu landing page en Vercel y verifica que:
   - El Pixel Helper muestra tu pixel (ID: 1618332022468743)
   - Muestra el evento "PageView"
   - Haz clic en el botón de WhatsApp y verifica que se dispare el evento "Contact"

---

## 📋 PASO 2: Configurar el Evento de Conversión en Facebook

1. Ve a **Events Manager** de Facebook: https://business.facebook.com/events_manager2/

2. Selecciona tu Pixel (ID: 1618332022468743)

3. Ve a la pestaña "Eventos personalizados" → Busca el evento **"Contact"**

4. Si no aparece aún, espera unas horas después de que alguien haga clic (o hazlo tú mismo varias veces)

5. Una vez que aparezca, haz clic en los 3 puntos (⋮) al lado del evento → **"Marcar como conversión"**

---

## 📋 PASO 3: Crear la Campaña de Facebook Ads

### A. Nivel de Campaña:

1. Ve a **Administrador de Anuncios**: https://business.facebook.com/adsmanager/

2. Haz clic en **"Crear"** → Selecciona **"Ventas"** como objetivo

3. Nombre de la campaña: "Landing Pages - Conversiones WhatsApp"

4. Desactiva "Advantage Campaign Budget" (para tener más control)

### B. Nivel de Conjunto de Anuncios:

1. **Evento de conversión**:
   - Selecciona tu Pixel
   - Elige el evento **"Contact"** (el que configuramos)

2. **Presupuesto**: Empieza con mínimo $5-10 USD/día

3. **Audiencia**:
   - Ubicación: Argentina (o donde estén tus clientes)
   - Edad: 25-55 años (emprendedores/negocios)
   - Intereses:
     - Marketing digital
     - Publicidad en Facebook
     - Emprendimiento
     - E-commerce
     - Desarrollo web

4. **Ubicaciones**: Deja "Advantage+ placements" (Facebook optimiza)

### C. Nivel de Anuncio:

1. Crea tu anuncio con:
   - **Título llamativo**: "Landing Pages que Generan Clientes Reales"
   - **Texto**: Enfócate en los beneficios (más mensajes, filtros anti-bot, etc.)
   - **Imagen/Video**: Muestra un ejemplo de landing page
   - **Llamado a la acción**: "Más información" o "Enviar mensaje"
   - **URL**: Tu landing page en Vercel

---

## 📋 PASO 4: Optimización de la Campaña

### Estrategia de Puja:
- Usa **"Conversiones"** como objetivo
- Estrategia: **"Costo más bajo"** (al inicio)
- Después de 50+ conversiones, puedes cambiar a "Costo objetivo"

### Qué esperar:
- **Primeros 3-7 días**: Facebook está "aprendiendo". No toques nada.
- **CPM más alto**: Pagarás más por impresión, pero tendrás clics de mayor calidad
- **Menos clics falsos**: Facebook mostrará tu anuncio solo a personas con alta intención

---

## 🎯 Diferencia Clave:

### ❌ Campaña de TRÁFICO (lo que NO querés):
- Objetivo: Clics al enlace
- Facebook te cobra por impresiones
- Facebook muestra tu anuncio a cualquiera que haga clic
- Muchos clics pero pocos leads reales

### ✅ Campaña de CONVERSIONES (lo que SÍ querés):
- Objetivo: Evento "Contact" (clic en WhatsApp)
- Facebook te cobra por impresiones
- Facebook muestra tu anuncio SOLO a personas con alta probabilidad de hacer clic en WhatsApp
- Menos clics totales, pero más clics de calidad

---

## 📊 Métricas a Monitorear:

1. **Costo por conversión (Contact)**: Este es tu costo por persona que hace clic en WhatsApp
2. **CTR (Click-Through Rate)**: % de personas que ven tu anuncio y hacen clic
3. **Tasa de conversión**: % de visitantes que hacen clic en WhatsApp
4. **ROAS**: Cuánto ganas por cada peso invertido

---

## 🚨 Puntos Importantes:

1. **Facebook NO te cobra por conversión**, te cobra por impresiones. Pero optimiza para mostrarte a gente que va a convertir.

2. **Fase de aprendizaje**: Facebook necesita ~50 conversiones por semana para optimizar bien. Si no llegas a eso, considera bajar el presupuesto.

3. **No cambies nada durante 3-7 días**: Déjalo aprender.

4. **Excluye remarketing**: En configuración de audiencia → Excluye "Personas que interactuaron con tu landing en los últimos 7 días" (evita pagar 2 veces por la misma persona)

---

## 🔍 Probar que Todo Funciona:

1. Publica tu landing con los cambios
2. Abre la consola del navegador (F12)
3. Haz clic en el botón de WhatsApp
4. Deberías ver en la consola: "Evento Contact enviado a Facebook Pixel"
5. En Meta Pixel Helper, verifica que aparezca el evento "Contact"

---

## 💡 Extra: Mejorar Conversiones

Si querés maximizar conversiones, considera:

1. **Agregar urgencia**: "Cupos limitados este mes"
2. **Prueba social**: "100+ landing pages creadas"
3. **Garantía**: "Si no te genera leads, te devolvemos el dinero"
4. **Precio ancla**: Mostrar precio tachado vs. precio actual

---

¿Dudas? Revisá la documentación oficial de Meta:
https://www.facebook.com/business/help/
