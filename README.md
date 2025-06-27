# Chat JS con OpenAI

Una aplicación web tipo chat que se conecta con la API de OpenAI para generar respuestas de inteligencia artificial a las preguntas del usuario.

## Descripción del Proyecto

Este proyecto es una aplicación web interactiva que permite a los usuarios mantener una conversación con un modelo de IA de OpenAI. La aplicación está construida con JavaScript y demuestra la implementación de conceptos fundamentales como objetos, closures, callbacks, promesas, async/await, y clases.

## Estructura del Proyecto

```
/js-challenge-week-two
  ├── assets/
  │   ├── css/style.css      # Estilos de la aplicación
  │   └── js/main.js         # Lógica principal del chat
  ├── index.html             # Estructura HTML de la aplicación
  ├── GUIA-PASO-A-PASO.md    # Guía detallada del desarrollo
  ├── README-CONVENCIONES.md # Convenciones de código
  └── README.md              # Este archivo
```

## Características Principales

La aplicación implementa los siguientes conceptos de JavaScript:

### Objetos y Clases
- Utiliza la clase `ChatMessage` para modelar los mensajes con propiedades `autor`, `contenido` y `timestamp`
- Mantiene un historial de conversaciones como un array de objetos mensaje

### Funciones y Scope
- Implementa closures para contar las preguntas del usuario
- Demuestra el concepto de hoisting con funciones declaradas
- Utiliza callbacks para manejar respuestas asíncronas

### Asincronía
- Consume la API de OpenAI utilizando `async/await` y `fetch`
- Implementa manejo de errores con bloques `try/catch`
- Simula carga de mensajes antiguos con promesas
- Utiliza `setTimeout` para crear efectos de "typing" de la IA

## Tecnologías Utilizadas

- HTML5
- CSS3
- JavaScript (ES6+)
- API de OpenAI
- Node.js
- Express
- dotenv
- node-fetch

## Funcionalidades Implementadas

1. **Interfaz de chat** con diseño responsive
2. **Modelado de mensajes** como objetos JS
3. **Historial de conversaciones** persistente durante la sesión
4. **Renderizado dinámico** de mensajes en el DOM
5. **Contador de preguntas** utilizando closures
6. **Callbacks** para procesar respuestas de la API
7. **Consumo de API** con async/await y manejo de errores
8. **Simulación de carga** de mensajes antiguos
9. **Efecto de escritura** para simular que la IA está escribiendo
10. **Manejo de estados** de carga y errores en la interfaz
11. **Modularización** del código en funciones separadas
12. **Diseño visual** moderno y amigable

## Cómo Usar la Aplicación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/Riwi-io-Medellin/js-api-openAI-conection

   cd js-challenge-week-two
   ```

2. Instala las dependencias necesarias:
   ```bash
   npm install
   ```

3. Configura el backend:
   - Crea un archivo `.env` en la raíz del proyecto
   - Añade tu API Key de OpenAI:
     ```
     OPENAI_API_KEY=tu_api_key_aqui
     ```

4. Inicia el servidor backend:
   ```bash
   # Si tienes configurado el script en package.json
   npm start

   # O directamente con Node.js
   node server.js
   ```
   El servidor debería estar ejecutándose en http://localhost:3001

5. Abre `index.html` en tu navegador:
   - Puedes abrir directamente el archivo HTML en tu navegador
   - O usar un servidor local como Live Server en VSCode

6. Interactúa con la aplicación:
   - Escribe tu mensaje en el campo de texto
   - Presiona Enter o haz clic en el botón de enviar
   - Espera la respuesta de la IA

## Configuración del Backend

Para usar esta aplicación, necesitas configurar un backend que maneje las peticiones a la API de OpenAI. El frontend está configurado para hacer peticiones a `http://localhost:3001/api/chat`.

**Nota importante:** Por razones de seguridad, nunca debes incluir tu API Key de OpenAI directamente en el código frontend.

## Recursos Adicionales

* [Guía paso a paso](./GUIA-PASO-A-PASO.md) - Explicación detallada del desarrollo
* [Convenciones de código](./README-CONVENCIONES.md) - Buenas prácticas de nombramiento y estructura
* [Documentación API de OpenAI](https://platform.openai.com/docs/guides/text?api-mode=chat)
* [Documentación de Fetch API](https://developer.mozilla.org/es/docs/Web/API/Fetch_API)


## Licencia

Este proyecto está bajo la licencia MIT.

