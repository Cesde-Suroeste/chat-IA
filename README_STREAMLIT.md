# OpenRouter Chat - Streamlit Edition

Una aplicación de chat moderna y segura que utiliza los modelos LLM gratuitos de OpenRouter a través de una interfaz web intuitiva construida con Streamlit.

## 🚀 Características

### 🔒 **Seguridad**
- API keys almacenadas como variables de entorno
- Configuración específica por modelo
- Sin exposición de credenciales en el frontend

### 🤖 **Modelos Soportados**
- **Qwen 2.5 VL 72B** (131,072 tokens) - Modelo avanzado de visión-lenguaje
- **Gemma 3 27B** (131,072 tokens) - Modelo de Google optimizado para instrucciones
- **DeepSeek R1 Zero** (163,840 tokens) - Modelo de razonamiento de DeepSeek

### 🎨 **Interfaz de Usuario**
- Interfaz moderna y responsive con Streamlit
- Chat en tiempo real con historial
- Configuración avanzada de parámetros
- Estadísticas de chat en tiempo real
- Exportación de conversaciones en JSON

## 🛠️ Instalación y Uso

### Instalación Rápida

```bash
# 1. Navegar al directorio
cd openrouter-streamlit

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Ejecutar la aplicación
streamlit run app.py
```

### Acceso
- La aplicación se abrirá automáticamente en `http://localhost:8501`

## 🔧 Configuración

Las API keys ya están configuradas en el archivo `.env`:

- **Qwen**: `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`
- **Gemma**: `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`
- **DeepSeek**: `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`

## 🎮 Uso

1. Selecciona un modelo en la barra lateral
2. Ajusta los parámetros (temperatura, max tokens, top-p)
3. Escribe tu mensaje en el campo de chat
4. ¡Disfruta de la conversación!

## 🚀 Ventajas de Streamlit

- **Desarrollo Rápido**: Interfaz completa en un solo archivo Python
- **Reactivo**: Actualizaciones automáticas de la UI
- **Componentes Ricos**: Chat, sliders, métricas out-of-the-box
- **Fácil Despliegue**: Compatible con múltiples plataformas
- **Sin JavaScript**: Todo en Python, más fácil de mantener
