Bot Asistente de IA para WhatsApp
Funcionalidades
Flujos de conversación automatizados para WhatsApp.
Integración con la API de asistente de OpenAI.
Agnóstico al proveedor de WhatsApp.
Respuestas automatizadas a preguntas frecuentes.
Recepción y respuesta de mensajes en tiempo real.
Seguimiento de interacciones con clientes.
Funcionalidad expandible a través de disparadores personalizados.
Primeros pasos
Clona este repositorio.
Instala las dependencias:
Copiar código
pnpm install
Configura tus variables de entorno en un archivo .env:
makefile
Copiar código
PORT=3008
ASSISTANT_ID=tu_id_de_asistente_openai
Ejecuta el servidor de desarrollo:
arduino
Copiar código
pnpm run dev
Uso de Docker (Recomendado)
Este proyecto incluye un Dockerfile para facilitar el despliegue y asegurar entornos consistentes. Para usar Docker:

Construye la imagen de Docker:
Copiar código
docker build -t whatsapp-ai-assistant .
Ejecuta el contenedor:
arduino
Copiar código
docker run -p 3008:3008 --env-file .env whatsapp-ai-assistant
Este método garantiza que la aplicación se ejecute en un entorno consistente en diferentes sistemas.

Uso
El bot está configurado en el archivo src/app.ts. Utiliza la librería BuilderBot para crear flujos y manejar los mensajes. El flujo principal de bienvenida se integra con el asistente de OpenAI para generar respuestas.

Licencia
Este proyecto es de código abierto y está disponible bajo la Licencia MIT.

Diseñado por FULLSYS TECNOLOGÍA SANTA MARTA.