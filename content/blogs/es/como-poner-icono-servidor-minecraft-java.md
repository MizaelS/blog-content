---
title: Cómo poner el icono del servidor en Minecraft Java
date: "2025-05-29"
authorId: "mizael-segovia"
excerpt: "Aprende cómo personalizar tu servidor de Minecraft Java añadiendo un ícono único que lo represente en la lista de servidores."
category: "Tutoriales"
tags: ["minecraft", "servidor", "icono", "personalización", "hosting"]
---

# ¿Cómo poner el icono del servidor en Minecraft Java?

Tener un servidor en Minecraft es genial, pero darle tu propio estilo lo hace único. Una de las formas más sencillas de personalizarlo es agregando un icono personalizado. En este blog te enseño paso a paso cómo poner el icono de tu servidor en Minecraft Java Edition.

---

## Requisitos

Antes de comenzar, necesitas lo siguiente:

- Un servidor de Minecraft Java Edition (versión 1.7.2 en adelante).
- Acceso a los archivos del servidor.
- Un icono en formato **PNG**, de exactamente **64x64 píxeles**.

---

## Paso a paso

### 1. Crea o convierte tu icono

Puedes usar herramientas como Canva, Photoshop, GIMP o incluso editores online para crear tu propio logo cuadrado. Asegúrate de que:

- El tamaño sea **64x64 px**.
- Esté en formato **PNG**.
- El nombre del archivo sea exactamente: `server-icon.png`

> Ejemplo: `server-icon.png`

¿Tu imagen está en JPG, JPEG, WebP o en otro formato? ¡No te preocupes! Puedes usar nuestra [herramienta oficial de Teramont Host](https://teramont.net/tools/minecraft-icon-converter) que convierte automáticamente tu logo al formato correcto (`server-icon.png` en PNG y 64x64 píxeles), listo para usar en tu servidor.

### 2. Coloca el archivo en la carpeta principal del servidor

Ubica el directorio donde están los archivos del servidor. Ahí debes copiar o mover tu `server-icon.png`.

La estructura quedaría algo así:

```
/server-icon.png
/server.jar
/server.properties
/world/
```

### 3. Reinicia el servidor

Una vez colocado el archivo, **reinicia el servidor** para que el icono se cargue correctamente. Minecraft lo detecta de forma automática si está bien nombrado y en la ruta correcta.

---

## Resultado final

Cuando tus jugadores vean el servidor en la lista multijugador, aparecerá el icono personalizado junto al nombre y MOTD de tu server.

---

## Consejos extra

* Si el icono no aparece, verifica que no tenga mayúsculas en el nombre (debe ser `server-icon.png`).
* Asegúrate de que no esté en una subcarpeta.
* Comprueba que esté en formato PNG y no JPG, JPEG o WebP.

---

¡Y listo! Así de fácil es darle un toque más profesional y personalizado a tu servidor. ¡Haz que destaque desde la lista de servidores!
