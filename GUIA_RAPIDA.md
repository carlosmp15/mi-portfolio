# 🎯 Guía Rápida de Personalización

## 📍 Archivos que DEBES personalizar:

### 1️⃣ **Hero Section** (`src/components/Hero.astro`)
```astro
Líneas a cambiar:
- Línea 10: "Tu Nombre" → Tu nombre real
- Línea 13: "Desarrollador Full Stack" → Tu título
- Línea 17-19: Descripción → Tu descripción personal
- Líneas 37-51: URLs de redes sociales
```

### 2️⃣ **Datos de Skills** (`src/data/skills.ts`)
```typescript
Personaliza las categorías e items con TUS habilidades reales
```

### 3️⃣ **Experiencia** (`src/data/experience.ts`)
```typescript
Agrega TU experiencia laboral real con:
- Puesto
- Empresa
- Período
- Descripción
- Tecnologías usadas
```

### 4️⃣ **Educación** (`src/data/education.ts`)
```typescript
Agrega TUS estudios y certificaciones
```

### 5️⃣ **Proyectos** (`src/data/projects.ts`)
```typescript
Agrega TUS proyectos con:
- Título
- Descripción
- Tecnologías
- Enlaces a GitHub y demo
- (Opcional) Ruta de imagen
```

### 6️⃣ **Contacto** (`src/components/Contact.astro`)
```astro
Líneas a cambiar:
- Línea 48: tu@email.com → Tu email real
- Línea 62: "Tu Ciudad, País" → Tu ubicación
- Líneas 76-88: URLs de redes sociales
```

### 7️⃣ **About Section** (`src/components/About.astro`)
```astro
Líneas 11-25: Personaliza tu descripción personal y estadísticas
```

## 🎨 Cambiar Colores

Si quieres cambiar el color principal (actualmente indigo):

1. **Buscar y reemplazar** en todos los archivos:
   - `indigo-600` → `tu-color-600` (ej: `blue-600`, `purple-600`, `green-600`)
   - `indigo-700` → `tu-color-700`
   - `indigo-500` → `tu-color-500`
   - etc.

2. Colores disponibles en Tailwind:
   - slate, gray, zinc, neutral, stone
   - red, orange, amber, yellow, lime, green
   - emerald, teal, cyan, sky, blue, indigo
   - violet, purple, fuchsia, pink, rose

## 🖼️ Agregar Imágenes

### Para tu foto de perfil:
1. Guarda tu foto en `public/profile.jpg`
2. En `Hero.astro`, reemplaza las líneas 46-48 con:
```astro
<img src="/profile.jpg" alt="Tu Nombre" class="w-full h-full object-cover" />
```

### Para imágenes de proyectos:
1. Guarda imágenes en `public/projects/`
2. En `projects.ts`, agrega la ruta:
```typescript
image: '/projects/nombre-proyecto.jpg'
```

## 🚀 Comandos Esenciales

```bash
# Ver el portfolio en desarrollo
pnpm dev

# Construir para producción
pnpm build

# Vista previa de producción
pnpm preview
```

## ✅ Checklist de Personalización

- [ ] Cambiar nombre en Hero
- [ ] Cambiar título profesional
- [ ] Actualizar descripción personal
- [ ] Agregar tus skills reales
- [ ] Agregar tu experiencia laboral
- [ ] Agregar tu educación
- [ ] Agregar tus proyectos
- [ ] Cambiar email y ubicación
- [ ] Actualizar enlaces de redes sociales
- [ ] (Opcional) Agregar tu foto
- [ ] (Opcional) Agregar imágenes de proyectos
- [ ] Probar en navegador
- [ ] Verificar responsive en móvil

## 🎯 Acceso Rápido a URLs

Después de personalizar, las secciones estarán en:
- `http://localhost:4321/#inicio` - Hero
- `http://localhost:4321/#sobre-mi` - Sobre Mí
- `http://localhost:4321/#skills` - Habilidades
- `http://localhost:4321/#experiencia` - Experiencia
- `http://localhost:4321/#educacion` - Educación
- `http://localhost:4321/#proyectos` - Proyectos
- `http://localhost:4321/#contacto` - Contacto

---

💡 **Tip**: Empieza por los datos (archivos en `src/data/`) y luego personaliza las secciones visuales.
