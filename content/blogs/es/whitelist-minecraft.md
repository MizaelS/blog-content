---
title: "Cómo usar la whitelist en Minecraft: añadir, eliminar, activar y desactivar"
date: "2025-05-30"
excerpt: "Aprende a gestionar la whitelist en Minecraft paso a paso. Guía completa para añadir, eliminar, activar y desactivar jugadores en servidores de Minecraft."
authorId: "mizael-segovia"
category: "Minecraft"
tags: ["minecraft", "whitelist", "servidor", "comandos", "seguridad", "tutorial"]
---

# Cómo usar la whitelist en Minecraft: Guía completa paso a paso

## Introducción a la whitelist de Minecraft

La whitelist (lista blanca) de Minecraft es una función de control de acceso en servidores que permite que solo jugadores autorizados se conecten. Es ampliamente utilizada por administradores para proteger sus mundos de accesos no deseados o actos de griefing.

## ¿Qué es una whitelist en Minecraft?

### Definición de whitelist

Una whitelist es una lista de nombres de usuario que tienen permiso para unirse a un servidor. Los jugadores no incluidos son rechazados al intentar conectarse.

### Propósito de la whitelist

* Restringe el acceso al servidor
* Aumenta la seguridad
* Previene el griefing
* Facilita la gestión de comunidades privadas

## Beneficios de usar una whitelist

### Mayor seguridad del servidor

La whitelist reduce las posibilidades de intrusiones y jugadores maliciosos.

### Acceso controlado

Ideal para servidores privados con solo personas de confianza.

### Mejor gestión comunitaria

Permite desarrollar comunidades más cerradas y seguras.

## Cómo activar la whitelist en Minecraft

### Instrucciones paso a paso

1. Abre la carpeta de tu servidor de Minecraft.
2. Localiza el archivo `server.properties`.
3. Cambia `white-list=false` por `white-list=true`.
4. Guarda y reinicia el servidor.

### Activar con comandos

Alternativamente, puedes usar:

```
/whitelist on
```

## Cómo desactivar la whitelist en Minecraft

### Método desde el archivo

1. Abre `server.properties`.
2. Cambia a `white-list=false`.
3. Guarda y reinicia el servidor.

### Método con comando

```
/whitelist off
```

## Cómo añadir jugadores a la whitelist

### Usando comandos

```
/whitelist add <nombredeusuario>
```

### Usando el archivo `whitelist.json`

1. Abre el archivo.
2. Añade manualmente el nombre del jugador.
3. Guarda y reinicia el servidor.

## Cómo eliminar jugadores de la whitelist

### Vía comandos

```
/whitelist remove <nombredeusuario>
```

### Editando el archivo

1. Abre `whitelist.json`.
2. Elimina el nombre del jugador.
3. Guarda y reinicia el servidor.

## Cómo ver los jugadores en la whitelist

### Con comando

```
/whitelist list
```

### Revisando el archivo

* Navega al archivo `whitelist.json`.
* Observa los nombres incluidos.

## Cómo recargar la whitelist

### Comando de recarga

```
/whitelist reload
```

Este comando es esencial tras editar manualmente el archivo.

## Errores comunes con la whitelist y soluciones

### Nombre de usuario no encontrado

* Verifica la ortografía
* Asegura que el jugador exista

### Cambios no aplicados

* Siempre reinicia o recarga tras cambios

## Buenas prácticas para gestionar la whitelist

* Haz copias de seguridad del archivo `whitelist.json`
* Usa nombres claros y organizados
* Lleva un registro externo de usuarios autorizados

## Preguntas frecuentes sobre la whitelist de Minecraft

### ¿Puedo usar whitelist en servidores Realms?

No, Realms funciona solo por invitación.

### ¿Se puede burlar la whitelist?

Solo si el servidor está comprometido o presenta fallos.

### ¿Funciona la whitelist en Java y Bedrock?

Totalmente compatible con Java. En Bedrock depende de la configuración y proveedor.

## Conclusión

Usar la whitelist en Minecraft es fundamental para la seguridad y el control de acceso en servidores privados. Con unos pocos comandos o ediciones simples al archivo correspondiente, puedes gestionar fácilmente quién entra y quién no.

## FAQs

**¿Cómo soluciono que la whitelist no funcione tras reiniciar?**
Verifica que `white-list=true` esté en el archivo y recarga con `/whitelist reload`.

**¿Puedo automatizar la whitelist?**
Sí, mediante scripts.

**¿Cuántos jugadores puedo tener en la whitelist?**
No hay límite oficial, pero listas muy grandes pueden afectar el rendimiento.

**¿La whitelist funciona con listas de baneo o permitidos?**
Sí, son sistemas compatibles.

**¿Es posible tener whitelists distintas por mundo?**
No de forma nativa, pero plugins como Multiverse pueden permitirlo.