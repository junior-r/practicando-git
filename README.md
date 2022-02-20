# Mis Notas Durante el curso

# CREANDO RAMAS

- Crear ramas ------------------------> git checkout -b <nombre_rama> 
- Cambiar de ramas -------------------> git switch <nombre_rama>
- Ver todas las ramas existentes -----> git branch
- Ver todos los commit de las ramas --> git log --oneline --all --graph --decorate

# FUSIONANDO RAMAS

- Unir ramas -----> git merge <nombre_rama>
traerá todos los commits de la rama que se le indicó.
Una vez que se unen las ramas, se elimina la que se creó a partir de master, porque no tiene sentido que siga existiendo.
Solo se puede eliminar una rama desde otra, no se puede eliminar estando parado en ella.
- Eliminar rama --> git branch -D <nombre_rama>

Si un mismo archivo se edita en dos ramas diferentes al momento del merge dará un error, la solución es manual, se tiene que evaluar que se queda y que se va.
- Abortar Merge --> git merge --abort

# IGNORANDO ARCHIVOS

crear en la raíz del proyecto un archivo .gitignore y dentro poner el nombre del archivo a ignorar, con su extensión.
Ignorar carpetas --> ./nombre_carpeta

# TRABAJANDO CON GITHUB

- Clonar un repositorio HTTPS ---> git clone <direccion_del_repositorio>
- Clonar un repositorio SSH -----> git clone <dirección_ssh>
  - Hacer esto si no tienes una llave SSH para clonar
    - cd -> ssh-keygen -t rsa
    - cd .ssh
    - cd  id_rsa.pub -> copiar y pegar en github agregar nueva llave
- Subir a Github ----------------> git push origin <rama>
- Saber a donde estoy subiendo el código --> git remote -v
- fetch -> descargar commits desde un repositorio
- git fetch origin
- traer archivos --> git pull origin <rama>
- push -> subir info a un repositorio

- Eliminar una rama remota ------> git push --delete origin <rama>
