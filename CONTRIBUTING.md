# Contribuyendo al Repositorio de Contenido del Blog

¡Gracias por tu interés en contribuir a nuestro repositorio de contenido! Aquí hay algunas pautas para ayudarte a comenzar.

## Cómo Contribuir

1. **Añadir Nuevas Entradas de Blog**
   - Crea un nuevo archivo Markdown en la carpeta `content/posts/en` para entradas en inglés o en `content/posts/es` para entradas en español.
   - Asegúrate de incluir los siguientes metadatos al principio del archivo:
     ```markdown
     ---
     title: "Título de tu entrada"
     date: "YYYY-MM-DD"
     excerpt: "Resumen de tu entrada"
     authorId: "id-del-autor"
     ---
     ```
   - Escribe el contenido de tu entrada en formato Markdown.

2. **Actualizar Información de Autores**
   - Si deseas añadir un nuevo autor, crea un archivo JSON en la carpeta `content/authors` con la siguiente estructura:
     ```json
     {
       "id": "nuevo-autor",
       "name": "Nombre del Autor",
       "links": {
         "github": "enlace-a-github",
         "twitter": "enlace-a-twitter",
         "website": "enlace-a-sitio-web"
       }
     }
     ```

3. **Imágenes Compartidas**
   - Si necesitas añadir imágenes, colócalas en la carpeta `content/shared/images`.

## Normas a Seguir

- Asegúrate de que tu contenido sea original y no infrinja derechos de autor.
- Mantén un tono amigable y profesional en tus entradas.
- Revisa la ortografía y gramática antes de enviar tu contribución.

## Envío de Contribuciones

- Realiza un fork del repositorio.
- Crea una nueva rama para tu contribución.
- Envía un pull request describiendo los cambios que has realizado.

¡Esperamos tus contribuciones!