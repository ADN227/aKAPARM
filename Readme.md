# Crear una plantilla de ARM
![](https://akncus.blob.core.windows.net/git/8/K_073.jpg)

Una de las formas de manejar es con azure-cli. Para crear una plantilla con azure-cli usamos las opciones:

- **deployment**: Para crear una plantilla de deployment.
- **create**: Para crear una plantilla de arm.
- **group**: Para crear una plantilla de grupo.

- **--name**: Para indicar el nombre de la plantilla.
- **--resource-group**: Para indicar el grupo de recursos donde se creará la plantilla.
- **--template-file**: Para indicar el archivo de plantilla.

Para crear una plantilla de ARM necesitamos un archivo de plantilla con extension [```.json```](azuredeploy.json).

en una terminal ejecutamos el comando:

    az group deployment create --name <my-deployment> --resource-group <my-resource-group> --template-file <my-template>.json

Si revisamos los recursos del grupo de recursos, podemos ver la cuenta de almacenamiento correspondiente a la plantilla.
![](https://akncus.blob.core.windows.net/git/8/K_076.jpg)

Al revzisar la sección **Implementaciones** dentro del grupo de recursos donde se creó la plantilla podemos ver que se creó una plantilla con el nombre **my-deployment**. 
![](https://akncus.blob.core.windows.net/git/8/K_074.jpg)

Al revisar la **Implementacio** en la **Plantilla** vemos el archivo json.
![](https://akncus.blob.core.windows.net/git/8/K_075.jpg)
