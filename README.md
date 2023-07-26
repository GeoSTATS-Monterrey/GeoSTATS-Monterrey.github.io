# GeoSTATS-Monterrey.github.io
Esta es la página web utilizada para almacenar los diferentes mapas y elementos que se muestran en la página web principal de GeoSTATS Monterrey.

## Agregar una sub-página
Para agregar una nueva subpágina, solo se debe de crear una nueva carpeta con el nombre de la subpágina, y dentro de esta carpeta se deben de colocar los archivos correspondientes a la sub-página, estos pueden ser archivos de texto, imágenes, videos, etc. además de un archivo llamado `index.md` o `index.html` que será el archivo que se mostrará al entrar a la sub-página.

## Agregar un mapa de qgis
Para agregar un mapa, se debe de crear una subpágina para este, y después se debe acceder al plugin de qgis2web dentro de la app de qgis teniendo el mapa abierto. Dentro del menú de opciones del plugin, se deben de seleccionar las opciones deseadas. La gran mayoría de las funcionalidades que se aplican a los mapas exportados provienen de la opción “appearance”  donde se pueden habilitar elementos interactivos para el usuario. Hasta este momento lo que ha funcionado mejor ha sido leaflet a comparación de open layers. Una vez exportado, se deben de copiar los archivos generados dentro de la carpeta de la sub-página (sin eliminar el .git ni .readme). Una vez hecho esto, simplemente se tienen que subir los cambios al repositorio remoto y la página web se actualizará automáticamente en unos minutos.

# Haciendo el embebido en la página principal
Una vez teniendo el mapa en la github page, se simplifica el proceso de hacer el embebido para mostrarlo. Para hacerlo se necesita un elemento de wix que muestra una vista de una página especificada, que en este caso será la que se creó dentro de la github page, tomando la url específica de la subpágina con el elemento a mostrar. Una vez configurado el elemento, el mapa aparecerá automáticamente y se actualizará si se hacen cambios a la github page.
