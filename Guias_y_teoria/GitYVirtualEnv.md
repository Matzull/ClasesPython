# Cheatsheet para Git y Virtualenv

## Git

### Configuración inicial

* git config --global user.name "nombre": Establecer el nombre de usuario.
* git config --global user.email "correo electrónico": Establecer el correo electrónico asociado al usuario.

### Comandos básicos

* git init: Inicializar un repositorio Git en la carpeta actual.
* git add .: Agregar todos los cambios en la carpeta actual al área de preparación.
* git commit -m "mensaje": Realizar un commit con un mensaje descriptivo.
* git status: Mostrar el estado actual del repositorio.
* git log: Mostrar el registro de commits del repositorio.

### Trabajar con remotos

* git remote add origin URL: Agregar un repositorio remoto con la URL especificada.
* git push -u origin rama: Empujar la rama actual al repositorio remoto.
* git pull: Traer los cambios más recientes del repositorio remoto.
* git clone URL: Clonar un repositorio remoto en la carpeta actual.

## Virtualenv

### Instalación

* pip install virtualenv: Instalar Virtualenv.

### Crear y activar un entorno virtual

* virtualenv nombre_entorno: Crear un nuevo entorno virtual con el nombre especificado.
* Se puede cambiar con defaultprofilewindows el terminal
* Activar el entorno
  * Mac/linux: source nombre_entorno/bin/activate.
  * Windows: nombre_entorno\Scripts\activate. (Atencion al sentindo de las barras \\ )

### Instalar paquetes y exportar requisitos

* pip install nombre_paquete: Instalar un paquete en el entorno virtual.
* pip freeze > requirements.txt: Exportar los paquetes instalados en un archivo de requisitos.

### Desactivar y eliminar un entorno virtual

* deactivate: Desactivar el entorno virtual actual.
* rm -rf nombre_entorno: Eliminar el entorno virtual con el nombre especificado.
