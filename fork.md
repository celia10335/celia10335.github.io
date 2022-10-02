## TRABAJANDO CON FORK EN GITHUB
En GitHub, hacer un "fork" se puede traducir como "bifurcar un proyecto". Esto es, hacer una copia de un proyecto de otra persona para hacer los cambios que se quieran sin afectar al proyecto original. Esta copia del proyecto se guarda como un repositorio nuevo en nuestro GitHub.

### Paso 1: Crear bifurcación
Elegimos un repositorio cualquiera en www.github.com, ya sea nuestro o de otra persona (lo suyo es que sea de otro usuario).
En la esquina superior izquierda, encontramos la pestaña Fork, la desplegamos y elegimos "Crete new fork".

Se creará un repositorio en nuestro GitHub a partir de la copia que vamos a hacer. Le ponemos un nombre.

![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%202022-10-02%20132217.jpg)

 
Hacemos clic en "Aceptar" a todas las opciones que vengan por defecto. Ya estaría hecha la bifurcación.
 
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-31-42.png)


### Paso 2: Clonar repositorio en nuestro equipo
Lo más adecuado para trabajar en esta copia de proyecto es llevarlo a nuestro repositorio local, es decir, clonarlo en nuestro ordenador.
En nuestro equipo, debemos crear una carpeta donde ubicar este repositorio. En el ejemplo, he creado un directorio llamado "Bifurcando", y ahí he ubicado "E_cliente_Manu".

```sh
git clone git@github.com:celia10335/E_Cliente_Manu.git
```

![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-33-04.png)

 
### Paso 3: Modificar la copia del proyecto como queramos
Hacemos las modificaciones que queramos sobre nuestra bifurcación. En este caso, he modificado el archivo README.md.
 
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-33-59.png)

Como siempre, para subir los cambios a nuestro repositorio remoto (GitHub), ejecutamos los comandos "add", "commit" y "push".
```sh
git add .
git commit
git push
```
 
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-34-31.png)
 
 

### Paso 4: Solicitar que los cambios que hemos hecho se fusionen con el proyecto original: "pull request"
Vamos al repositorio de GitHub que contiene la bifurcación y hacemos clic en el segundo icono por la derecha, "pull request". Seleccionamos "New pull request".
 
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-31-26.png)
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-31-02.png)
 
Si el propietario del proyecto original acepta, en su repositorio se verá algo así. Como se puede comprobar, el archivo README.md se ha actualizado con los cambios que hicimos en nuestra copia.
 
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-28-27.png)
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-28-41.png)
![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-29-20.png)


## DIFERENCIAS ENTRE FORK Y CLONE
Realmente, fork y clone se refieren a cosas totalmente distintas. Clone es la operación que nos sirve para traer un repositorio remoto a nuestro repositorio local. Esto también lo vamos a realizar con el repositorio que ha resultado de la bifurcación, ya que se crea un repositorio aparte.

Entonces, podríamos decir que la diferencia estaría en qué repositorio estamos clonando. ¿Estamos clonando el repositorio original o el repositorio "fork", que es una copia? De eso va a depender también los "commit" que hagamos. Si intentamos hacer un "commit" de un repositorio que no es nuestro, deberemos estar habilitados como colaboradores, de lo contrario no se reflejarán los cambios.

Sin embargo, podemos hacer los "commit" que queramos en la bifurcación, ya que realmente es un repositorio de nuestra propiedad que refleja una copia de otro. No va a afectar al repositorio original, salvo que el propietario acepte nuestro "pull request".
