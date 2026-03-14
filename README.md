# 🚀 Agencia RapidWeb - Sitio Web Profesional

Sitio web completo, moderno y responsive para **Agencia RapidWeb**, especializada en desarrollo rápido de sitios web, aplicaciones móviles y sistemas a medida usando inteligencia artificial.

## ✨ Características

- ✅ Diseño minimalista y profesional
- ✅ 100% responsive (mobile-first)
- ✅ Colores corporativos: Azul (#0066FF, #00A3FF), grises y blanco
- ✅ Tipografía moderna: Google Fonts (Inter)
- ✅ Animaciones sutiles y transiciones
- ✅ SEO optimizado
- ✅ Solo HTML5, CSS3 y JavaScript vanilla (sin frameworks pesados)
- ✅ Formulario de contacto funcional
- ✅ Imágenes de Unsplash (placeholders profesionales)

## 📁 Estructura del Proyecto

```
agencia-rapidweb/
├── index.html              # Página de inicio
├── about.html              # Sobre Nosotros
├── services.html           # Servicios
├── portfolio.html          # Portafolio de proyectos
├── contact.html            # Contacto
├── css/
│   └── style.css           # Estilos principales
├── js/
│   └── script.js           # JavaScript funcional
├── img/                    # Carpeta para imágenes (actualmente usa Unsplash)
└── README.md               # Este archivo
```

## 🎨 Paleta de Colores

- **Azul Principal**: `#0066FF`
- **Azul Secundario**: `#00A3FF`
- **Gris Oscuro**: `#333`
- **Gris Medio**: `#666`
- **Gris Claro**: `#999`
- **Blanco**: `#FFFFFF`
- **Fondo Claro**: `#f8f9fa`

## 🚀 Despliegue Rápido

### Opción 1: Vercel (Recomendado)

1. Crea una cuenta en [Vercel](https://vercel.com)
2. Instala Vercel CLI:
   ```bash
   npm i -g vercel
   ```
3. Desde la carpeta del proyecto:
   ```bash
   cd agencia-rapidweb
   vercel
   ```
4. Sigue las instrucciones en pantalla
5. ¡Listo! Tu sitio estará online en menos de 1 minuto

**Opción alternativa (sin CLI):**
- Ve a [vercel.com/new](https://vercel.com/new)
- Arrastra y suelta la carpeta `agencia-rapidweb`
- ¡Desplegado!

### Opción 2: Netlify

1. Crea una cuenta en [Netlify](https://www.netlify.com)
2. Arrastra y suelta la carpeta `agencia-rapidweb` en el área de deploy
3. ¡Tu sitio estará online!

**Opción alternativa (con Git):**
```bash
# Sube el proyecto a GitHub
git init
git add .
git commit -m "Initial commit"
git remote add origin TU_REPO_URL
git push -u origin main

# Luego conecta el repo en Netlify
```

### Opción 3: GitHub Pages

1. Sube el proyecto a un repositorio de GitHub
2. Ve a Settings > Pages
3. Selecciona la rama `main` y carpeta `/ (root)`
4. Guarda y espera unos minutos
5. Tu sitio estará en: `https://TU_USUARIO.github.io/NOMBRE_REPO`

## ⚙️ Configuración Inicial

### 1. Cambiar el Email del Formulario

Edita `contact.html` en la línea 67:

```html
<!-- ANTES -->
<form action="https://formsubmit.co/hola@agenciarapidweb.com" method="POST">

<!-- DESPUÉS -->
<form action="https://formsubmit.co/TU_EMAIL@ejemplo.com" method="POST">
```

**Importante:** La primera vez que recibas un mensaje, FormSubmit te enviará un email de confirmación. Haz click en el link para activar el formulario.

### 2. Actualizar Datos de Contacto

Busca y reemplaza en **TODOS los archivos HTML**:

- `+54 9 XXX-XXXXXX` → Tu número de WhatsApp (ej: `+54 9 260-1234567`)
- `hola@agenciarapidweb.com` → Tu email real
- `@agenciarapidweb` → Tu usuario de Instagram
- `549XXXXXXXXX` → Tu número de WhatsApp SIN espacios ni guiones (ej: `5492601234567`)

**Tip:** Usa "Buscar y Reemplazar" en tu editor de código para hacerlo más rápido.

### 3. Reemplazar Logo e Imágenes

**Logo:**
- El logo actual es un SVG de un rayo/relámpago en azul
- Para cambiarlo, reemplaza el `<svg>` en el header de cada página HTML
- O crea un archivo `logo.png` y reemplaza el SVG por:
  ```html
  <img src="img/logo.png" alt="Agencia RapidWeb" class="logo-icon">
  ```

**Imágenes del Portafolio:**
- Actualmente usa imágenes de Unsplash (placeholders profesionales)
- Para usar tus propias imágenes:
  1. Guárdalas en la carpeta `img/`
  2. Edita `portfolio.html` y reemplaza las URLs de Unsplash por:
     ```html
     <img src="img/nombre-proyecto.jpg" alt="Descripción" class="portfolio-image">
     ```

### 4. Personalizar Contenido

Edita cada archivo HTML para personalizar:

- **index.html**: Hero section, beneficios, testimonios
- **about.html**: Historia, valores, estadísticas
- **services.html**: Precios, paquetes, servicios
- **portfolio.html**: Proyectos reales
- **contact.html**: Información de contacto, horarios, FAQ

## 📱 Probar en Local

Simplemente abre `index.html` en tu navegador. Para mejor experiencia, usa un servidor local:

**Opción 1 - Python:**
```bash
cd agencia-rapidweb
python -m http.server 8000
# Abre http://localhost:8000
```

**Opción 2 - Node.js:**
```bash
npx http-server
```

**Opción 3 - VS Code:**
- Instala la extensión "Live Server"
- Click derecho en `index.html` > "Open with Live Server"

## 🔧 Personalización Avanzada

### Cambiar Colores

Edita las variables CSS en `css/style.css` (líneas 14-21):

```css
:root {
    --primary-blue: #0066FF;      /* Cambia el azul principal */
    --secondary-blue: #00A3FF;    /* Cambia el azul secundario */
    --dark-gray: #333;
    --medium-gray: #666;
    /* ... */
}
```

### Cambiar Fuente

1. Ve a [Google Fonts](https://fonts.google.com)
2. Selecciona una fuente (ej: Poppins, Roboto, Montserrat)
3. Copia el link y reemplázalo en cada HTML:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=TU_FUENTE:wght@400;500;600;700&display=swap" rel="stylesheet">
   ```
4. Actualiza el CSS:
   ```css
   --font-primary: 'TU_FUENTE', sans-serif;
   ```

### Añadir Google Analytics

Antes del cierre de `</head>` en cada HTML, agrega:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-TU-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-TU-ID');
</script>
```

## 📊 SEO Mejorado

El sitio ya incluye:
- Meta tags de descripción y keywords
- Open Graph para redes sociales
- Alt tags en imágenes
- Estructura HTML semántica
- URLs limpias

**Para mejorar más:**
1. Registra el sitio en [Google Search Console](https://search.google.com/search-console)
2. Crea un archivo `sitemap.xml`
3. Añade un archivo `robots.txt`

## 🐛 Solución de Problemas

**El formulario no funciona:**
- Verifica que pusiste tu email correcto en FormSubmit
- Confirma tu email haciendo click en el link que te envían
- Revisa la carpeta de spam

**Las imágenes no cargan:**
- Verifica que las rutas sean correctas
- Asegúrate de que los archivos estén en la carpeta `img/`
- Revisa la consola del navegador (F12) por errores

**El sitio se ve mal en móvil:**
- Limpia la caché del navegador
- Verifica que el meta viewport esté presente en el HTML

## 📞 Soporte

Si tienes problemas o necesitas ayuda:
- Email: hola@agenciarapidweb.com
- WhatsApp: +54 9 XXX-XXXXXX

## 📄 Licencia

Este proyecto fue creado para Agencia RapidWeb. Puedes modificarlo y personalizarlo libremente.

---

**Desarrollado con ⚡ por Agencia RapidWeb**
*Desarrollo rápido con IA - Mendoza, Argentina*
