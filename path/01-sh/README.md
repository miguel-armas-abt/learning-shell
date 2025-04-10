# SH

[← Regresar a notas](../../README.md) <br>

---
[1. Shortcuts](#1-shortcuts) <br>
[2. Gestión de comandos](#2-gestión-de-comandos) <br>
[3. Gestión de ficheros y directorios](#3-gestión-de-ficheros-y-directorios) <br>
[4. Grep](#4-grep) <br>

---

## 1. Shortcuts

> ### 💡 Limpiar consola
> ```
> ctrl + L
> ```

> ### 💡 Autocompletar comando
> ```
> Tab
> ```

---

## 2. Gestión de comandos

> ### ▶️ Mostrar el historial de comandos escritos
> ```shell script
> history
> ```

> ### ▶️ Ejecutar el enésimo comando
> ```shell script
> !11
> ```

> ### ▶️ Gestión de alias
> Los alias existen solo durante la sesión de la shell.
> ```shell script
> alias <alias-name>=<command> # Crear alias
> alias # Mostrar alias
> unalias <alias-name> # Eliminar alias
> ```
>
> Ejemplo: `alias docker-ps-format=docker ps -a --format "table {{.ID}}\t{{.Names}}\t{{.Status}}"`
---

## 3. Gestión de ficheros y directorios

> ### ▶️ Acceder al directorio de usuario
> 📌 La raíz del disco se especifica con `/` y el directorio de usuario con `~`
> ```shell script
> pwd
> cd ~
> ```

> ### ▶️ Acceder a un directorio
> ```shell script
> cd <directory-name>/
> cd . # directorio actual
> cd .. # directorio anterior
> ```

> ### ▶️ Crear directorio
> ```shell script
> mkdir <directory-name>
> ```

> ### ▶️ Mostrar el contenido del directorio actual
> ```shell script
> ls
> ls -al # incluye archivos ocultos
> ```

> ### ▶️ Crear archivo
> ```shell script
> touch <filename.extension>
> ```

> ### ▶️ Eliminar archivo
> ```shell script
> rm <filename.extension>
> ```

> ### ▶️ Mostrar el contenido de un archivo
> ```shell script
> cat <filename.extension>
> ```

--- 

## 4. GREP
El comando `grep` (Global Regular Expression Print) es útil para extraer solo las líneas que coinciden con un patrón especificado.

> ### ▶️ Filtrar las líneas coincidentes
> - Utilice `-i` para ignorar mayúsculas y minúsculas
> - Utilice `-v` para mostrar las líneas que no coincidan con el patrón
> ```shell script
> grep "<match-word>" <filename>.<extension> # Filtrar líneas de un archivo
> kubectl get pods -A | grep "<match-word>" # Filtrar salida de comandos
> ```







