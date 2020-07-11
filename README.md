# Deepin-wallpaper-blur-for-Nvidia

![Captura que muestra el error](https://raw.githubusercontent.com/igatjens/Deepin-wallpaper-blur-for-Nvidia/master/Screen%20Capture_20200711112142.png)
Captura que muestra el error - Screenshot showing error

![Captura que muestra el resultado después de aplicar el parche](https://raw.githubusercontent.com/igatjens/Deepin-wallpaper-blur-for-Nvidia/master/Screen%20Capture_20200711112749.png)
Captura que muestra el resultado después de aplicar el parche - Screenshot showing the result after applying the patch

# Español

Este parche es para solucionar un problema en Deepin cuando se usa el driver privativo de Nvidia. El problema es que cuando se establecen fondos de escritorio que no son los fondos por defecto de Deepin, el menú de aplicaciones a pantalla completa se muestra con fondo negro en vez de mostrar un efecto blur (borroso) del fondo de escritorio.

1. Descargue el parche de blur_image

2. Agregar permisos de ejecución al parche

`chmod +x blur_image`

3. Respaldar `blur_image` original

`sudo mv /usr/bin/blur_image /usr/bin/blur_image-backup`

4. Copiar el parche a `/usr/bin`

`sudo cp blur_image /usr/bin/`

5. Limpiar el caché de wallpapers con blur

`sudo rm /var/cache/image-blur/*.jpg`


# English

This patch is to fix a problem in Deepin when using the proprietary Nvidia driver. The problem is that when setting wallpapers other than Deepin's default backgrounds, the full-screen application menu is shown with a black background instead of showing a blur effect of the desktop background.

1. Download the blur_image patch

2. Add execute permissions to the patch

`chmod + x blur_image`

3. Backup original `blur_image`

`sudo mv / usr / bin / blur_image / usr / bin / blur_image-backup`

4. Copy the patch to `/ usr / bin`

`sudo cp blur_image / usr / bin /`

5. Clear cache of wallpapers with blur

`sudo rm /var/cache/image-blur/*.jpg`
