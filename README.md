# 🐱 Gaticos — Galería de Razas con React + Vite

Aplicación web desarrollada como laboratorio introductorio a React, que muestra una galería interactiva de razas de gatos con imágenes, videos y fichas técnicas servidas desde **Azure Blob Storage**.

---

## 📋 Descripción

La app renderiza una colección de 8 razas felinas en tarjetas visuales. Cada tarjeta permite al usuario marcar el gato como favorito (❤️), y al hacer clic abre un modal con imagen ampliada, video y un enlace a la ficha técnica en PDF. El conteo de favoritos se muestra dinámicamente en la parte superior de la galería.

---

## 🧱 Estructura del proyecto
```
src/
├── components/
│   ├── catCard.jsx       # Tarjeta visual de cada raza (componente presentacional)
│   └── catDetail.jsx     # Modal con detalle completo: imagen, video y PDF
├── hooks/
│   └── useCats.js        # Hook personalizado con toda la lógica de estado
├── pages/
│   └── Gallery.jsx       # Página principal que compone los componentes
├── services/
│   └── catService.js     # Construcción de URLs y datos de las razas
├── styles/
│   └── gallery.css       # Estilos principales de la galería y modal
├── App.jsx               # Componente raíz
└── main.jsx              # Punto de entrada de la aplicación
```

---

## ⚙️ Tecnologías

- **React 19** — librería de interfaces de usuario
- **Vite 7** — bundler y servidor de desarrollo
- **Tailwind CSS 4** — utilidades de estilos
- **TanStack React Query 5** — gestión de estado asíncrono (disponible como dependencia)
- **Azure Blob Storage** — almacenamiento externo de imágenes, videos y PDFs

---

## 🚀 Cómo correr el proyecto
```bash
# 1. Instalar dependencias
npm install

# 2. Configurar variable de entorno
# Crea un archivo .env en la raíz con:
VITE_AZURE_STORAGE_URL=https://tu-cuenta.blob.core.windows.net

# 3. Iniciar el servidor de desarrollo
npm run dev
```

---

## 🔧 Scripts disponibles

| Comando | Descripción |
|---|---|
| `npm run dev` | Inicia el servidor de desarrollo con HMR |
| `npm run build` | Genera el build de producción |
| `npm run preview` | Vista previa del build de producción |
| `npm run lint` | Ejecuta ESLint sobre el código fuente |

---

## 🗂️ Funcionalidades

- Galería en
