# Laboratorio #4 - CSS Introducción

## Instrucciones

### Objetivos:

- Comprender cómo se integra CSS en un documento HTML.  
- Aplicar selectores básicos (elementos, clases e IDs).  
- Practicar con propiedades comunes: color, tipografía, márgenes, paddings, bordes y fondos.  
- Familiarizarse con el modelo de caja (box model).  

### Resolver

Crea una carpeta llamada **lab4** que contenga:

- index.html  
- styles.css  

En **index.html**, coloca esta estructura inicial:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mi Primera Página con CSS</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Bienvenidos a mi página</h1>
    <p class="subtitulo">Aprendiendo CSS paso a paso</p>
  </header>

  <main>
    <section id="intro">
      <h2>Introducción</h2>
      <p>Este es un párrafo de ejemplo para practicar estilos con CSS.</p>
    </section>

    <section class="tarjeta">
      <h2>Tarjeta de prueba</h2>
      <p>Aquí probaremos bordes, márgenes y padding.</p>
    </section>

    <button>Haz clic aquí</button>
  </main>

  <footer>
    <p>&copy; 2025 Mi Nombre</p>
  </footer>
</body>
</html>
