# 1. Comando ls

<details open>
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

<details open>
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

<details open>
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

<details open>
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


<details open>
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

<details open>
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
