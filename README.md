# README.md

# Blog Content Repository

Este repositorio está diseñado para facilitar la creación y gestión de contenido de blog en múltiples idiomas. Permite a los autores contribuir con entradas de blog sin necesidad de acceso completo al sitio web.

## Estructura del Proyecto

- **content/**: Contiene todas las entradas de blog y la información de los autores.
  - **authors/**: Archivos JSON que contienen información sobre los autores.
  - **posts/**: Entradas de blog organizadas por idioma.
    - **es/**: Entradas de blog en español.
    - **en/**: Entradas de blog en inglés.
  - **shared/**: Recursos compartidos, como imágenes.

- **.github/**: Contiene flujos de trabajo de GitHub Actions para validar el contenido del repositorio.
  
- **package.json**: Configuración del proyecto y dependencias necesarias.

- **CONTRIBUTING.md**: Directrices para contribuir al repositorio.

## Cómo Contribuir

Si deseas añadir una nueva entrada de blog, por favor revisa el archivo `CONTRIBUTING.md` para obtener instrucciones sobre cómo hacerlo.

## Configuración

Para configurar el proyecto localmente, clona el repositorio y ejecuta:

```bash
npm install
```

Esto instalará todas las dependencias necesarias para el proyecto.

## Licencia

Este proyecto está bajo la Licencia MIT.