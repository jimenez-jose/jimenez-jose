# Laboratorio 3

## Objetivos
Implementar elementos HTML avanzados y multimedia creando un **Portal de Eventos UTP** completo.

## Resolver
Crear desde cero un sitio web para promocionar eventos estudiantiles/académicos de la UTP que incluya:

### 🎬 Sección Multimedia de Eventos
- `<video>`: Video promocional del último evento (ej: graduación, feria tecnológica)
  - Incluir controles (`controls`)
  - Usar al menos 2 formatos: `<source src="evento.mp4" type="video/mp4">` y `<source src="evento.webm" type="video/webm">`
  - Agregar texto alternativo para accesibilidad
- `<audio>`: Audio la canción de patria de Rubén Blades
  - Usar controles y autoplay opcional
  - Incluir múltiples formatos (mp3, ogg)
- `<iframe>`: Embebido de ubicación del campus en Google Maps
  - Configurar dimensiones apropiadas
  - Agregar título descriptivo

### 🏗️ Estructura Semántica de la Página
- `<header>`: Logo UTP + navegación principal
- `<main>`: Contenido principal del portal
- `<article>`: Cada evento como un artículo individual con:
  - Título del evento
  - Fecha, hora, lugar
  - Descripción del evento
- `<section>`: Agrupar eventos por categorías (académicos, deportivos, culturales)
- `<aside>`: Sidebar con eventos destacados o noticias relacionadas
- `<figure>` y `<figcaption>`: Fotos de eventos pasados con descripciones
- `<footer>`: Información de contacto UTP y redes sociales

### 📅 Formulario de Registro a Eventos
- `<fieldset>` y `<legend>`: Agrupar campos en "Información Personal" y "Selección de Evento"
- Inputs HTML5 específicos:
  - `<input type="date" required>`: Fecha de nacimiento
  - `<input type="time">`: Hora preferida para el evento
  - `<input type="email">`: Correo institucional
  - `<input type="tel">`: Número de teléfono
  - `<input type="color">`: Color favorito (para personalización)
  - `<input type="range">`: Nivel de interés (1-10)
  - `<input type="number">`: Cantidad de acompañantes
- `<datalist>`: Lista de facultades UTP para autocompletado

```html
<input list="facultades" name="facultad">
<datalist id="facultades">
  <option value="Ingeniería de Sistemas">
  <option value="Ingeniería Civil">
  <option value="Ingeniería Industrial">
</datalist>
```

- Validación HTML5:
  - `required` en campos obligatorios
  - `pattern` para formato de cédula panameña `^\d{2}-\d{3-4}-\d{4}$`
  - `min` y `max` para fechas y números

### ⚡ Elementos Interactivos
- `<details>` y `<summary>`: FAQ expandible sobre los eventos

```html
<details>
  <summary>¿Cómo me registro para un evento?</summary>
  <p>Completa el formulario de registro...</p>
</details>
```

- `<progress>`: Barra de cupos disponibles para cada evento

```html
<progress value="75" max="100">75% de cupos ocupados</progress>
```

- `<meter>`: Indicador de popularidad del evento

```html
<meter value="8.5" min="0" max="10">8.5 de 10 estrellas</meter>
```

### 🔍 SEO y Metadatos
- Meta tags:

```html
<meta name="description" content="Portal oficial de eventos UTP - Universidad Tecnológica de Panamá">
<meta name="keywords" content="UTP, eventos, universidad, Panamá, estudiantes">
<meta name="author" content="[Tu nombre]">
```

- Open Graph para redes sociales:

```html
<meta property="og:title" content="Eventos UTP">
<meta property="og:description" content="Descubre los próximos eventos en la UTP">
<meta property="og:image" content="logo-utp.png">
```

- Favicon: Ícono de UTP en la pestaña del navegador

### 📂 Estructura de Archivos Requerida
```
lab3/
├── index.html
├── favicon.ico
├── assets/
│   ├── evento-video.mp4
│   ├── patria.mp3
│   └── evento-foto.jpg
└── README.md
```

### ✅ Requerimientos técnicos
- Página completamente funcional e independiente (no usar lab2)
- Todos los elementos multimedia deben funcionar
- Formulario debe validarse correctamente
- Código semánticamente correcto
- Al menos 5 eventos diferentes mostrados
- Implementar principios de accesibilidad básicos

### 📌 Notas
- No se permite la importación de ninguna librería JavaScript como dependencia
- El trabajo se debe realizar de forma individual
- Para la entrega, se debe enviar un screenshot de la aplicación funcionando, mostrando especialmente los elementos multimedia e interactivos, además del código HTML utilizado. Además de las capturas, se debe enviar un enlace de git que apunte a su repositorio
- Recordar que, el nombre del repositorio debe seguir el siguiente patrón: "apellido-nombre", por ejemplo: `agrazal-erick`. Dentro de ese repositorio, crear una carpeta con el nombre del laboratorio correspondiente
- Los archivos multimedia (videos, audios) pueden ser de muestra/placeholder si no tienen contenido propio

### 🔗 Para mayor información, favor referirse a
- [Guía HTML](https://github.com/ErickAgrazal/agrazal-erick-2025-1GS221/blob/master/docs/01-html/README.md)
- [Guía Git](https://github.com/ErickAgrazal/agrazal-erick-2025-1GS221/blob/master/docs/04-git/README.md)

