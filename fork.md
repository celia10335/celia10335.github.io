## TRABAJANDO CON FORK EN GITHUB
En GitHub, hacer un "fork" se puede traducir como "bifurcar un proyecto". Esto es, hacer una copia de un proyecto de otra persona para hacer los cambios que se quieran sin afectar al proyecto original. Esta copia del proyecto se guarda como un repositorio nuevo en nuestro GitHub, de manera que si hacemos push, no va a afectar al repositorio de la otra persona que creó el proyecto, aunque se le puede solicitar que añada esos cambios al proyecto original mediante "pull request" (solicitud de subida de cambios).

### Paso 1: Crear bifurcación
Elegimos un repositorio cualquiera en www.github.com, ya sea nuestro o de otra persona (lo suyo es que sea de otro usuario).
En la esquina superior izquierda, encontramos la pestaña Fork, la desplegamos y elegimor "Crete new fork".

![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%202022-10-02%20102052.jpg)

![](https://github.com/celia10335/celia10335.github.io/blob/main/capturas%20fork/Captura%20de%20pantalla%20de%202022-09-29%2009-32-12.png)

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

