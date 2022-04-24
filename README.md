**Manual de Git**

**Ver la versión de Git**

- **git –versión** (ver la versión de git)

**Configuración Inicial**

- **git config –global user.name &quot;Mi Nombre&quot;** (configuración global del usuario de git para todos los proyectos)

- **git config –global user.email** [**micorreo@gmail.com**] (configuración global del correo de git para todos los proyectos)

- **git config –global core.editor &quot;code --wait&quot;** (configuración global del editor por defecto a usar, comando wait espera a que se cierre el editor)

- **git config –global -e** (verificar la configuración global de git en el editor de texto)

- **git config –global core.autocrlf true** (Windows)

- **git config –global core.autocrlf input** (Mac/Linux)

- **git config -h** (todos los comandos de configuración disponible para git)

**Iniciar repositorio**

- **git init** (Iniciar un repositorio nuevo)

**Abrir editor**

- **code .** (Abrir VS Code desde git bash)

**Agregar archivos**

- **git add archivo.txt** (agrega un archivo en específico)
- **git add \*.txt** (agrega los archivos que tenga una extensión especifica usando expresiones regulares)
- **git add .** (agrega todos los archivos listados) solo usar cuando se este seguro de que todos los archivos a comprometer sean necesarios.
- **git add arhcivo1.txt archivo2.txt** (agregar multiples archivos, separando los nombres por espacios)

**Comprometer archivos**

- **git commit -m &quot;primer commit&quot;** (comprometer archivos agregándoles un mensaje dentro de las comillas)
- **git commit** (abre el editor configurado para que se agregue el texto correspondiente al commit)

**Eliminar y recuperar archivos**

- **rm archivo2.txt** (eliminar archivo desde la terminal)
- **git add archivo2.txt** (agregar el archivo a la etapa stage para hacer el commit)

- **git rm archivo.txt** (elimina el archivo y queda listo para hacer el commit)

- **git restore --staged archivo.txt** (sacar un archivo de la etapa de stage)
- **git restore archivo.txt** (recuperar un archivo borrado)

**Renombrar archivos**

- **mv archivoPrimero.txt archivo.txt** (renombrar archivos desde la terminal)
- **git add archivoPrimero.txt archivo.txt** (renombrar y asignar el nuevo nombre del archivo para hacer el commit)
- **git mv archivo.txt archivoPrimero.txt** (renombrar el archive y dejar listo para el commit)

**Ignorar archivos específicos**

- Crear archivo **.gitignore** y dentro colocar el/los archivos a ignorar, de igual manera con la/las carpetas.

**Ver el estado de los archivos**

- **git status** (ver todos los detalles de los estados de los archivos)
- **git status -s** (ver el estado de los archivos de manera comprimida)

- **git diff** (ver los cambios realizados que se han realizado, pero no se han agregado ni comprometido)
- **git diff --staged** (ver los cambios realizados que se han realizado y que se han agregado, pero no comprometido)

**Ver el historial de commits**

- **git log** (ver el historial completo de los commit realizados y quien los ha realizado)
- **git log --oneline** (ver el historial de manera más comprimida)
- **git log --stat** (muestra las líneas que se han agregado o borrado)
- **git log -p** (muestra los cambios que se han realizado)
- **git log -p 1234567** (Ver los cambios específicos de un commit en espacial, usando el numero SHA)

**Tags en Github**

- **git tag -a xyz** (agrega el nombre xyz al tag y abre el editor de texto)
- **git tag xyz** (agrega el nombre xyz al tag)
- **git tag** (sirve para ver el ultimo tag)
- **git tag -d xyz** (borra el tag y el nombre)
- **git tag -a xyz 1234567** (agrega un tag con su nombre al número SHA del commit elegido)

**Ramas en GitHub**

- **git branch** (verifica la rama actual)
- **git checkout -b nombredelarama** (crear una nueva rama y se le asigna un nombre)
- **cat archivo.txt** (ver el contenido de un archivo)
- **git branch -d nombredelarama** (elimina la rama creada)
- **git merge nombredelarama** (estar en la rama que se quiere traer el contenido de la otra rama, para así poder ejecutar el código)

**Vincular Git con GitHub**

- **Crear repositorio en github, no seleccionar ninguna palomita y crearlo.**
- **git remote add origin url\_del\_repositorio**
- **git push -u origin main** (subir el contenido y crear la rama main en github)

**-usuario registrado**

**-contrasena (KEY):** settings, developer setttings, personal acces tokens, generate new token, nombredeltoken, expiration, alcance(todas del repo), generate token.

- **Git push -u origin nuevaRama** (estando en una rama que se quiera subir a github, pero no merge con la principal. Esto creara la nueva rama en github)