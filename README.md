# 🛍️ Shop_html_css

Proyecto de maquetación responsive de una tienda en línea moderna, implementada con HTML5 y CSS3 puro, siguiendo las mejores prácticas de diseño web y los principios de Mobile First.

## ✨ Características

### 🎨 Diseño
- 📱 Diseño totalmente responsive
- 🎯 Basado en un diseño de Figma
- 🖼️ Layout moderno con grid y flexbox
- 🎭 Animaciones y transiciones suaves
- 📦 Componentes reutilizables

### 🛠️ Tecnologías
- **HTML5 Semántico**
- **CSS3 Moderno**
- **Normalize.css**
- **Google Fonts** (Roboto)
- **CSS Grid & Flexbox**
- **BEM Methodology**

### 📱 Componentes
1. **Header**
   - Logo de la marca
   - Navegación principal
   - Botón de contacto
   - Menú responsive

2. **Sección Principal**
   - Galería de productos
   - Chips de categorías
   - Precios y descuentos
   - Imágenes de productos

3. **Sección de Recomendados**
   - Productos relacionados
   - Precios y etiquetas
   - Navegación de productos

4. **Sección de Sorteo**
   - Formulario de participación
   - Diseño llamativo
   - Call-to-action

5. **Footer**
   - Copyright
   - Enlaces legales
   - Información de contacto

## 🎯 Metodologías Implementadas

### 🔷 BEM (Block Element Modifier)
```css
.block {}
.block__element {}
.block--modifier {}
```

### 🔷 Arquitectura CSS
- Normalización
- Variables CSS
- Componentes modulares
- Utilidades

### 🔷 Buenas Prácticas
- HTML semántico
- CSS reutilizable
- Nombres descriptivos
- Comentarios claros

## 🌓 Modo Oscuro

### Características
- 🎨 Temas claro y oscuro completamente personalizados
- 🔄 Cambio automático según preferencias del sistema
- 💾 Persistencia de la preferencia del usuario
- 🎭 Transiciones suaves entre temas
- 🖱️ Botón de cambio manual en la navegación

### Implementación Técnica

#### Variables CSS
```css
:root {
  /* Tema Claro (default) */
  --color-bg: #ffffff;
  --color-text: #333333;
  /* ... más variables ... */
}

/* Tema Oscuro */
[data-theme="dark"] {
  --color-bg: #1a1a1a;
  --color-text: #e5e7eb;
  /* ... más variables ... */
}
```

#### JavaScript para Control de Tema
```javascript
// Obtener tema guardado o preferencia del sistema
const currentTheme = localStorage.getItem('theme') || 
                    (prefersDarkScheme.matches ? 'dark' : 'light');

// Aplicar tema
document.documentElement.setAttribute('data-theme', currentTheme);
```

### Uso del Modo Oscuro

1. **Cambio Automático**
   - El tema se ajusta automáticamente según las preferencias del sistema
   - Detecta cambios en tiempo real en la configuración del sistema

2. **Cambio Manual**
   - Usa el botón 🌞/🌙 en la navegación
   - El tema seleccionado se guarda y persiste entre sesiones

3. **Personalización**
   - Modifica las variables CSS en `style.css` para ajustar colores
   - Añade nuevas variables según necesidades
   - Personaliza las transiciones y animaciones

### Estructura de Archivos Modificados

```
Shop_html_css/
├── index.html      # Agregado botón de tema y script
├── style.css       # Nuevas variables y estilos de tema
└── README.md       # Documentación actualizada
```

### Cambios Realizados

1. **HTML (`index.html`)**
   - Agregado botón de cambio de tema en la navegación
   - Implementado script para gestión del tema
   - Añadidos atributos de accesibilidad

2. **CSS (`style.css`)**
   - Definidas variables para ambos temas
   - Implementadas clases de tema
   - Añadidas transiciones suaves
   - Estilos adaptados para modo oscuro

3. **JavaScript**
   - Gestión de preferencias del usuario
   - Persistencia en localStorage
   - Detección de preferencias del sistema
   - Manejo de eventos de cambio

### Mejoras Futuras
- [ ] Añadir más variantes de tema
- [ ] Implementar transiciones personalizadas por componente
- [ ] Mejorar accesibilidad del selector de tema
- [ ] Agregar prefers-reduced-motion
- [ ] Optimizar rendimiento de transiciones

## 💻 Uso

1. Clona el repositorio:
```bash
git clone https://github.com/tuusuario/Shop_html_css.git
```

2. Abre `index.html` en tu navegador

## 🎨 Estilos

### Variables CSS
```css
:root {
  /* Colores */
  --color-primary: #...;
  --color-secondary: #...;
  
  /* Espaciado */
  --spacing-sm: 8px;
  --spacing-md: 16px;
  --spacing-lg: 24px;
  
  /* Tipografía */
  --font-primary: 'Roboto', sans-serif;
}
```

### Breakpoints
```css
/* Mobile First */
@media (min-width: 768px) {
  /* Tablet */
}

@media (min-width: 1024px) {
  /* Desktop */
}
```

## 📱 Responsive Design

- Mobile First approach
- Breakpoints estratégicos
- Imágenes flexibles
- Grid responsive
- Menú adaptativo

## 🚀 Optimizaciones

- Imágenes optimizadas
- CSS minificado
- HTML limpio
- Fuentes optimizadas
- Rendimiento mejorado

## 👤 Autor

**SatruxDev**
- Website: [satruxdev.com](https://satruxdev.com)
- GitHub: [@satruxdev](https://github.com/satruxdev)

## 📝 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 🎯 TODOs

- [ ] Agregar más animaciones
- [ ] Implementar dark mode
- [ ] Mejorar accesibilidad
- [ ] Optimizar imágenes
- [ ] Agregar más interactividad
