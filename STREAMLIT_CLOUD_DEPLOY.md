# 🚀 Despliegue en Streamlit Cloud

Guía completa para desplegar Chat IA en Streamlit Cloud.

## 📋 Requisitos Previos

- ✅ Cuenta en [Streamlit Cloud](https://share.streamlit.io/)
- ✅ Repositorio en GitHub (ya tienes: `https://github.com/Cesde-Suroeste/chat-IA`)
- ✅ API keys de OpenRouter (ya configuradas en el proyecto)

## 🚀 Pasos para Desplegar

### **PASO 1: Acceder a Streamlit Cloud**

1. Ve a [share.streamlit.io](https://share.streamlit.io/)
2. Inicia sesión con tu cuenta de GitHub
3. Haz clic en "New app"

### **PASO 2: Configurar la Aplicación**

1. **Repository**: `Cesde-Suroeste/chat-IA`
2. **Branch**: `main`
3. **Main file path**: `app.py`
4. **App URL** (opcional): Personaliza la URL de tu aplicación

### **PASO 3: Configurar Secrets (Variables de Entorno)**

1. **Antes de hacer deploy**, haz clic en "Advanced settings"
2. En la sección **"Secrets"**, pega exactamente esto:

```toml
# OpenRouter API Keys
QWEN_API_KEY = "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"
GEMMA_API_KEY = "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"
DEEPSEEK_API_KEY = "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"

# OpenRouter Configuration
OPENROUTER_BASE_URL = "https://openrouter.ai/api/v1"
DEFAULT_API_KEY = "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"

# App Configuration
APP_TITLE = "OpenRouter Chat Application"
APP_ICON = "🤖"
DEFAULT_MODEL = "qwen/qwen2.5-vl-72b-instruct:free"
```

### **PASO 4: Desplegar**

1. Haz clic en **"Deploy!"**
2. Espera a que se complete el despliegue (2-5 minutos)
3. ¡Tu aplicación estará disponible en la URL generada!

## 🔧 Configuración Avanzada

### **Python Version**
Si necesitas especificar la versión de Python, crea un archivo `.python-version`:
```
3.11
```

### **Dependencias Adicionales**
El archivo `requirements.txt` ya está configurado correctamente:
```
streamlit>=1.28.0
requests>=2.31.0
python-dotenv>=1.0.0
```

## 🔒 Seguridad en Streamlit Cloud

### **✅ Buenas Prácticas:**
- ✅ Las API keys están encriptadas en Streamlit Cloud
- ✅ Solo tu aplicación puede acceder a los secrets
- ✅ Los secrets no son visibles en los logs
- ✅ Puedes actualizar secrets sin redeployar

### **🔄 Actualizar Secrets:**
1. Ve a tu aplicación en Streamlit Cloud
2. Haz clic en "Settings" → "Secrets"
3. Modifica los valores
4. Los cambios se aplican automáticamente en ~1 minuto

## 🌐 URLs de Ejemplo

Después del despliegue, tu aplicación estará disponible en:
- `https://chat-ia-cesde-suroeste.streamlit.app/`
- `https://cesde-suroeste-chat-ia-app-xyz123.streamlit.app/`

## 🔧 Solución de Problemas

### **Error: "ModuleNotFoundError"**
- Verifica que todas las dependencias estén en `requirements.txt`
- Asegúrate de que las versiones sean compatibles

### **Error: "KeyError" en secrets**
- Verifica que todos los secrets estén configurados correctamente
- Asegúrate de usar el formato TOML exacto
- No uses comillas simples, solo comillas dobles

### **Error: "API Error 401"**
- Verifica que las API keys sean válidas
- Asegúrate de que no haya espacios extra en los secrets

### **La aplicación no carga**
- Revisa los logs en Streamlit Cloud
- Verifica que el archivo `app.py` esté en la raíz del repositorio
- Asegúrate de que la rama sea `main`

## 📊 Monitoreo

### **Ver Logs:**
1. Ve a tu aplicación en Streamlit Cloud
2. Haz clic en "Manage app"
3. Ve a la pestaña "Logs"

### **Métricas de Uso:**
- Streamlit Cloud proporciona métricas básicas de uso
- Puedes ver el número de visitantes y uso de recursos

## 🔄 Actualizaciones

### **Actualización Automática:**
- Cada push a la rama `main` actualiza automáticamente la aplicación
- Los cambios se reflejan en 1-2 minutos

### **Actualización Manual:**
1. Ve a "Manage app"
2. Haz clic en "Reboot app"

## 🎯 Optimización para Streamlit Cloud

### **Rendimiento:**
- La aplicación está optimizada para Streamlit Cloud
- Usa caché de Streamlit para mejorar velocidad
- Las API keys se cargan eficientemente

### **Límites:**
- **CPU**: Compartido
- **RAM**: 1GB
- **Ancho de banda**: Ilimitado para uso normal
- **Tiempo de ejecución**: Sin límite

## 📞 Soporte

### **Problemas con Streamlit Cloud:**
- [Documentación oficial](https://docs.streamlit.io/streamlit-cloud)
- [Foro de la comunidad](https://discuss.streamlit.io/)

### **Problemas con la aplicación:**
- Abre un issue en [GitHub](https://github.com/Cesde-Suroeste/chat-IA/issues)
- Incluye los logs de Streamlit Cloud

---

**¡Disfruta de tu aplicación desplegada en la nube!** 🎉
