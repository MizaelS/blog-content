
---
title: ¿Cómo crear un servidor no premium y protegerlo?
date: "2025-03-03"
authorId: "teoremal-dev"
excerpt: "Esta guía te mostrará cómo configurar un servidor no premium de Minecraft y protegerlo contra posibles amenazas."
category: "Tutoriales"
tags: [Minecraft Java, No Premium, Cracked]
---

:::info
Esta guía se ha adaptado para explicar la creación y protección de un servidor no premium, donde la verificación oficial de Mojang está deshabilitada.
:::

# Introducción

Crear un servidor no premium (también conocido como "cracked") permite que jugadores sin cuenta oficial de Mojang se unan a tu mundo. Esto amplía el alcance de tu servidor, pero implica riesgos adicionales de seguridad, ya que no se realiza la verificación de identidad. En este tutorial aprenderás a configurar tu servidor para aceptar jugadores no premium y, al mismo tiempo, implementar medidas de protección que eviten problemas como impostores y ataques.

:::warning
**Advertencia:** Al desactivar la verificación de Mojang, el servidor es más vulnerable a ataques de impostores y bots. Es fundamental implementar medidas de seguridad adicionales, como plugins de login o BungeeGuard.
:::

# Preparativos

:::info
Antes de comenzar, asegúrate de contar con el hardware y software adecuado, y de tener un plan de respaldo por si ocurre algún imprevisto.
:::

## Software Recomendado

- **Paper** – [PaperMC](https://github.com/PaperMC/Paper)  
  Recomendado por su compatibilidad con plugins de seguridad.
- **Pufferfish** – [Pufferfish](https://github.com/pufferfish-gg/Pufferfish)  
  Un fork de Paper con opciones adicionales para la personalización.
- **Purpur** – [Purpur](https://github.com/PurpurMC/Purpur)  
  Ofrece mayor personalización para ajustar detalles específicos.

:::tip
**Consejo:** Elige el software que mejor se adapte a las necesidades de seguridad de tu servidor.
:::

# Configuración del Archivo `server.properties`

Para permitir la conexión de jugadores no premium, es esencial desactivar la verificación oficial. Abre tu archivo `server.properties` y realiza los siguientes cambios:

```properties
#Minecraft server properties
#Tue Mar 04 03:36:10 UTC 2025
accepts-transfers=false
allow-flight=false
allow-nether=true
broadcast-console-to-ops=true
broadcast-rcon-to-ops=true
bug-report-link=
debug=false
difficulty=easy
enable-command-block=false
enable-jmx-monitoring=false
enable-query=false
enable-rcon=false
enable-status=true
enforce-secure-profile=false  # Desactiva la verificación de perfiles seguros para jugadores no premium
enforce-whitelist=false
entity-broadcast-range-percentage=100
force-gamemode=false
function-permission-level=2
gamemode=survival
generate-structures=true
generator-settings={}
hardcore=false
hide-online-players=false
initial-disabled-packs=
initial-enabled-packs=vanilla
level-name=world
level-seed=
level-type=minecraft:normal
log-ips=true
max-chained-neighbor-updates=1000000
max-players=20
max-tick-time=60000
max-world-size=29999984
motd=A Minecraft Server (Servidor No Premium)
network-compression-threshold=256
online-mode=false  # Importante: Desactiva la verificación oficial para permitir jugadores sin cuenta oficial
op-permission-level=4
pause-when-empty-seconds=-1
player-idle-timeout=0
prevent-proxy-connections=false
pvp=true
query.port=25565
rate-limit=0
rcon.password=
rcon.port=25575
region-file-compression=deflate
require-resource-pack=false
resource-pack=
resource-pack-id=
resource-pack-prompt=
resource-pack-sha1=
server-ip=0.0.0.0
server-name=Servidor No Premium
server-port=25570
simulation-distance=10
spawn-monsters=true
spawn-protection=16
sync-chunk-writes=true
text-filtering-config=
text-filtering-version=0
use-native-transport=true
view-distance=10
white-list=false
```

:::tip
**Tip:** Asegúrate de que las propiedades `online-mode` y `enforce-secure-profile` estén en `false` para permitir el acceso de jugadores sin cuenta oficial.
:::

# Plugins y Medidas de Seguridad

Al desactivar la verificación de Mojang, cualquier persona podría conectarse y hacerse pasar por otro jugador. Para mitigar estos riesgos, es vital implementar plugins y ajustes de seguridad:

:::info
**Autenticación:** Usa plugins como **AuthMe Reloaded** para que los jugadores se registren y se autentiquen mediante una contraseña, evitando accesos no autorizados.
:::

- **AuthMe Reloaded:**  
  Obliga a los jugadores a registrarse y autentificarse mediante una contraseña.
  
- **Whitelist y Sistema de Permisos:**  
  Configura una whitelist para controlar quién puede ingresar y asigna permisos específicos para proteger áreas críticas del servidor.

- **Plugins Anti-Bot:**  
  Considera utilizar herramientas que detecten y bloqueen ataques de bots o intentos de spam.

:::warning
**Advertencia:** Sin medidas de seguridad adicionales, los servidores no premium pueden ser explotados por jugadores malintencionados, lo que afectaría la administración y la experiencia de juego.
:::

:::tip
**Consejo:** Mantén siempre actualizado el servidor y sus plugins, y revisa periódicamente los logs para detectar actividades sospechosas.
:::

# Conclusión

Crear un servidor no premium abre la puerta a una comunidad más amplia, pero también exige reforzar la seguridad para evitar abusos.

:::info
**Resumen:** Con los cambios adecuados en el archivo `server.properties` y la implementación de plugins de seguridad, podrás ofrecer una experiencia de juego controlada y protegida, permitiendo el acceso a jugadores sin cuenta oficial.
:::

Configura correctamente tu servidor y refuerza la seguridad para mantenerlo protegido. ¡Mucho éxito y a darle con todo!

---