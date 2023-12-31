# 1. Comando ls

<details>
<summary>Ver</summary>
<br>
El comando `ls` en Linux se utiliza para listar archivos y directorios en un directorio específico. Aquí tienes algunos ejemplos comunes de uso de `ls`:

1. **Listar archivos y directorios en el directorio actual:**
   ```bash
   ls
   ```

2. **Listar archivos y directorios con detalles:**
   ```bash
   ls -l
   ```

3. **Listar archivos y directorios, incluyendo los ocultos:**
   ```bash
   ls -a
   ```

4. **Listar archivos y directorios con detalles, incluyendo los ocultos:**
   ```bash
   ls -la
   ```

5. **Listar archivos y directorios en un directorio específico:**
   ```bash
   ls ruta/del/directorio
   ```

6. **Listar archivos y directorios con detalles en un directorio específico:**
   ```bash
   ls -l ruta/del/directorio
   ```

Estos son solo ejemplos básicos y hay muchas opciones y combinaciones que puedes usar con `ls`. Si necesitas ayuda con una tarea o un escenario específico, no dudes en proporcionar más detalles para que pueda ofrecerte una guía más precisa.

</details>

# 2 Comando cd

<details>
<summary>Ver</summary>
<br>
El comando `cd` en sistemas operativos tipo Unix (como Linux) se utiliza para cambiar el directorio actual en el que te encuentras. Aquí tienes algunos ejemplos de cómo usar `cd`:

1. **Cambiar al directorio especificado:**
   ```bash
   cd /ruta/del/directorio
   ```

   Este comando te llevará al directorio especificado.

2. **Cambiar al directorio principal del usuario:**
   ```bash
   cd
   ```

   Este comando te llevará al directorio principal del usuario actual.

3. **Cambiar al directorio anterior:**
   ```bash
   cd -
   ```

   Este comando te llevará al directorio desde el que cambiaste anteriormente.

4. **Cambiar al directorio superior (uno nivel arriba):**
   ```bash
   cd ..
   ```

   Este comando te llevará al directorio padre del directorio actual.

5. **Cambiar al directorio home del usuario:**
   ```bash
   cd ~
   ```

   Este comando te llevará al directorio home del usuario actual.

6. **Usar rutas relativas:**
   ```bash
   cd directorio/subdirectorio
   ```

   Cambia al subdirectorio dentro del directorio actual.

Es importante destacar que el comando `cd` es fundamental para la navegación en la línea de comandos. Puedes utilizar rutas absolutas o relativas según tus necesidades para cambiar entre diferentes directorios. Si necesitas más información sobre el comando `cd` o cómo usarlo en situaciones específicas, no dudes en preguntar.


</details>

# 3. Comando pwd

<details>
<summary>Ver</summary>


<br>

El comando `pwd` en sistemas operativos tipo Unix (como Linux) se utiliza para imprimir el nombre del directorio de trabajo actual (present working directory). Es útil para saber en qué directorio te encuentras en un momento dado. Aquí tienes un ejemplo básico:

```bash
pwd
```

Al ejecutar este comando, el sistema te mostrará la ruta completa del directorio actual. Por ejemplo:

```
/home/usuario
```

Esto indica que el directorio actual es "/home/usuario". La salida dependerá del directorio en el que te encuentres cuando ejecutes el comando `pwd`.

Adicionalmente, puedes utilizar opciones adicionales con `pwd`. Por ejemplo:

- `pwd -P`: Imprime la ruta física, sin enlaces simbólicos.
- `pwd -L`: Imprime la ruta lógica, teniendo en cuenta enlaces simbólicos.

El comando `pwd` es útil para verificar rápidamente tu ubicación en el sistema de archivos cuando trabajas en la línea de comandos.

</details>



# 4. Comando mkadir

<details>
<summary>Ver</summary>

<br>

El comando `mkdir` en sistemas operativos tipo Unix (como Linux) se utiliza para crear un nuevo directorio (carpeta). Aquí tienes un ejemplo básico de cómo usar `mkdir`:

```bash
mkdir nombre_del_directorio
```

Este comando creará un nuevo directorio con el nombre especificado en el directorio actual. Si deseas crear un directorio en una ubicación específica, puedes proporcionar la ruta completa:

```bash
mkdir /ruta/del/nuevo_directorio
```

Además, puedes crear múltiples directorios a la vez utilizando la opción `-p`. Por ejemplo, si deseas crear una estructura de directorios jerárquica:

```bash
mkdir -p directorio1/directorio2/directorio3
```

En este caso, se crearán los directorios `directorio1`, `directorio2` y `directorio3` incluso si no existen, junto con la estructura de directorios necesaria.

Estos son ejemplos básicos de cómo utilizar el comando `mkdir`. Puedes consultar la página de manual del comando (`man mkdir`) para obtener más detalles y opciones disponibles.

</details>

# 5. Comando rmdir


<details>
<summary>Ver</summary>

El comando `rmdir` en sistemas operativos tipo Unix (como Linux) se utiliza para eliminar directorios vacíos. Aquí tienes un ejemplo básico de cómo usar `rmdir`:

```bash
rmdir nombre_del_directorio
```

Este comando eliminará el directorio especificado solo si está vacío. Si el directorio contiene archivos o subdirectorios, `rmdir` no realizará la eliminación y mostrará un mensaje de error.

Ejemplo:

```bash
rmdir directorio_vacio
```

Si deseas eliminar un directorio y su contenido, puedes utilizar el comando `rm` con la opción `-r` (recursivo). Asegúrate de tener cuidado al usar esta opción, ya que eliminará todo el contenido del directorio.

Ejemplo:

```bash
rm -r directorio_con_contenido
```

Además, puedes usar la opción `-p` con `rmdir` para eliminar directorios padres que se vuelven vacíos después de eliminar un subdirectorio.

Ejemplo:

```bash
rmdir -p directorio_padre/subdirectorio_vacio
```

Estos son ejemplos básicos del uso del comando `rmdir`. Ten en cuenta que, para eliminar directorios que no estén vacíos, es más común utilizar `rm -r`, pero también debes ser cauteloso para evitar la pérdida accidental de datos importantes.

</details>

# 6. Comando mv

<details>
   <summary>Ver</summary>
   <br>

El comando `mv` en sistemas operativos tipo Unix (como Linux) se utiliza para mover o renombrar archivos y directorios. Aquí tienes algunos ejemplos básicos de cómo usar `mv`:

### Mover un Archivo a un Directorio

```bash
mv archivo.txt directorio_destino/
```

Este comando mueve el archivo `archivo.txt` al directorio especificado.

### Renombrar un Archivo

```bash
mv nombre_antiguo.txt nombre_nuevo.txt
```

Este comando renombra el archivo `nombre_antiguo.txt` a `nombre_nuevo.txt`.

### Mover y Renombrar Directorios

```bash
mv directorio_antiguo/ directorio_nuevo/
```

Este comando mueve y/o renombra el directorio `directorio_antiguo` a `directorio_nuevo`.

### Forzar la Sobrescritura y la Fusión (útil al mover directorios)

```bash
mv -f directorio_origen/ directorio_destino/
```

Este comando fuerza la sobrescritura de archivos si ya existen en el directorio de destino y fusiona los contenidos de los directorios si ya existe un directorio con el mismo nombre en el destino.

### Mover y Renombrar con Ruta Específica

```bash
mv archivo.txt /ruta/absoluta/para/destino/nuevo_nombre.txt
```

Este comando mueve el archivo `archivo.txt` a una ruta específica y lo renombra en el proceso.

Estos son solo ejemplos básicos del uso del comando `mv`. La versatilidad de `mv` permite una amplia gama de operaciones de movimiento y renombrado en sistemas Unix. Si necesitas más información o ejemplos específicos, no dudes en preguntar.
   
</details>

# 7. Comando cp

<details>
   <summary>Ver</summary>
   <br>
   El comando `cp` en sistemas operativos tipo Unix (como Linux) se utiliza para copiar archivos y directorios. Aquí tienes algunos ejemplos básicos de cómo usar `cp`:

### Copiar un Archivo

```bash
cp archivo_origen.txt directorio_destino/
```

Este comando copia el archivo `archivo_origen.txt` al directorio especificado.

### Copiar un Archivo y Renombrarlo

```bash
cp archivo_origen.txt archivo_destino.txt
```

Este comando copia el archivo `archivo_origen.txt` y lo renombra como `archivo_destino.txt`.

### Copiar un Directorio y su Contenido Recursivamente

```bash
cp -r directorio_origen/ directorio_destino/
```

Este comando copia el directorio `directorio_origen` y su contenido al directorio `directorio_destino`. La opción `-r` es para realizar una copia recursiva y copiar también los subdirectorios y sus contenidos.

### Copiar con Confirmación (evitar sobrescrituras no deseadas)

```bash
cp -i archivo_origen.txt directorio_destino/
```

Este comando solicitará confirmación antes de sobrescribir un archivo existente en el destino. Preguntará si deseas sobrescribir cada archivo.

### Copiar y Conservar Metadatos y Permisos

```bash
cp -p archivo_origen.txt directorio_destino/
```

Este comando copia el archivo `archivo_origen.txt` al directorio `directorio_destino` y conserva los metadatos (timestamp) y los permisos del archivo original.

### Copiar Solo si el Archivo es Más Nuevo

```bash
cp -u archivo_origen.txt directorio_destino/
```

Este comando copia el archivo `archivo_origen.txt` al directorio `directorio_destino` solo si el archivo origen es más nuevo que el archivo destino o si el archivo destino no existe.

Estos son solo ejemplos básicos del uso del comando `cp`. La variedad de opciones proporciona flexibilidad para adaptarse a diferentes situaciones de copiado en sistemas Unix. Si necesitas más información o ejemplos específicos, no dudes en preguntar.
</details>

# 8. Comando open

<details>
   <summary>Ver</summary>
   <br>

El comando `open` en sistemas operativos basados en Unix, como macOS, se utiliza para abrir archivos o directorios con la aplicación predeterminada asociada a ese tipo de archivo. También se puede utilizar para abrir archivos o aplicaciones específicas desde la línea de comandos.

### Ejemplos básicos:

1. **Abrir un archivo con la aplicación predeterminada:**
   ```bash
   open archivo.txt
   ```
   Esto abrirá el archivo `archivo.txt` con la aplicación predeterminada asociada al tipo de archivo.

2. **Abrir un directorio con el Finder (en macOS):**
   ```bash
   open directorio/
   ```
   Esto abrirá el directorio `directorio` utilizando el Finder en macOS.

3. **Abrir una aplicación específica:**
   ```bash
   open -a "Nombre de la Aplicación"
   ```
   Sustituye "Nombre de la Aplicación" con el nombre de la aplicación que deseas abrir. Por ejemplo:
   ```bash
   open -a "Google Chrome"
   ```

4. **Abrir varios archivos o directorios:**
   ```bash
   open archivo1.txt archivo2.txt
   open directorio1/ directorio2/
   ```

### Opciones adicionales:

- `-e`: Abre el archivo o directorio con el editor de texto predeterminado.
- `-t`: Abre el archivo o directorio con la aplicación de texto predeterminada.
- `-b`: Abre la aplicación asociada al identificador de paquete.

Es importante mencionar que el comando `open` es específico de sistemas como macOS y puede no estar disponible en sistemas operativos basados en Linux o Unix diferentes. En esos sistemas, se utilizan comandos diferentes para abrir archivos y aplicaciones.

   
</details>

# 9. Comando touch
<details>
   <summary>Ver</summary>
   <br>

   El comando `touch` en sistemas operativos tipo Unix, como Linux, se utiliza para actualizar las marcas de tiempo de acceso y modificación de un archivo o directorio. Si el archivo no existe, `touch` se encargará de crear un archivo vacío con el nombre especificado. Aquí tienes algunos ejemplos básicos de cómo usar `touch`:

### Ejemplos básicos:

1. **Crear un archivo vacío:**
   ```bash
   touch archivo.txt
   ```
   Esto creará un archivo llamado `archivo.txt` si no existe. Si ya existe, actualizará las marcas de tiempo.

2. **Actualizar las marcas de tiempo de un archivo existente:**
   ```bash
   touch archivo_existente.txt
   ```
   Esto actualizará las marcas de tiempo de acceso y modificación del archivo `archivo_existente.txt`.

3. **Crear varios archivos a la vez:**
   ```bash
   touch archivo1.txt archivo2.txt archivo3.txt
   ```
   Esto creará tres archivos vacíos con los nombres especificados.

### Opciones adicionales:

- `-c`: No crea el archivo si no existe. Simplemente actualiza las marcas de tiempo de los archivos existentes.
- `-t`: Permite especificar una marca de tiempo específica en lugar de usar la hora actual.

### Ejemplos con opciones:

1. **Actualizar las marcas de tiempo sin crear el archivo si no existe:**
   ```bash
   touch -c archivo_no_existente.txt
   ```

2. **Crear un archivo con una marca de tiempo específica:**
   ```bash
   touch -t YYYYMMDDHHMM.SS archivo_con_fecha.txt
   ```
   Reemplaza `YYYYMMDDHHMM.SS` con la marca de tiempo deseada en el formato AAMMDDhhmm.SS.

El comando `touch` es útil para actualizar marcas de tiempo y crear archivos vacíos cuando sea necesario. Si necesitas más información o tienes preguntas adicionales, no dudes en preguntar.

   
</details>


# 10. comando chown

<details>
   <summary>Ver</summary>
   <br>
   El comando `chown` es utilizado en sistemas operativos tipo Unix y Linux para cambiar el propietario de archivos y directorios. La sintaxis básica del comando es la siguiente:

```bash
chown [opciones] nuevo_propietario[:nuevo_grupo] archivo(s)
```

- `nuevo_propietario`: Especifica el nuevo propietario al que se asignará el archivo o directorio.
- `nuevo_grupo`: (Opcional) Especifica el nuevo grupo al que se asignará el archivo o directorio.
- `archivo(s)`: Especifica el archivo o archivos para los cuales se cambiará el propietario.

Ejemplos de uso:

1. Cambiar el propietario de un archivo:
   ```bash
   chown nuevo_propietario archivo
   ```

2. Cambiar el propietario y el grupo de un archivo:
   ```bash
   chown nuevo_propietario:nuevo_grupo archivo
   ```

3. Cambiar el propietario de un directorio y de manera recursiva para todos sus archivos y subdirectorios:
   ```bash
   chown -R nuevo_propietario directorio
   ```

Algunas opciones comunes de `chown`:

- `-R`: Realiza la operación de manera recursiva, cambiando el propietario de los archivos y directorios dentro del directorio especificado y sus subdirectorios.
- `-v`: Muestra un mensaje para cada archivo o directorio procesado, indicando si el cambio de propietario fue exitoso.
- `-c`: Muestra mensajes solo cuando se realiza un cambio efectivo.
- `--from=propietario_anterior`: Especifica el propietario actual del archivo o directorio.

Es importante tener en cuenta que el comando `chown` generalmente requiere privilegios de superusuario (root) para cambiar el propietario de archivos fuera del contexto del usuario actual. Si no tienes los privilegios adecuados, es posible que necesites usar `sudo` antes del comando para ejecutarlo con permisos elevados.
</details>

# 11. Comando top
<details>
   <summary>Ver</summary>

   <br>

   El comando `top` es una herramienta de línea de comandos que se utiliza en sistemas operativos Unix y Linux para monitorear las estadísticas del sistema en tiempo real. Proporciona una vista en tiempo real de la actividad del sistema, mostrando información sobre el uso de la CPU, la memoria, los procesos en ejecución y otros recursos del sistema. Aquí hay una descripción básica de cómo usar el comando `top`:

1. **Ejecución del comando:**
   Simplemente escribe `top` en la terminal y presiona Enter. Esto abrirá una ventana en la terminal que mostrará información actualizada sobre el estado del sistema.

   ```bash
   top
   ```

2. **Interfaz de usuario:**
   La interfaz de `top` consta de varias secciones. Algunas de las secciones más importantes incluyen:

   - **Resumen del sistema:** Muestra información sobre la carga promedio del sistema, el tiempo de actividad, el número de usuarios, y más.
   - **Estadísticas de la CPU:** Muestra el uso de la CPU por proceso y en general.
   - **Memoria:** Muestra el uso de la memoria, incluyendo RAM y swap.
   - **Información de procesos:** Lista los procesos en ejecución, ordenados por diferentes criterios como uso de CPU, memoria, etc.

3. **Comandos durante la ejecución:**
   - `q`: Salir de `top`.
   - `k`: Matar un proceso. Selecciona un proceso y presiona `k`, luego ingresa el número del proceso que deseas matar.
   - `Space`: Actualizar la pantalla.

4. **Opciones de línea de comandos:**
   - `top -u usuario`: Muestra solo los procesos del usuario especificado.
   - `top -p PID`: Muestra información sobre un proceso específico, donde `PID` es el ID del proceso.
   - `top -n num`: Especifica el número de actualizaciones que se mostrarán antes de salir.

El comando `top` es una herramienta poderosa para monitorear el rendimiento del sistema en tiempo real y es comúnmente utilizado por administradores de sistemas y usuarios avanzados para diagnosticar problemas de rendimiento.

</details>

# 12. Comando Kill

<details>
   <summary>
      Ver
   </summary>
   <br>
   El comando `kill` se utiliza en sistemas operativos tipo Unix y Linux para enviar señales a procesos. La señal más comúnmente enviada con `kill` es la señal SIGTERM (15), que solicita a un proceso que se cierre de manera ordenada. Aquí está la sintaxis básica del comando `kill`:

```bash
kill [opciones] ID_de_proceso
```

- `opciones`: Pueden ser diferentes señales o parámetros adicionales.
- `ID_de_proceso`: Es el identificador del proceso al que se enviará la señal. Puedes obtener el ID de proceso utilizando comandos como `ps` o `top`.

Ejemplos de uso:

1. **Enviar la señal SIGTERM (15) a un proceso:**
   ```bash
   kill PID_del_proceso
   ```

2. **Enviar la señal SIGKILL (9) para forzar la terminación de un proceso:**
   ```bash
   kill -9 PID_del_proceso
   ```

3. **Enviar una señal específica a un proceso:**
   ```bash
   kill -SIGNUM PID_del_proceso
   ```
   Reemplaza `SIGNUM` con el número de la señal específica que deseas enviar. Por ejemplo, `kill -HUP` envía la señal SIGHUP.

4. **Enviar señal a todos los procesos de un usuario:**
   ```bash
   pkill -u nombre_de_usuario
   ```
   Esto enviará la señal predeterminada (SIGTERM) a todos los procesos del usuario especificado.

Algunas señales comunes que se pueden enviar con `kill`:

- **SIGTERM (15):** Terminación suave. Permite al proceso realizar acciones de limpieza antes de cerrarse.
- **SIGKILL (9):** Terminación forzada. Mata al proceso inmediatamente sin permitir que realice ninguna acción de limpieza.
- **SIGHUP (1):** Hup (hang up). A menudo utilizado para reiniciar un proceso.

Es importante tener en cuenta que algunos programas responden de manera diferente a diferentes señales, y el comportamiento exacto puede depender del programa y de cómo está diseñado para manejar señales. Además, ten cuidado al usar la señal SIGKILL, ya que puede dejar recursos no liberados si el proceso no tiene la oportunidad de realizar acciones de limpieza.
</details>

## 12. Comando nano

<details>
    <summary>Ver</summary>
    <br>
   El comando `nano` es un editor de texto en línea de comandos que se utiliza en sistemas operativos tipo Unix y Linux. Es una opción fácil de usar, especialmente para principiantes, ya que presenta una interfaz de usuario simple y comandos básicos en la parte inferior de la pantalla. Aquí tienes una descripción básica del uso del comando `nano`:

```bash
nano [opciones] nombre_del_archivo
```

- `opciones`: Pueden ser diferentes opciones de configuración o acciones específicas del editor.
- `nombre_del_archivo`: Especifica el nombre del archivo que deseas editar o crear.

Algunas operaciones básicas dentro de `nano` incluyen:

1. **Abrir un archivo para editar:**
   ```bash
   nano nombre_del_archivo
   ```

2. **Guardar cambios:**
   - `Ctrl + O`: Guarda el archivo. Puedes confirmar el nombre del archivo y presionar Enter.
  
3. **Salir de `nano`:**
   - `Ctrl + X`: Sale del editor. Si has realizado cambios, se te preguntará si deseas guardarlos antes de salir.

4. **Desplazarse por el texto:**
   - Usa las teclas de flecha para moverte arriba, abajo, izquierda y derecha.

5. **Copiar y pegar texto:**
   - `Ctrl + K`: Corta el texto.
   - `Ctrl + U`: Pega el texto.

6. **Buscar y reemplazar:**
   - `Ctrl + W`: Busca texto en el archivo.
   - `Ctrl + \`: Inicia el proceso de reemplazo de texto.

7. **Mostrar/ocultar números de línea:**
   - `Alt + N`: Activa/desactiva la visualización de números de línea.

Estos son solo algunos ejemplos de los comandos y funciones básicas de `nano`. La pantalla de ayuda de `nano` en la parte inferior proporciona información adicional sobre los comandos disponibles. `nano` es una excelente opción para editar archivos de configuración o realizar ediciones rápidas en la línea de comandos.
</details>

# 14. Comando sudo

<details>
    <summary>Ver</summary>
       <br>
   El comando `su` (abreviatura de "switch user" o "substitute user") se utiliza en sistemas operativos tipo Unix y Linux para cambiar de usuario en la terminal. También puede utilizarse para abrir una nueva sesión de shell como otro usuario, ya sea un usuario común o el usuario root (superusuario). Aquí tienes la sintaxis básica del comando `su`:

```bash
su [opciones] [nombre_de_usuario]
```

- `opciones`: Pueden ser diferentes opciones de configuración.
- `nombre_de_usuario`: Especifica el nombre de usuario al que deseas cambiar. Si no se proporciona, por defecto intentará cambiar al usuario root.

Ejemplos de uso:

1. **Cambiar al usuario root:**
   ```bash
   su
   ```
   Te pedirá la contraseña del usuario root.

2. **Cambiar a otro usuario:**
   ```bash
   su nombre_de_usuario
   ```
   Reemplaza `nombre_de_usuario` con el nombre del usuario al que deseas cambiar. Se te pedirá la contraseña del usuario especificado.

3. **Ejecutar un comando como otro usuario:**
   ```bash
   su -c "comando" -s /bin/sh nombre_de_usuario
   ```
   Esto ejecutará el comando especificado como el usuario especificado. Reemplaza `"comando"` con el comando que deseas ejecutar y `nombre_de_usuario` con el nombre del usuario.

4. **Abrir una shell como otro usuario:**
   ```bash
   su -s /bin/bash nombre_de_usuario
   ```
   Esto abrirá una nueva sesión de shell como el usuario especificado. Reemplaza `nombre_de_usuario` con el nombre del usuario.

Es importante destacar que para utilizar `su` para cambiar al usuario root o a otro usuario, generalmente necesitarás conocer la contraseña de ese usuario. Además, algunas distribuciones de Linux pueden tener configuraciones específicas para restringir el uso de `su` por razones de seguridad. En lugar de `su`, también puedes utilizar `sudo` para ejecutar comandos con privilegios de superusuario en sistemas que lo admitan.
</details>



