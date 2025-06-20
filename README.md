# Reto JS Básico: Conecta con la API de OpenAI

Este reto está diseñado para quienes están comenzando con JavaScript y desean aprender a **consumir APIs externas** desde el navegador. Utilizaremos la API de OpenAI como caso práctico concreto para que experimentes cómo enviar datos, recibir respuestas y mostrar resultados en pantalla.

---

## Objetivo

Construir una pequeña aplicación web tipo "chat" donde el usuario pueda escribir una pregunta, enviarla a la API de OpenAI y ver la respuesta generada por la inteligencia artificial directamente en el navegador.

El objetivo principal es que comprendas el flujo completo de consumo de una API REST desde JavaScript puro:
- Cómo estructurar una petición HTTP usando `fetch()`
- Cómo enviar datos y recibir respuestas en formato JSON
- Cómo manejar errores y mostrar mensajes claros al usuario
- Cómo manipular el DOM para mostrar los resultados

Además, aprenderás buenas prácticas de seguridad para el manejo de claves API y la importancia de **no exponer secretos en repositorios públicos**.

---

## Instrucciones
- Debes consumir la API de OpenAI (por ejemplo, usando `fetch`) y mostrar las respuestas en el navegador (puedes simular un chat simple).
- El manejo de la API Key lo hará el instructor, tú solo debes dejar el espacio o la variable preparada para colocarla.
- Implementa manejo básico de errores y muestra mensajes claros si algo sale mal.
- No uses frameworks ni librerías externas (solo JS puro).

### Qué debes entregar
- Un archivo HTML básico con la estructura mínima.
- Un archivo CSS opcional para estilos simples (no es el foco del reto).
- Un archivo JS donde esté toda la lógica de conexión, envío de mensajes y manejo de respuestas de la API.

### Qué se evaluará
- Que logres conectarte exitosamente a la API de OpenAI y mostrar respuestas.
- Que entiendas y expliques cómo funciona el flujo de petición/respuesta de una API.
- Que se manejen errores básicos (por ejemplo, si la API responde con error, mostrarlo en pantalla).

**Recuerda:** El foco es aprender a consumir APIs desde JavaScript y entender el flujo de datos, no el diseño visual.

---

## Requisitos

- Un archivo `.html` donde pegues el script JS.
- Un entorno simple: navegador + editor de código como VSCode.

---

## Paso a Paso sugerido

A continuación tienes una guía sugerida para conectar tu aplicación con la API de OpenAI:

1. **Prepara tu estructura básica**
   - Crea un archivo `index.html` con un formulario simple para enviar preguntas y un área para mostrar respuestas.
   - Crea un archivo `main.js` (o como prefieras llamarlo) donde pondrás toda la lógica de conexión con la API.
   - (Opcional) Un archivo CSS para estilos básicos.

2. **Obtén tu API Key de OpenAI**
   - **No subas tu API Key al repositorio ni la compartas públicamente.**
   - Los tutores entregarán las API Keys físicamente y las distribuirán a los líderes de célula.

3. **Conecta con la API de OpenAI usando JavaScript**
   - En tu archivo JS, crea una función que use `fetch()` para hacer una petición POST a la API de OpenAI (por ejemplo, a `https://api.openai.com/v1/chat/completions`).
   - Incluye tu API Key en el header `Authorization` (ejemplo: `Bearer TU_API_KEY`).
   - Envía el mensaje del usuario en el cuerpo de la petición, siguiendo el formato que pide la documentación.
   - Muestra la respuesta de la API en el navegador.
   - Maneja posibles errores y muestra mensajes claros si algo sale mal.

4. **Seguridad**
   - Nunca subas tu API Key a GitHub ni la dejes en archivos públicos. Usa variables de entorno o pide que el usuario la ingrese manualmente si es necesario.

5. **Recursos útiles**
   - Documentación oficial de OpenAI para la API de chat:  
     https://platform.openai.com/docs/guides/text?api-mode=chat
   - Ejemplo de uso con `fetch`:  
     https://platform.openai.com/docs/api-reference/chat/create
   - Documentación general (overview):  
     https://platform.openai.com/docs/overview

---
