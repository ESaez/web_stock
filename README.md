# Web Stock - Chat con Claude AI

Una aplicación web desarrollada con React y TypeScript que incluye autenticación simulada y un chat integrado con Claude AI.

## 🚀 Características

- ✅ Autenticación mock (sin backend)
- 💬 Chat integrado con Claude AI
- 🎨 Interfaz moderna con Material-UI (MUI)
- 🔒 Rutas protegidas con React Router
- 📱 Diseño responsive
- 💾 Persistencia de sesión con localStorage

## 🛠️ Tecnologías

- React 18
- TypeScript
- Vite
- Material-UI (MUI)
- React Router DOM
- Anthropic SDK (Claude AI)

## 📋 Requisitos Previos

- Node.js (v16 o superior)
- npm o yarn
- API Key de Anthropic (Claude AI)

## ⚙️ Instalación

1. Clona el repositorio (ya hecho)

2. Instala las dependencias:
```bash
npm install
```

3. Configura tu API Key de Anthropic:
   - Abre el archivo `.env.local`
   - Reemplaza `tu_api_key_aqui` con tu API Key real de Anthropic
   - Puedes obtener una en: https://console.anthropic.com/

```env
VITE_ANTHROPIC_API_KEY=tu_api_key_real_aqui
```

## 🚀 Ejecución

Inicia el servidor de desarrollo:

```bash
npm run dev
```

La aplicación estará disponible en `http://localhost:5173`

## 👤 Credenciales de Prueba

Para iniciar sesión, usa cualquiera de estas credenciales:

- **Usuario:** admin | **Contraseña:** admin123
- **Usuario:** user | **Contraseña:** user123

## 📁 Estructura del Proyecto

```
src/
├── components/       # Componentes reutilizables
│   └── PrivateRoute.tsx
├── contexts/         # Contextos de React
│   └── AuthContext.tsx
├── pages/           # Páginas de la aplicación
│   ├── LoginPage.tsx
│   └── ChatPage.tsx
├── types/           # Definiciones de TypeScript
│   └── index.ts
├── App.tsx          # Componente principal
└── main.tsx         # Punto de entrada
```

## 🔐 Funcionalidades de Autenticación

- Sistema de autenticación simulado sin backend
- Validación de credenciales con usuarios predefinidos
- Persistencia de sesión en localStorage
- Protección de rutas con PrivateRoute
- Redirección automática según estado de autenticación

## 💬 Funcionalidades del Chat

- Interfaz de chat moderna con Material-UI
- Integración con Claude AI (Anthropic)
- Historial de mensajes en tiempo real
- Indicadores de carga durante las respuestas
- Scroll automático a nuevos mensajes
- Manejo de errores de API

## ⚠️ Nota Importante

Este proyecto usa `dangerouslyAllowBrowser: true` en el SDK de Anthropic para propósitos de desarrollo. En producción, se recomienda hacer las llamadas a la API desde un backend para proteger tu API Key.

## 📝 Próximos Pasos

- [ ] Implementar backend real para autenticación
- [ ] Mover las llamadas a la API de Claude al backend
- [ ] Agregar más funcionalidades al chat (subir archivos, etc.)
- [ ] Implementar tests unitarios
- [ ] Agregar más temas y personalización de UI

## 📄 Licencia

MIT

