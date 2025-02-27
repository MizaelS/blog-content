---
title: Configurar clave SSH en Linux
date: "2025-02-26"
authorId: "mizael-segovia"
excerpt: "Aprende a configurar la autenticación con clave SSH en tu servidor para mejorar la seguridad de tus conexiones."
category: "Tutoriales"
tags: ["seguridad", "ssh", "linux", "servidor", "configuración"]
---

# Configurar clave SSH en Linux

La autenticación con clave SSH ofrece un método seguro para acceder a tu servidor sin utilizar contraseñas. Este tutorial te guía en la configuración para sistemas Unix-like y Windows.

## Crear par de claves SSH

1. **Abrir terminal:** Linux/macOS (Terminal) o Windows (PowerShell).
2. **Generar claves:** Ejecuta el comando:
    ```bash
    ssh-keygen -t rsa -b 4096 -C "tu_email@ejemplo.com"
    ```
    - Reemplaza "tu_email@ejemplo.com" por tu correo.
3. **Guardar claves:** Sigue las instrucciones para guardar las claves en una ubicación segura.
4. **Contraseña:** Establece una contraseña segura para tu clave privada.

## Copiar clave pública al servidor

### Usuarios de Unix-like

1. **Comando `ssh-copy-id`:**
    ```bash
    ssh-copy-id tu_usuario@tu_servidor
    ```
    - Cambia "tu_usuario" y "tu_servidor" por tu información.

### Usuarios de Windows

1. **Leer clave pública:**
    ```powershell
    Get-Content ~/.ssh/id_rsa.pub
    ```
2. **Copiar contenido mostrado.**
3. **Iniciar sesión en servidor:**
    ```powershell
    ssh tu_usuario@tu_servidor
    ```
4. **Añadir clave al servidor:**
    - Crear directorio `.ssh` y ajustar permisos:
    ```bash
    mkdir -p ~/.ssh
    chmod 700 ~/.ssh
    ```
    - Añadir clave al archivo `authorized_keys`:
    ```bash
    echo 'tu_clave_publica' >> ~/.ssh/authorized_keys
    chmod 600 ~/.ssh/authorized_keys
    ```
    - Reemplaza `'tu_clave_publica'` con el contenido de tu clave pública.

## Configurar servidor para aceptar autenticación SSH

1. **Iniciar sesión en servidor.**
2. **Editar configuración SSH:**
    ```bash
    sudo nano /etc/ssh/sshd_config
    ```
3. **Ajustes necesarios:**
   - Desactivar acceso por contraseña: `PasswordAuthentication no`
   - Habilitar autenticación por clave pública: `PubkeyAuthentication yes`
4. **Reiniciar servicio SSH:**
    ```bash
    sudo systemctl restart ssh
    ```

## Verificar clave en llaves conocidas

- **Verificación:** Asegúrate de que tu clave pública esté en `~/.ssh/authorized_keys` en tu servidor.

:::warning
Mantén tu clave privada segura y nunca la compartas. Si pierdes tu clave privada o olvidas la contraseña, necesitarás otro método de acceso para reconfigurar la autenticación SSH.
:::
