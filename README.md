# 🌿 Santa Lucía — Landing Page Institucional
### Barrio privado dentro del masterplan **Pilar del Este**

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-22c55e?style=flat-square&logo=github)](https://pages.github.com/)
[![HTML5](https://img.shields.io/badge/HTML5-Semántico-e34f26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-CDN-06b6d4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

---

## 📋 Descripción del Proyecto

Landing page institucional para el **Barrio Santa Lucía**, uno de los barrios consolidados del masterplan Pilar del Este (RP 25, km 46, Pilar, Buenos Aires). El sitio presenta la oferta residencial, infraestructura, amenities y canales de contacto del barrio de manera clara y elegante.

Desarrollada con foco en:
- Diseño editorial premium con paleta natural (verdes sage + neutros cálidos)
- Tipografía de alta jerarquía (Cormorant Garamond + DM Sans)
- Experiencia 100% responsive (mobile-first)
- Animaciones CSS suaves y scroll-triggered

---

## 🗂 Estructura del Repositorio

```
santa-lucia/
├── index.html          ← Página principal (único archivo HTML)
├── README.md           ← Este archivo
└── assets/             ← Carpeta de recursos de imágenes
    ├── hero-santa-lucia.jpg    (Hero a pantalla completa)
    ├── galeria-aerea.jpg       (Vista aérea del barrio)
    ├── galeria-sum.jpg         (Club House / SUM)
    ├── galeria-deportes.jpg    (Canchas deportivas)
    └── galeria-entorno.jpg     (Boulevard y entorno)
```

> ⚠️ **Importante:** Las imágenes de la carpeta `assets/` deben ser añadidas manualmente al repositorio. El HTML referencia imágenes locales con rutas relativas.

---

## 🛠 Tecnologías Utilizadas

| Tecnología | Versión / Canal | Rol |
|---|---|---|
| **HTML5** | Semántico | Estructura y contenido |
| **Tailwind CSS** | CDN oficial (v3) | Estilos y layout responsive |
| **Google Fonts** | CDN | Tipografías Cormorant Garamond + DM Sans |
| **JavaScript Vanilla** | ES6+ inline | Menú mobile, navbar scroll, animaciones |

**Sin build tools. Sin dependencias npm. Sin frameworks.** El proyecto es 100% estático y se puede desplegar directamente.

---

## 🚀 Cómo Activar GitHub Pages

### Paso 1 — Crear el repositorio

1. Crear un repositorio nuevo en GitHub (ej: `santa-lucia-pilar`)
2. Clonar localmente:
   ```bash
   git clone https://github.com/tu-usuario/santa-lucia-pilar.git
   cd santa-lucia-pilar
   ```

### Paso 2 — Subir los archivos

```bash
# Copiar index.html, README.md y la carpeta assets/ al directorio del repo
cp index.html README.md ./
cp -r assets/ ./assets/

# Confirmar y subir
git add .
git commit -m "feat: landing page inicial Santa Lucía"
git push origin main
```

### Paso 3 — Activar GitHub Pages

1. Ir a **Settings** → **Pages** en el repositorio de GitHub
2. En **Source**, seleccionar:
   - Branch: `main`
   - Folder: `/ (root)`
3. Hacer clic en **Save**
4. En unos minutos el sitio estará disponible en:
   ```
   https://tu-usuario.github.io/santa-lucia-pilar/
   ```

---

## ✏️ Personalización

### Imágenes
Reemplazar los archivos en `assets/` con fotografías reales del barrio:

```
assets/hero-santa-lucia.jpg  → Foto aérea / panorámica de alta resolución (1920×1080 mín.)
assets/galeria-aerea.jpg     → Vista aérea del trazado
assets/galeria-sum.jpg       → Club House y sector de parrillas
assets/galeria-deportes.jpg  → Canchas deportivas
assets/galeria-entorno.jpg   → Boulevard o calle principal
```

### Datos de contacto
Actualizar en el HTML la sección `#contacto` con los números y correos reales de Administración Urbis / Eidico.

### Colores
El tema de color está definido en la configuración de Tailwind dentro del `<head>`:
```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        'sage': { ... },   // Verde principal
        'stone': { ... },  // Grises neutros
        'cream': '#faf8f4' // Fondo cálido
      }
    }
  }
}
```

---

## 📄 Licencia

Proyecto de referencia institucional. Contenido sujeto a la disponibilidad y términos de **Eidico / Urbis / Pilar del Este**.

---

*Desarrollado con HTML5 + Tailwind CSS · Barrio Santa Lucía, Pilar del Este*
