# LocalChat AI

LocalChat AI es una colección de aplicaciones de chat local construidas con **Python**, **Chainlit** y **Ollama**.

El objetivo es ofrecer asistentes de inteligencia artificial que funcionen **completamente en local**, sin depender de APIs externas.

El repositorio incluye dos aplicaciones:

- **Chat conversacional** usando el modelo `deepseek-r1:7b`
- **Chat multimodal con visión** usando el modelo `llama3.2-vision`

---

# Características

- IA ejecutándose **100% en local**
- Integración sencilla con **Ollama**
- Interfaz web con **Chainlit**
- Soporte para **streaming de respuestas**
- Soporte para **análisis de imágenes** en el modo visión

---

# Estructura del proyecto

```
.
├── localchat-deepseek.py
├── localchat-vision.py
└── README.md
```

---

# Requisitos

Antes de ejecutar las aplicaciones necesitas:

- Python 3.10 o superior
- Ollama instalado
- Chainlit

---

# Instalación

## 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/localchat-ai.git
cd localchat-ai
```

---

## 2. Crear entorno virtual

### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
```

---

## 3. Instalar dependencias

```bash
pip install chainlit ollama
```

---

# Descargar los modelos

Antes de ejecutar las aplicaciones debes descargar los modelos con Ollama.

## Modelo conversacional

```bash
ollama pull deepseek-r1:7b
```

## Modelo multimodal con visión

```bash
ollama pull llama3.2-vision
```

---

# Aplicaciones incluidas

## 1. Chat conversacional (DeepSeek)

Aplicación de chat basada en el modelo **DeepSeek R1 7B** que permite mantener conversaciones completamente en local.

### Ejecutar

```bash
chainlit run localchat-deepseek.py
```

### Funcionalidades

- chat interactivo
- historial de conversación
- respuestas en streaming
- ejecución local con Ollama

---

## 2. Chat multimodal con visión

Aplicación de chat que permite enviar **texto e imágenes** al modelo **Llama 3.2 Vision** para obtener análisis visual y respuestas inteligentes.

### Ejecutar

```bash
chainlit run localchat-vision.py
```

### Funcionalidades

- chat con imágenes
- análisis visual
- respuestas multimodales
- streaming de respuestas

---

# Uso recomendado

Este repositorio está pensado para:

- aprender a integrar **LLMs locales**
- crear asistentes privados sin depender de APIs
- prototipar aplicaciones con **Ollama**
- desarrollar interfaces de chat con **Chainlit**

---

# Posibles mejoras

- añadir selector de modelos
- crear interfaz única con selector de modo (texto / visión)
- añadir system prompts configurables
- dockerizar la aplicación
- añadir soporte para más modelos de Ollama

---

# Licencia

Puedes añadir una licencia como **MIT** para permitir uso libre del proyecto.
