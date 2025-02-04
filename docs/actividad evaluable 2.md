

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

**Iván Gutiérrez Raimundo**

**DAW 2º DISTANCIA   2024-2025**

**DESPLIEGUE**







# ACTIVIDAD EVALUABLE- 2 -Ejercicio de Git


<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

<br>

<br>

<br>

<br>

<br>

<br>

<br>

<br>

<br>

<br>

<br>

[TOC]


## **TRABAJO LOCAL**

1. Inicializa un nuevo repositorio Git en una carpeta llamada `"labdist"` y agrega los
archivos proporcionados en el aula virtual. Renombra la rama master a `main` , si es
necesario. Realiza el primer commit. Muestra el log del repositorio.

```bash
$ git config --global merge.ff false
$ git init
$ git branch –M main
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\1\1.1.primera parte.png)

- Realizado primer commit

```bash
$ git add .

$ git commit -m "primer commit"
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\1\1.1. segunda parte commit.png)



- Log del repositorio

```bash
$ git log
$ git log –oneline
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\1\1.1.3 parte log.png)



2. Incluye un fichero `.gitignore` para que los ficheros `README.md` , `LICENCE.txt` y
`passwords.txt` sean ignorados por el control de versiones. Realiza el commit y muestra
los logs del repositorio en una línea.



- Archivo `.gitignore` creado:

```bash
$ notepad .gitignore

$ git add .gitignore

$ git commit -m "archivo gitignore creado"
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\2\1.2.1 crear archivo gitignore.png)

- Edito el archivo `.gitignore` y meto los archivos a ignorar,luego hago commit

```bash
$ nano .gitignore

$ git add.
$ git commit –m “"gitignore configurado con los archivos a ignorar"
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\2\1.2.2edito el archivo gitignore.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\2\sigo editando gitignore.png)

- Log

```bash
$ git log --oneline
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\2\log de la 1.2.png)

3. En el repositorio, crea los archivos `README.md` , `LICENCE.txt` y `passwords.txt` con
   algún contenido. Muestra el estado del repositorio. Muestra el listado de archivos
   ignorados.

   

- Creo los archivos e intento hacer commit , no se puede , los ignora .

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\3\3 . archivos creados.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\3\ignora los archivos al hacer commit.png)

- Estado del repositorio

```bash
$ git status
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\3\estado del repositorio.png)



- Listado de archivos ignorados

```bash
$ git ls-files --others --ignored --exclude-standard
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\3\listado archivos ignorados.png)



4. Crea una rama `feature-estilos` . Cámbiate a ella.
   Modifica el archivo `estilos.css` :
   propiedad color del `body` y de `h2` : `#2a2a2a`
   propiedad `background-color` de `header` y `footer`: `#2a75ff`
   Comprueba el estado del repositorio. Añade los cambios, realiza un commit con el
   mensaje "actualizados estilos a azules"



- Crear rama y entrar en ella

```bash
$ git branch feature-estilos
$ git checkout feature-estilos
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\4\crear rama y entrar.png)



- Cambio el código css

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\4\cambios en css.png)



- Estado, añadir los cambios y  hacer commit

```bash
$ git status 
$ git add .
$ git commit –m “actualizados estilos azules”
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\4\estado y commit de los cambios en rama.png)



5. Vuelve a la rama `main` . En el archivo `index.html` añade un comentario donde se indique
   tu nombre como autor de la página. Comprueba el estado del repositorio. Añade los
   cambios, realiza un commit con el mensaje ' añadido autor en index'. Muestra los logs del
   repositorio en una línea, gráficamente y con 'decoración'



- Cambio de rama a `main`

```bash
$ git checkout main
```

- Cambio en el código de `index.html`

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\5\cambio en index html.png)

- Estado del repositorio , añadidos los cambios y commit realizado

```bash
$ git status
$ git add .
$ git commit –m “añadido autor en index”
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\5\subido el cambio de index.png)

- Log del repositorio en una línea, gráficamente y con decoración 

```bash
$ git log --all --decorate --oneline --graph
```

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\5\log grafico.png)

6. Fusiona la rama `feature-estilos` en la rama `main` . Muestra los logs del repositorio en
   una línea, gráficamente y con 'decoración'

   - Hacemos un merge para realizar la fusión (desde la rama `main`)

   ```bash
   $ git merge feature-estilos
   ```

   - Log del repositorio en una línea, gráficamente y con decoración 

   ```bash
   $ git log --all --decorate --oneline --graph
   ```


   ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en local\6 fusion realizada y log grafico.png)



## **TRABAJO EN REMOTO**



1. Continúa con el repositorio `labdist` . Añade el repositorio a **Sourcetree**

   

   ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\1\añadido labdist a sourcetree.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\1\añadido labdist a sourcetree 2.png)

2. En tu cuenta de GitHub, crea un repositorio remoto y sube al remoto los ficheros de tu
  repositorio local. Debes subir todas las ramas. Muestra, además, la captura de pantalla
  donde se vean en GitHub.

  - En el icono de settings, situado en la pestaña de remoto, añado el repositorio remoto (add) con la URL.

  ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\2\1 en settings añado repo remoto.PNG)

  ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\2\añado el repositorio remoto a sourcetree.png)

  - Le damos al icono de PUSH y seleccionamos todas las ramas

  ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\2\subo todas las ramas.png)

  

  - Vemos q en github aparecen el repositorio con todas las ramas

  ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\2\ramas subidas a github.png)



3.  En el repositorio local, crea una rama `feature-index` . Añade el siguiente código dentro
   de la `<section class="about">` . Añade los cambios y crea un commit con el mensaje
   "Añadido párrafo equipo en index.html". Sube los cambios al remoto. (Recuerda que
   debes usar SourceTree en todo este apartado )

- Creo la rama feature-index pulsando en el icono BRANCH

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\creo rama feature-index.png)

- Añado cambios en el código de index.html

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\añadido parrafo en index.png)

- Añado cambios (add)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\add cambios.PNG)

- Hago el commit

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\commit cambios.PNG)

- Subo cambios al remoto (PUSH), vemos ahora que hay tres ramas en el remoto.
  ![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\subo cambios al remoto.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\3\tres ramas.png)



4. En el repositorio local, fusiona la rama `feature-index` en la rama `main` .

- Situado en la rama `main` , hacemos la fusion dando al icono merge, seleccionamos rama a fusionar.(si le das un click en la rama a fusionar antes de dar a merge y queda sombreada ya saldrá seleccionada).

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\4\realizo merge.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\4\MERGE REALIZADO.png)

5. Edita el fichero `contacto.html` . Borra unas líneas. Muestra los ficheros con cambios
   pendientes y las diferencias. Añade los cambios y haz un commit.

- Edito fichero contacto, borro unas líneas del footer

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\5\BORRO LINEAS DE FOOTER.png)

- Ficheros con cambios pendientes y diferencias a la derecha

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\5\CAMBIOS PENDIENTES Y DIFERENCIAS.png)

- Commit realizado 

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\5\commit realizado.png)



6. Te das cuenta del error. Deshaz TOTALMENTE el commit anterior. Captura el estado
   actual del repositorio. (Asegúrate de que el fichero `contacto.html` ha recuperado todas
   las líneas borradas y no hay cambios pendientes en el repositorio.)

- Selecciono el commit anterior al que quiero volver, con el botón derecho seleciono `“Reset current branch  to this commit”`

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\6\Selecciono commit anterior pa volver.png)



- Selecciono la opción reset HARD , que volverá totalmente al commit anterior sin dejar ningún rastro ni ningún cambio .

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\6\reset hard seleccionado.png)



7. Crea una rama feature-mapa y cámbiate a ella. Incluye este código en el archivo
   `contacto.html` . Añade los cambios. Realiza un commit.

- rama creada

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\7\rama creada.png)

- Archivo contacto modificado

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\7\Contacto html modificado.png)

- Commit realizado

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\7\contacto html commiteado.png)



8. Sube los cambios al remoto - los de todas las ramas. Muestra en el remoto los cambios
   del archivo `contacto.html` en la rama `feature-mapa` .



- Subo todas las ramas al remoto

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\8\subo todas las ramas al remoto.png)

- Muestro los cambios en el repositorio remoto hechos en `contacto.html` en la rama `feature-mapa`

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\8\muestro cambios en remoto.PNG)



9. En GitHub, en la rama main , fusiona la rama feature-mapa . Baja los cambios del remoto
   a local. Deja los dos repositorios sincronizados. Muestra una captura de pantalla donde
   se vea la página principal de tu repositorio remoto

- Fusiono las ramas con pull request 

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\fusiono con pull request.png)

- Abro un pull request

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\abro un pull request.png)

- Hago el merge y lo confirmo

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\hago el merge.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\confirmo.png)

- Bajo los cambios a local

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\bajo los cambios al local.png)

- Los dos repositorios sincronizados

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\repositorio sincronizado 1.png)



![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\trabajo en remoto\9\repositorio sincronizado 2.png)



## **CONFLICTO**

1.Crea una rama `hotfix-js` . Cámbiate a ella. Añade este código en el fichero `script.js` .
Confirma el cambio y haz un commit con el mensaje "corregido problema en script.js".
(Fíjate en los números de línea de tu editor ...)

- Rama creada

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\1\creada rama hotfix.png)

- Código añadido en script.js

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\1\cambio en script.png)

- Commit realizado

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\1\commit hecho.png)

2. Vuelve a la rama `main` . En el fichero `script.js` en las mismas líneas que en la cuestión
   anterior, añade el código siguiente. Confirma el cambio y haz un commit con el mensaje
   "corregido problema en script.js rama main".

- Cambiado el código en script.js en las mismas líneas que el anterior

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\2\cambio en codigo script.js.png)

- Commit realizado

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\2\commit cambio.png)



3. Fusiona la rama `hotfix-js` en `main` . Debe producirse un conflicto. Resuélvelo como
   consideres oportuno. Cuando termines la resolución del conflicto sube los cambios al
   remoto

Hacemos merge

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\hacemos merge.png)

Conflicto creado warning

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\conflicto.png)

Resuelvo desde visual studio , elijo quitar por favor

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\conflicto desde visual studio.png)

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\resuelvo quitando porfavor.png)

Cambio enviado a remoto

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\cambio enviado al remoto.png)



![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\cambio enviado al remoto2.png)



Resuelto el conflicto 

![](C:\Users\Guty\Desktop\DESPLIEGUE\TAREA 2\capturas\conflictos\3\resuelto conflicto.png)





## **VIDEOCLIP**

https://www.loom.com/share/0ac4c48bbdb94f4e948a87047b5167cb?sid=01d70436-dd53-43a3-b8c8-8816243ef540





## **Bibliografía o Webgrafía**

- Apuntes y ejercicios de clase

- Pro Git - Chacon, Scott; Straub Straub

- https://aprendeconalf.es/docencia/git/manual/

- Curso sourcetree de TheHarryCode: https://www.youtube.com/playlist?list=PLdX95r_5VhojrYffoY3OEySCW4RlEtaMG



## **Repositorio remoto (GitHub)**







