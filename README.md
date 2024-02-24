# GIT (Github)
				  ### Local
## repositorio <
				  ### Remoto
## git config user.name				
*** git config --global user.name "Jane Doe" ***


## 122334+nomre@users.noreply.github.com
git config --global user.email "oscardo@miEmpresa.com"
*** git config user.email ***

# crear reporitorio: git init 

*** tres áreas en GIT ***
	>Directorio de trabajo (ruta en windows) working Directory
	>	Área de preparación --              staging area (add)
	>		Commit 
	>			reporitorio --              Repository (.git)

*** Estado ***
>git status
>	git add <archivo o carpeta>
>		git commit -m "cualquier ruta o archivo"
>			git log 
>		git commit --amend #reporitorio Local
>		git reset --soft head~1 (para volver atrás en el tiempo del commit, volvemos el archivo a staging area >       o preparación)
		
*** Ramas en git ***
	LINEAS INDEPENDIENTE DE DESARROLLO
		branch --- ramas
	git branch version-javascript (creamos la rama)
	git branch (visualizamos la(s) ramas)
	git checkout version-javascript (cambiar a una rama)
	git checkout -b version-python (crear e ir a la ruta de la rama)
		git branch -m version-js (modificar el nombre de la rama)
		o 
		git branch -m version-python version-py (cambiar el nombre de la rama)
	git branch -d version-py (Deleted branch version-py (was cba0009).) eliminar esta rama que hemos creado
	git log --oneline (solo muestra los datos en una sola linea)
	git log -p
--- Funcionar ramas ---
	merge --- fusionar la versión
	PROCESO QUE PERMITE COMBINAR VARIAS LÍNEAS INDEPENDIENTES DE DESARROLLO EN UNA SOLA RAMA
	para FUSIONAR DOS RAMAS, DEBES DEBES ESTAR EN LA RAMA QUE RECIBIRÁ la FUSIÓN
	(main) git merge <rama que se desea fusionar> 
	<rama raiz donde se desea fusionar> git merge <rama a fusionar>
	
--- GITHUB ---
git remote 
	--origin (el nombre que se le asigno al servidor de git)
git remote -v
origin  https://github.com/oscardo/repositorio.git (fetch) --> obtener la información del repositorio remoto a mi local
origin  https://github.com/oscardo/repositorio.git (push)  --> dejar la información que hemos hecho de nuestro local al repositorio remoto

--- Git Push ---
Comando usado para enviar los cambios realizados en un repositorio local a un repositorio remoto 
para que ambos tengan la misma información
	git push origin 
	
--- Git Pull ---
Comando usaod para descargar el contenido de un repositorio remoto e inmediamente actualiza un reporitorio local 
para que ambos tengan la misma información
	git pull origin main (origin  remoto ... main local)
--- Git fetch ---
Comando usado para verificar los cambios realizados en los repositorios remotos SIN combinar esos cambios con el 
repositorio local.
te permite saber SI SE HAN REALIZADO CAMBIOS en el repositorio remoto desde la última vez que actualizarte tu reporitorio local con git pull
	git fetch 

--- Adicionar un git remoto ---
git remote -v
(ninguno)
git remote add origin "www.remotesite.com/algo.git"

--- fork (bifurcar un repositorio)
git fork 

Un fork es una copia de un repositorio de Git en tu cuenta. Te permite:
¿Cuándo usar un fork?

Para contribuir a un proyecto de código abierto.
Para probar ideas sin afectar al proyecto original.
Para aprender de la experiencia de otros desarrolladores.
¡Crea tu propio fork y empieza a explorar!

--- Pull Request ---
Solicitud de combinar tus cambios con el reporitorio original del proyecto
git pull request --- 
Git Pull Request:

Solicitud de cambios: Un desarrollador propone cambios a un proyecto.
Colaboración: Permite discutir y revisar los cambios antes de integrarlos.
Integración: Los cambios se fusionan en la rama principal del proyecto

