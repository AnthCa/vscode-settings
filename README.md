# Instrucciones

**NOTA:** Tómate un momento para leer la breve documentación de **"Custom CSS and JS Loader"** para obtener algunos consejos útiles sobre varios sistemas operativos y evitar problemas con los cambios que no se aplican correctamente.

1. Instala la extensión "Custom CSS and JS Loader" de VS Code.
2. Copia el contenido de `settings.json` a tu archivo `settings.json` de VS Code (advertencia: sobrescribirá tu configuración actual).
3. Añade el array `vscode_custom_css.imports` a tu archivo `settings.json`:
   ```json
   "vscode_custom_css.imports": [
       // Rutas absolutas de tus archivos css/js
       // Para Mac o Linux
       // "file:///Users/tu-nombre-de-usuario/custom-vscode.css",
       // "file:///Users/tu-nombre-de-usuario/custom-vscode-script.js"

       // Para Windows
       // "file:///C:/ruta-de-css-personalizado/custom-vscode.css",
       // "file:///C:/ruta-de-css-personalizado/custom-vscode-script.js"
   ],
4.	Es posible que necesites tomar posesión de los archivos CSS/JS que hayas creado o ejecutar VS Code con privilegios de administrador en ciertos sistemas operativos:
    Usuarios de Mac y Linux
    La extensión NO funcionará si Visual Studio Code no puede modificarse a sí mismo. Los casos incluyen:

    Archivos de código de solo lectura, como en un sistema de archivos de solo lectura o,
    VS Code no se inicia con los permisos necesarios para modificarse a sí mismo.
    Necesitas reclamar la propiedad del directorio de instalación de Visual Studio Code, ejecutando este comando:

    Nota: Reemplaza /usr/share/code con la ubicación donde está instalado tu VS Code.
    sudo chown -R tu-nombre-de-usuario /usr/share/code

5.	Habilita “Custom CSS and JS Loader” desde el diálogo de comandos de VS Code.
6.	Personaliza el CSS o JS desde este repositorio para que luzca como lo deseas, o incluso mejor, explora áreas de VS Code que quieras personalizar.
7.	Después de realizar algunos cambios, recarga la extensión (Recargar CSS y JS personalizados) desde el diálogo de comandos de VS Code.


