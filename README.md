# 🤖 Chatbot asistente virtual y traductor
Este proyecto es una API REST basada en FastAPI que funciona como un asistente virtual que te da las respuestas a todas tus preguntas acerca de la universidad e ingles. Utiliza el modelo Mistral a través de OpenRouter (compatible con la API de OpenAI) para generar respuestas conversacionales.

## 🚀 Requisitos
- Python 3.8 o superior
- Tener una API Key de OpenRouter
- Conexión a internet

## 🛠 Instalación
1. Clona este repositorio o descarga los archivos
2. Crea un entorno virtual:
```
python -m venv venv  
Activa el entorno virtual:

Windows: venv\Scripts\activate

macOS/Linux: source venv/bin/activate

Instala las dependencias:

pip install -r requirements.txt  
Crea un archivo .env en la raíz del proyecto con:

API_KEY=tu_api_key_de_openrouter  
BASE_URL=https://openrouter.ai/api/v1  
▶ Ejecución
Inicia el servidor con:

uvicorn main:app --reload  
API disponible en: http://127.0.0.1:8000

Documentación Swagger UI: http://127.0.0.1:8000/docs

📬 Ejemplo de uso
Petición POST a /chat:

{"pregunta": "¿cual es la traduccion de la palabra levitar en ingles?"}  
Respuesta esperada:

{"respuesta": "la traduccion de la palabra es levitade "}  

📁 Estructura del proyecto
chatbot-ia_python/  
├── chatbot.py           # API con FastAPI  
├── config.py         # Contiene el PROMPT_SISTEMA  
├── .env              # Variables de entorno  
├── requirements.txt  # Dependencias  
├── Dockerfile        # Configuración para Docker  
├── frontend/         # Interfaz web para el chatbot  
│   ├── index.html    # Estructura HTML  
│   ├── style.css     # Estilos modernos (Glassmorphism + Python theme)  
│   └── script.js     # Lógica de chat, efectos y temporizadores  
└── README.md  

💬 Interfaz Web del Chatbot
El proyecto incluye una interfaz web moderna y funcional para interactuar visualmente con la API:

✨ Funcionalidades del frontend
💎 Diseño basico

🎨 colores de la universidad: colores blanco y verde inspirados en la universidad simon bolivar

⌨️ Tipografía técnica: uso de fuente original 'MERCY'

💬 Mensajes organizados: estilo chat con diferenciación clara entre el usuario y el bot.

🕒 Temporizadores de inactividad:

A los 2 minutos sin interacción se muestra una alerta.

A los 5 minutos el chat se limpia automáticamente.

✍️ Efecto "escribiendo...": simula la respuesta del bot en tiempo real.

🔄 Soporte CORS habilitado para comunicación frontend-backend.

▶ Cómo usarlo
Asegúrate de que el backend esté en ejecución (uvicorn main:app --reload)

Abre el archivo frontend/index.html en tu navegador

Pregunta lo que quieras sobre Python 😄
```
---

👤 Autor:
Desarrollado por desarrolador diego diaz

---

