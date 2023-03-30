# git-commands

Configuración inicial
Antes de utilizar Git, es recomendable configurar algunos datos iniciales, como tu nombre y correo electrónico. Puedes hacerlo utilizando los siguientes comandos:

arduino
Copy code
git config --global user.name "Tu nombre"
git config --global user.email "Tu correo electrónico"
Crear un nuevo repositorio
Para crear un nuevo repositorio de Git, puedes utilizar el siguiente comando:

csharp
Copy code
git init
Este comando creará un nuevo repositorio de Git en el directorio actual.

Agregar archivos al repositorio
Una vez que hayas creado un repositorio, puedes agregar archivos al mismo utilizando el siguiente comando:

csharp
Copy code
git add nombre_del_archivo
Este comando agregará el archivo especificado al área de preparación (staging area) de Git, lo que significa que el archivo está listo para ser confirmado (commited).

Confirmar cambios
Una vez que hayas agregado los archivos que deseas confirmar, puedes confirmar los cambios utilizando el siguiente comando:

sql
Copy code
git commit -m "Mensaje de confirmación"
Este comando confirmará los cambios en el repositorio, utilizando el mensaje especificado para describir los cambios realizados.

Verificar el estado del repositorio
Puedes verificar el estado actual del repositorio utilizando el siguiente comando:

lua
Copy code
git status
Este comando te mostrará los archivos que han sido modificados, agregados o eliminados, y que aún no han sido confirmados.

Verificar el historial de confirmaciones
Puedes verificar el historial de confirmaciones (commits) en el repositorio utilizando el siguiente comando:

bash
Copy code
git log
Este comando te mostrará una lista de todas las confirmaciones realizadas en el repositorio, incluyendo los mensajes de confirmación y los autores.

Crear una nueva rama
Puedes crear una nueva rama en el repositorio utilizando el siguiente comando:

Configuración inicial
Antes de utilizar Git, es recomendable configurar algunos datos iniciales, como tu nombre y correo electrónico. Puedes hacerlo utilizando los siguientes comandos:

arduino
Copy code
git config --global user.name "Tu nombre"
git config --global user.email "Tu correo electrónico"
Crear un nuevo repositorio
Para crear un nuevo repositorio de Git, puedes utilizar el siguiente comando:

csharp
Copy code
git init
Este comando creará un nuevo repositorio de Git en el directorio actual.

Agregar archivos al repositorio
Una vez que hayas creado un repositorio, puedes agregar archivos al mismo utilizando el siguiente comando:

csharp
Copy code
git add nombre_del_archivo
Este comando agregará el archivo especificado al área de preparación (staging area) de Git, lo que significa que el archivo está listo para ser confirmado (commited).

Confirmar cambios
Una vez que hayas agregado los archivos que deseas confirmar, puedes confirmar los cambios utilizando el siguiente comando:

sql
Copy code
git commit -m "Mensaje de confirmación"
Este comando confirmará los cambios en el repositorio, utilizando el mensaje especificado para describir los cambios realizados.

Verificar el estado del repositorio
Puedes verificar el estado actual del repositorio utilizando el siguiente comando:

lua
Copy code
git status
Este comando te mostrará los archivos que han sido modificados, agregados o eliminados, y que aún no han sido confirmados.

Verificar el historial de confirmaciones
Puedes verificar el historial de confirmaciones (commits) en el repositorio utilizando el siguiente comando:

bash
Copy code
git log
Este comando te mostrará una lista de todas las confirmaciones realizadas en el repositorio, incluyendo los mensajes de confirmación y los autores.

Crear una nueva rama
Puedes crear una nueva rama en el repositorio utilizando el siguiente comando:

Copy code
git branch nombre_de_la_rama
Este comando creará una nueva rama en el repositorio, que se basará en la rama actual.

Cambiar a una rama existente
Puedes cambiar a una rama existente en el repositorio utilizando el siguiente comando:

Copy code
git checkout nombre_de_la_rama
Este comando cambiará a la rama especificada en el repositorio.

Fusionar ramas
Puedes fusionar dos ramas en el repositorio utilizando el siguiente comando:

sql
Copy code
git merge nombre_de_la_rama
Este comando fusionará la rama especificada con la rama actual del repositorio.

Actualizar el repositorio
Puedes actualizar el repositorio con los cambios más recientes desde el repositorio remoto utilizando el siguiente comando:

Copy code
git pull
Este comando descargará los cambios más recientes del repositorio remoto y los fusionará con la rama actual del repositorio.

Subir cambios al repositorio remoto
Una vez que hayas confirmado los cambios en el repositorio local, puedes subir los cambios al repositorio remoto utilizando el siguiente comando:

perl
Copy code
git push
Este comando subirá los cambios confirmados al repositorio remoto, lo que permitirá que otros usuarios accedan a los mismos.
git branch nombre_de_la_rama
Este comando creará una nueva rama en el repositorio, que se basará en la rama actual.

Cambiar a una rama existente
Puedes cambiar a una rama existente en el repositorio utilizando el siguiente comando:

Copy code
git checkout nombre_de_la_rama
Este comando cambiará a la rama especificada en el repositorio.

Fusionar ramas
Puedes fusionar dos ramas en el repositorio utilizando el siguiente comando:

sql
Copy code
git merge nombre_de_la_rama
Este comando fusionará la rama especificada con la rama actual del repositorio.

Actualizar el repositorio
Puedes actualizar el repositorio con los cambios más recientes desde el repositorio remoto utilizando el siguiente comando:

Copy code
git pull
Este comando descargará los cambios más recientes del repositorio remoto y los fusionará con la rama actual del repositorio.

Subir cambios al repositorio remoto
Una vez que hayas confirmado los cambios en el repositorio local, puedes subir los cambios al repositorio remoto utilizando el siguiente comando:

perl
Copy code
git push
Este comando subirá los cambios confirmados al repositorio remoto, lo que permitirá que otros usuarios accedan a los mismos.
