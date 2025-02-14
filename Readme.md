# Proyecto de Vinculación de Eclipse con GitHub

Este proyecto documenta el proceso de vinculación de un espacio de trabajo de Eclipse con un repositorio de GitHub. A continuación, se detallan los pasos seguidos para lograr esta integración.

## Autor
- **Nombre:** Jorge Castillo

## Descripción del Proyecto
El objetivo de este proyecto es vincular el espacio de trabajo de Eclipse con un repositorio remoto en GitHub. Esto incluye la creación de un repositorio público, la configuración de un archivo `.gitignore`.

## Pasos Seguidos

1. **Creación del Repositorio en GitHub**
   - Se creó un nuevo repositorio público en GitHub sin inicializar con `README.md` o `.gitignore`.

2. **Inicialización del Repositorio Local**
   - Se abrió una terminal y se navegó hasta la carpeta `eclipse-workspace`.
   - Se inicializó un nuevo repositorio con el comando `git init`.

3. **Configuración del Archivo `.gitignore`**
   - Se creó el archivo `.gitignore` con las siguientes reglas para ignorar archivos y directorios innecesarios:
     ```
     .metadata
     .classpath
     .project
     .settings/
     bin/
     ```

4. **Creación del Archivo `README.md`**
   - Se incluyó este archivo `README.md` con la información relevante del proyecto.

5. **Vinculación del Repositorio Local con el Remoto**
   - Se vinculó el repositorio local con el repositorio remoto utilizando el comando `git remote add origin <URL del repositorio>`.

6. **Primer Commit y Subida de Cambios**
   - Se añadieron los cambios con `git add .`.
   - Se realizó el primer commit con `git commit -m "Initial commit"`.
   - Se subieron los cambios al repositorio remoto con `git push -u origin master`.

7. **Verificación y Limpieza del Repositorio**
   - Se comprobó en GitHub que solo existían las carpetas `src` y otros archivos auxiliares necesarios.
   - Se eliminaron archivos y directorios de configuración no deseados con `git rm --cached <nombre>`.
   - Se actualizó el archivo `.gitignore` y se realizó un nuevo commit.

8. **Prueba de Nuevo Proyecto en Eclipse**
   - Se creó un nuevo proyecto en Eclipse con archivos `.java`.
   - Se confirmaron los cambios y se subieron al repositorio.
   - Se verificó que solo la carpeta `src` y los archivos de código fuente fueron subidos.

9. **Documentación y Eliminación del Repositorio**
   - Se documentó todo el proceso en un archivo PDF.
   - Se eliminó el repositorio de GitHub para evitar el acceso no autorizado al código.

## Estructura del Repositorio
- `src/`: Contiene el código fuente de los proyectos de Eclipse.
- `.gitignore`: Archivo que especifica qué archivos y directorios deben ser ignorados por Git.
- `README.md`: Este archivo, que proporciona una descripción del proyecto y los pasos seguidos.
