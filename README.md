
# 😸 caritas – Avatar facial reactivo con transparencia ética

**caritas** es una herramienta de comunicación aumentativa que genera un avatar facial expresivo a partir del texto que escribes. Analiza el tono emocional (o lo eliges manualmente) y sincroniza los labios con una voz sintética. Todo en un solo archivo HTML, sin dependencias, sin cámaras, sin hardware especial.

Está pensado para personas con dificultades de habla, educadores, o cualquiera que quiera experimentar con la expresión emocional sintética de forma segura y transparente.

## ✨ Características

- 😊 **Emociones manuales o automáticas**: botones para forzar alegría, tristeza, sorpresa, enfado, o dejar que el texto decida.
- 🗣️ **Voz sintética modulada**: velocidad y tono ajustables según la emoción detectada.
- 🎨 **Avatar dibujado en canvas**: cejas, ojos y boca cambian en tiempo real.
- 🛡️ **Adaptador Ético de Salida**:
  - Marca de agua visual "🤖 IA" superpuesta permanentemente.
  - Prefijo de voz obligatorio: "Atención: mensaje generado por inteligencia artificial".
  - Estas medidas **no se pueden desactivar desde la interfaz** y requieren modificar el código fuente para eliminarlas.
- ⚙️ **Panel de configuración**: ajusta velocidad de habla, tono y sensibilidad del análisis de sentimiento.
- 📱 **Funciona en móviles y ordenadores** sin instalar nada.

## 🚀 Cómo usar

1. Abre `caritas.html` en cualquier navegador moderno (Chrome, Firefox, Edge, Safari).
2. Escribe un mensaje en el cuadro de texto.
3. Opcionalmente, elige una emoción con los botones de abajo (😊😢😐😮😠). Por defecto está en "Auto", que detecta la emoción por palabras clave.
4. Pulsa **Hablar**.
5. El avatar articulará el mensaje con la expresión y la voz adecuadas, siempre precedido del aviso de IA.

## 🧩 Estructura del proyecto
caritas/
├── caritas.html ← la aplicación completa
└── README.md ← este documento

text

## 🛠️ Personalización y mejoras

El código está organizado en dos partes:
- **Core**: lógica de dibujo, análisis de sentimiento y síntesis de voz.
- **Adaptador Ético**: envoltura que fuerza la transparencia.

Puedes:
- Cambiar la lista de palabras clave para otros idiomas.
- Añadir más emociones en el `switch` de dibujo.
- Sustituir el canvas 2D por un modelo 3D (Three.js) manteniendo el adaptador ético intacto.
- Conectar el Core a un chatbot para conversaciones completas.

## 🐞 Limitaciones

- Análisis de sentimiento básico (pronto se podrá integrar un modelo más fino como transformers.js).
- Sincronización labial por intervalos, no por fonemas reales.
- La marca de agua visual puede ser eliminada editando el HTML, pero la voz siempre llevará el prefijo (salvo que se manipule el JavaScript). La idea es desincentivar el mal uso, no ofrecer una jaula 100% irrompible.

## 📜 Licencia

AGPLv3 – Software libre. Puedes usar, modificar y distribuir, siempre que mantengas las mismas libertades. El uso para suplantación de identidad o engaño está explícitamente prohibido por la ética del proyecto, más allá de la licencia.

---

*caritas nació de una conversación sobre ética, arquitectura de software y un japonés que hizo en un fin de semana lo que Apple intenta vender por miles de euros. Ahora es una herramienta útil, transparente y respetuosa con las personas.*
