# Como contribuir contenido al sitio web hsmty.org

Este repositorio está dedicado a la gestión y curación de contenido para [hsmty.org](https://hsmty.org).

El objetivo del contenido es compartir nuestros proyectos y publicar guías para aprender cómo 
realizarlos. 
Agradecemos las contribuciones de la comunidad para ayudarnos a crecer y mejorar esta colección.

## Contribuyendo

¡Puedes mandar tus contribuciones a este proyecto! 
Para mantener la calidad y coherencia de nuestro repositorio, pedimos que las colaboraciones sigan las siguientes pautas.

### Prerrequisitos

Antes de comenzar, asegúrate de tener Git instalado en tu sistema. 
Si eres nuevo en Git, puedes revisar la [documentación de Git](https://git-scm.com/doc) para una guía rápida.

### Configuración de tu Entorno

1. **Haz Fork del Repositorio**: Navega al [repositorio](https://github.com/hsmty/web_content) y haz clic en el botón 'Fork'. 
Esto creará una copia del repositorio en tu cuenta de GitHub.


2. **Clona tu Fork**: Abre tu terminal y ejecuta el siguiente comando para clonar el repositorio:
   ```
   git clone https://github.com/[TuUsuario]/web_content.git
   ```
   Reemplaza `[TuUsuario]` con tu nombre de usuario de GitHub.


3. **Agrega el repositorio original como Upstream**: Para mantener tu fork actualizado, agrega un remoto upstream:
   ```
   git remote add upstream https://github.com/hsmty/web_content.git
   ```

### Haciendo Cambios

1. **Crea una Nueva Rama**: Antes de empezar a trabajar en algo nuevo, jala lo último de upstream a tu rama public:
   ```commandline
   git checkout public
   git pull upstream
   ```
y luego crea tu rama basada en esta:

   ```commandline
   git checkout -b [nombre-rama]
   ```

   Reemplaza `[nombre-rama]` con un nombre descriptivo para tu rama.

2. **Realiza tus Cambios**: Haz los cambios necesarios en tu repositorio local.


3. **Confirma tus Cambios**: Después de realizar cambios, confírmalos en tu rama:
   ```
   git add .
   git commit -m "Un mensaje de commit descriptivo"
   ```

### Enviando tus Cambios

1. **Actualiza desde Upstream**: Antes de empujar tus cambios, actualiza con los últimos cambios desde el upstream:
   ```
   git pull upstream public
   ```

2. **Empuja a tu Fork**: Empuja tus cambios a tu fork:
   ```
   git push origin [nombre-rama]
   ```

3. **Crea un Pull Request**: Ve a tu fork en GitHub y haz clic en 'Nuevo Pull Request'. 
Compara tu rama con la rama principal del repositorio original y envía el pull request con una descripción clara de los cambios.

### Proceso de Revisión

Se revisarán las contribuciones y se dará retroalimentación mediante el sistema de Pull Request de GitHub. 
Si alguna persona de la comunidad se ofreció a revisar tu contribución, recuerda agregarle como reviewer. 
Apreciamos tu tiempo y esfuerzo en mejorar este proyecto.
