# git-commands

# Configuración inicial
Antes de utilizar Git, es recomendable configurar algunos datos iniciales, como tu nombre y correo electrónico. Puedes hacerlo utilizando los siguientes comandos:

   - git config --global user.name "Tu nombre"
   - git config --global user.email "Tu correo electrónico"



# Crear un nuevo repositorio
Para crear un nuevo repositorio de Git, puedes utilizar el siguiente comando:

  - git init //Este comando creará un nuevo repositorio de Git en el directorio actual.

# Agregar archivos al repositorio
Una vez que hayas creado un repositorio, puedes agregar archivos al mismo utilizando el siguiente comando:

  - git add nombre_del_archivo !Este comando agregará el archivo especificado al área de preparación (staging area) de Git, lo que significa que el archivo está listo para ser confirmado (commited).

# Confirmar cambios
Una vez que hayas agregado los archivos que deseas confirmar, puedes confirmar los cambios utilizando el siguiente comando:

  - git commit -m "Mensaje de confirmación" 
    Este comando confirmará los cambios en el repositorio, utilizando el mensaje especificado para describir los cambios realizados.

# Verificar el estado del repositorio
Puedes verificar el estado actual del repositorio utilizando el siguiente comando:

 - git status //Este comando te mostrará los archivos que han sido modificados, agregados o eliminados, y que aún no han sido confirmados.

# Verificar el historial de confirmaciones
Puedes verificar el historial de confirmaciones (commits) en el repositorio utilizando el siguiente comando:

  - git log //Este comando te mostrará una lista de todas las confirmaciones realizadas en el repositorio, incluyendo los mensajes de confirmación y los autores.

# Crear una nueva rama
Puedes crear una nueva rama en el repositorio utilizando el siguiente comando:

  - git branch nombre_de_la_rama //Este comando creará una nueva rama en el repositorio, que se basará en la rama actual.

# Cambiar a una rama existente
Puedes cambiar a una rama existente en el repositorio utilizando el siguiente comando:

  - git checkout nombre_de_la_rama //Este comando cambiará a la rama especificada en el repositorio.

#Fusionar ramas
Puedes fusionar dos ramas en el repositorio utilizando el siguiente comando:

 - git merge nombre_de_la_rama //Este comando fusionará la rama especificada con la rama actual del repositorio.

# Actualizar el repositorio
Puedes actualizar el repositorio con los cambios más recientes desde el repositorio remoto utilizando el siguiente comando:

  - git pull //Este comando descargará los cambios más recientes del repositorio remoto y los fusionará con la rama actual del repositorio.

# Subir cambios al repositorio remoto
Una vez que hayas confirmado los cambios en el repositorio local, puedes subir los cambios al repositorio remoto utilizando el siguiente comando:

  - git push //Este comando subirá los cambios confirmados al repositorio remoto, lo que permitirá que otros usuarios accedan a los mismos.
  
##################################################################################################


# GitFlow Workflow


# Ramas principales
   - master: La rama master representa el código en producción.
   - develop: La rama develop es la rama base para todas las demás ramas, y representa el código en desarrollo.

# Ramas de feature
   - feature-*: Las ramas de feature se crean a partir de la rama develop, y se utilizan para desarrollar nuevas características o funcionalidades. Cuando se completa      el trabajo en una rama de feature, se fusiona de vuelta en la rama develop.

# Para crear una nueva rama de feature:

   - git checkout develop
   - git pull origin develop
   - git checkout -b feature/nombre_de_la_caracteristica

# Cuando se completa el trabajo en la rama de feature:

   - git checkout develop
   - git pull origin develop
   - git merge --no-ff feature/nombre_de_la_caracteristica
   
# Ramas de bugfix
   - bugfix-*: Las ramas de bugfix se crean a partir de la rama master, y se utilizan para solucionar errores críticos en el código en producción. Cuando se completa      el trabajo en una rama de bugfix, se fusiona de vuelta en la rama master y en la rama develop.
   
# Para crear una nueva rama de bugfix:

  - git checkout master
  - git pull origin master
  - git checkout -b bugfix/nombre_del_error
   
# Cuando se completa el trabajo en la rama de bugfix:

  - git checkout master
  - git pull origin master
  - git merge --no-ff bugfix/nombre_del_error
  - git checkout develop
  - git merge --no-ff bugfix/nombre_del_error

# Ramas de release
  - release-*: Las ramas de release se crean a partir de la rama develop, y se utilizan para preparar el código para su lanzamiento en producción. En la rama de        release, se pueden realizar tareas como pruebas, corrección de errores y documentación. Cuando se completa el trabajo en una rama de release, se fusiona de vuelta en la rama master y en la rama develop.

# Para crear una nueva rama de release:

  - git checkout develop
  - git pull origin develop
  - git checkout -b release/nombre_de_la_version

# Cuando se completa el trabajo en la rama de release:

  - git checkout master
  - git pull origin master
  - git merge --no-ff release/nombre_de_la_version
  - git checkout develop
  - git merge --no-ff release/nombre_de_la_version
  
# Ramas de hotfix
   - hotfix-*: Las ramas de hotfix se crean a partir de la rama master, y se utilizan para solucionar errores críticos en el código en producción. Cuando se completa el trabajo en una rama de hotfix, se fusiona de vuelta en la rama master y en la rama develop.

# Para crear una nueva rama de hotfix:

   - git checkout master
   - git pull origin master
   - git checkout -b hotfix/nombre_del_error_critico

# Cuando se completa el trabajo en la rama de hotfix:

   - git checkout master
   - git pull origin master
   - git merge --no-ff hotfix/nombre_del_error_critico
   - git checkout develop



# Documentacion completa
https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=What%20is%20Gitflow%3F,lived%20branches%20and%20larger%20commits.
