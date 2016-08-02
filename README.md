# Plantilla para Gitbook en Español 

> Un proyecto semilla para Gitbook

## ¿Qué es esto?

Este es un proyecto plantilla para la creación de libros usando Gitbook.

## ¿Qué software se necesita para instarlo?

Ud. debe tener instalado [Node.js](https://nodejs.org), [Git]((https://git-scm.com/downloads)) y las [herramientas de línea de comandos de Gitbook](https://github.com/GitbookIO/gitbook-cli)

- Para node.js
    - para revisar si node.js esta instalaod, puede ejecutar:  

    ```
    $ npm -v
    ```
    
    - Si no está instalado, debe descargar e instalar el software desde [el sitio oficial de node.js](https://nodejs.org/en/download/)

- Para Git
    - Para revisar si Git está instalado, puede ejecutar:  

    ```
    $ git --version
    ```
    
    - Si no está instalado, debe descargar e instalar el software desde [el sitio oficial de Git](https://git-scm.com/downloads)

- Para las herramiemtas de línea de comandos de Gitbook
    - Para revisar si Gitbook-Cli está instalado, puede ejecutar:

    ```
    $ gitbook -V
    ```

    - Si no está instalado, se puede instalar el paquete usando ``npm``  como un usuario administrador  

    ```
    $ npm install -g gitbook-cli
    ```
    
    - En linux o mac, puede usar ``sudo`` para definir el usuario y la ruta para la carpeta ``.npm`` e instalar el paquete  

    ```
    $ export PATH=$PATH:$HOME/.npm-packages/bin
    $ sudo chown -R $USER:$GROUP ~/.npm
    $ sudo npm install -g gitbook-cli
    ```


## ¿Cómo instalarlo?

Si desea editar el libro usando el [Gitbook Editor](https://www.gitbook.com/editor), solo necesita clonar o hacer un "fork" del proyecto. 
Es posible crear un nuevo libro dentro del editor de Gitbook usando el repositorio Git resultante.

Si desea publicar el libro en un sitio de [Github-Pages](https://pages.github.com/), debe cambiar el URL para el repositorio en el archivo ``package.json``.

- Revise el URL del repositorio en el Github.
- Reemplace el URL del repositorio. Por defecto, el URL aparece "noname/noname.git". 

## ¿Cómo ejecutarlo?

El proyecto incluye una serie de comandos que pueden ser usados para automatizar parte del proceso.


- **Para instalar o actualizar los plugins** de Gitbook

  ```
  $ npm run book:prepare
  ```

- **Para visualizar el libro**.
    Este comando ejecuta un servidor web que permite revisar el libro a medida que se escribe.
    Cualquier cambio en el libro se actualiza inmediatamente en el sitio web.

  ```
  $ npm run book:watch
  ```

- **Para crear el libro** (en Windows)

  ```
  $ npm run book:build
  ```

- **Para publicar el libro** en el sitio web de Github-Pages (en Windows)

  ```
  $ npm run book:publish
  ```

- **Para crear el libro** (en Linux)

  ```
  $ npm run book:build-linux
  ```

- **Para publicar el libro** en el sitio web de Github-Pages (en Linux)

  ```
  $ npm run book:publish-linux
  ```
