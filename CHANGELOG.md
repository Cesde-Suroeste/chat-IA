# 📋 Changelog - Chat IA

Registro de cambios y mejoras del proyecto.

## [v2.0.0] - 2025-01-23

### 🎉 Nuevas Características

#### **🤖 Modelos Ampliados**
- ✅ **5 modelos LLM disponibles** (anteriormente 3)
- ✅ **Qwen 2.5 VL 72B** - Modelo principal de visión-lenguaje
- ✅ **Gemma 3N E4B** - Modelo de Google optimizado
- ✅ **DeepSeek R1 Zero** - Modelo de razonamiento matemático
- ✅ **Llama 3.2 3B** - Modelo rápido y eficiente de Meta
- ✅ **Gemma 2 9B** - Modelo compacto de Google

#### **☁️ Compatibilidad con Streamlit Cloud**
- ✅ **Función híbrida `get_env_var()`** - Compatible con desarrollo local y Streamlit Cloud
- ✅ **Soporte para `st.secrets`** - Variables de entorno en la nube
- ✅ **Documentación completa** de despliegue en Streamlit Cloud
- ✅ **Archivos de ejemplo** para configuración de secrets

#### **🚀 Scripts de Instalación Automática**
- ✅ **4 scripts diferentes** según nivel de usuario
- ✅ **install_and_run.bat** - Instalador completo con interfaz visual
- ✅ **quick_install.bat** - Instalación rápida de una línea
- ✅ **run.bat** - Ejecutor para uso diario
- ✅ **install_and_run.ps1** - Versión PowerShell con parámetros

### 🔧 Mejoras Técnicas

#### **🔌 Gestión de Puertos**
- ✅ **Detección automática** de puertos ocupados
- ✅ **Configuración flexible** de puertos (8501, 8502, 80, etc.)
- ✅ **Soporte para puerto 80** con permisos de administrador
- ✅ **Múltiples instancias** simultáneas

#### **🛡️ Seguridad Mejorada**
- ✅ **Variables de entorno protegidas** - .env en .gitignore
- ✅ **Archivos de ejemplo seguros** - Sin credenciales reales
- ✅ **Documentación de buenas prácticas** de seguridad
- ✅ **Formato TOML** para Streamlit Cloud

#### **📚 Documentación Completa**
- ✅ **README.md actualizado** con instrucciones detalladas
- ✅ **Ejemplos prácticos** para diferentes tipos de usuarios
- ✅ **Solución de problemas** específicos
- ✅ **Guías paso a paso** para Windows 11

### 🐛 Correcciones

#### **🔑 API Keys**
- ✅ **Credenciales actualizadas** - Nuevas API keys funcionales
- ✅ **Modelo Gemma corregido** - `google/gemma-3n-e4b-it:free`
- ✅ **HTTP-Referer actualizado** - URL correcta del repositorio
- ✅ **Manejo de errores mejorado** - Mensajes más claros

#### **🧹 Código Limpio**
- ✅ **Removidos mensajes de debug** - Interfaz más limpia
- ✅ **Eliminado modo demo** - Solo funcionalidad real
- ✅ **Modelos no disponibles removidos** - Solo modelos funcionales
- ✅ **Optimización de funciones** - Código más eficiente

### 📊 Estadísticas

#### **Antes (v1.0.0)**
- 3 modelos LLM
- Solo desarrollo local
- Instalación manual
- Documentación básica

#### **Ahora (v2.0.0)**
- 5 modelos LLM ✅
- Compatible con Streamlit Cloud ✅
- Instalación automática ✅
- Documentación completa ✅

### 🎯 Casos de Uso Soportados

#### **👨‍💻 Desarrolladores**
- Instalación rápida con scripts
- Múltiples puertos configurables
- Desarrollo local y despliegue en la nube

#### **🎓 Estudiantes**
- Instrucciones paso a paso
- Scripts con interfaz visual
- Documentación en español

#### **🏢 Empresas**
- Puerto 80 para servidores web
- Configuración de proxy corporativo
- Múltiples instancias simultáneas

#### **☁️ Despliegue en la Nube**
- Streamlit Cloud listo
- Heroku compatible
- Railway y Render soportados

### 🔮 Próximas Características

#### **En Desarrollo**
- [ ] Más modelos LLM gratuitos
- [ ] Interfaz de configuración visual
- [ ] Exportación de chats en más formatos
- [ ] Temas personalizables

#### **Considerando**
- [ ] Soporte para imágenes (modelos de visión)
- [ ] Chat con archivos PDF
- [ ] Integración con bases de datos
- [ ] API REST propia

---

## [v1.0.0] - 2025-01-22

### 🎉 Lanzamiento Inicial
- ✅ Aplicación Streamlit básica
- ✅ 3 modelos LLM (Qwen, Gemma, DeepSeek)
- ✅ Chat en tiempo real
- ✅ Configuración de parámetros
- ✅ Exportación de conversaciones

---

**¡Gracias por usar Chat IA!** 🎊
