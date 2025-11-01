# 🎨 Portfolio Personal

Portfolio profesional desarrollado con Astro y Tailwind CSS. Diseño moderno, responsivo y totalmente personalizable.

## ✨ Características

- ✅ **Diseño moderno y responsivo** - Se adapta perfectamente a todos los dispositivos
- ✅ **Navegación sticky** con scroll suave
- ✅ **Secciones completas**: Hero, Sobre Mí, Skills, Experiencia, Educación, Proyectos, Contacto
- ✅ **Modo oscuro** compatible
- ✅ **Animaciones suaves** y transiciones
- ✅ **Optimizado para SEO**
- ✅ **Totalmente personalizable**

## 🚀 Estructura del Proyecto

```
/
├── public/              # Archivos estáticos
├── src/
│   ├── components/      # Componentes de Astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Skills.astro
│   │   ├── Experience.astro
│   │   ├── Education.astro
│   │   ├── Projects.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── data/           # Datos del portfolio
│   │   ├── skills.ts
│   │   ├── experience.ts
│   │   ├── education.ts
│   │   └── projects.ts
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
└── package.json
```

## 📝 Personalización

### 1. Información Personal

Edita el componente `src/components/Hero.astro` para cambiar:
- Tu nombre
- Título profesional
- Descripción
- Enlaces de redes sociales
- Email

### 2. Skills

Edita `src/data/skills.ts` para agregar o modificar tus habilidades:

```typescript
export const skills = [
  {
    category: 'Frontend',
    icon: '🎨',
    items: ['React', 'Vue.js', 'Astro', 'TypeScript', 'Tailwind CSS']
  },
  // Agrega más categorías...
];
```

### 3. Experiencia Profesional

Edita `src/data/experience.ts`:

```typescript
export const experience = [
  {
    position: 'Tu Puesto',
    company: 'Nombre de la Empresa',
    period: '2022 - Presente',
    description: 'Descripción de tus responsabilidades',
    technologies: ['Tech1', 'Tech2', 'Tech3']
  },
  // Agrega más experiencias...
];
```

### 4. Educación

Edita `src/data/education.ts`:

```typescript
export const education = [
  {
    degree: 'Tu Título',
    institution: 'Universidad/Institución',
    period: '2014 - 2018',
    description: 'Descripción opcional'
  },
  // Agrega más estudios...
];
```

### 5. Proyectos

Edita `src/data/projects.ts`:

```typescript
export const projects = [
  {
    title: 'Nombre del Proyecto',
    description: 'Descripción breve del proyecto',
    technologies: ['React', 'Node.js', 'MongoDB'],
    image: '/ruta/a/imagen.jpg', // Opcional
    github: 'https://github.com/usuario/repo',
    demo: 'https://demo.com' // Opcional
  },
  // Agrega más proyectos...
];
```

### 6. Colores y Estilos

Los colores principales están en `tailwind.config.js` y `src/styles/global.css`. 
Para cambiar el color principal de indigo a otro:

1. Busca y reemplaza `indigo` por el color que prefieras en todos los componentes
2. O personaliza los colores en `tailwind.config.js`

### 7. Información de Contacto

Edita `src/components/Contact.astro` para cambiar:
- Email
- Ubicación
- Enlaces de redes sociales

## 🛠️ Comandos

```bash
# Instalar dependencias
pnpm install

# Iniciar servidor de desarrollo
pnpm dev

# Construir para producción
pnpm build

# Vista previa de producción
pnpm preview
```

## 📦 Deployment

Este proyecto se puede desplegar en:

- **Vercel**: Conecta tu repositorio y despliega automáticamente
- **Netlify**: Similar a Vercel
- **GitHub Pages**: Usando GitHub Actions
- **Cloudflare Pages**: Otra opción rápida y gratuita

### Ejemplo para Vercel:

```bash
pnpm build
# Luego sube la carpeta dist/ a Vercel
```

## 🎨 Personalización Avanzada

### Agregar más secciones

1. Crea un nuevo componente en `src/components/`
2. Importa y agrega el componente en `src/pages/index.astro`
3. Agrega un enlace en el Header si es necesario

### Agregar imágenes

1. Coloca las imágenes en la carpeta `public/`
2. Refiérelas en tus componentes: `<img src="/imagen.jpg" />`

### Modo oscuro

El portfolio ya soporta modo oscuro. Puedes agregar un toggle agregando este código al Header:

```astro
<button id="theme-toggle" class="...">
  <!-- Iconos de sol/luna -->
</button>

<script>
  const toggle = document.getElementById('theme-toggle');
  toggle?.addEventListener('click', () => {
    document.documentElement.classList.toggle('dark');
  });
</script>
```

## 📱 Responsividad

El diseño es completamente responsivo y se adapta a:
- 📱 Móviles (< 768px)
- 📱 Tablets (768px - 1024px)
- 💻 Desktop (> 1024px)

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si encuentras algún bug o tienes sugerencias:

1. Fork el proyecto
2. Crea una rama (`git checkout -b feature/mejora`)
3. Commit tus cambios (`git commit -m 'Agrega nueva característica'`)
4. Push a la rama (`git push origin feature/mejora`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Siéntete libre de usarlo para tu portfolio personal.

## 💡 Tips

- Mantén las descripciones concisas y enfocadas en resultados
- Usa imágenes de alta calidad para tus proyectos
- Actualiza regularmente con nuevos proyectos y experiencias
- Optimiza las imágenes antes de subirlas (usa formatos webp cuando sea posible)
- Prueba tu portfolio en diferentes dispositivos y navegadores
- Considera agregar Google Analytics para rastrear visitantes

## 🎯 Próximas Mejoras

- [ ] Agregar animaciones al hacer scroll
- [ ] Implementar formulario de contacto funcional
- [ ] Agregar blog integrado
- [ ] Implementar i18n (internacionalización)
- [ ] Agregar más temas de color
- [ ] Integrar CMS para gestión de contenido

---

Hecho con ❤️ usando [Astro](https://astro.build) y [Tailwind CSS](https://tailwindcss.com)
