# Ejercicio - Crear un paquete

En este ejercicio, aprenderas a utilizar entornos virtuales como una forma para no afectar a los paquetes instalados globalmente u otros programas que se ejecutan en tu maquina.

*Para este ejercicio es necesario que lo ejecutes desde la terminal, linea de comandos, cdm consola, cli, etc. de u computadora, se que es desafiante, pero no te preocupes ¡¡Se que puedes lograrlo!!*

# Crear un entorno virtual

Crea un entorno virtual mediante ``venv``

* Ejecutar en su terminal: ``python3 -m venv env`` o bien ``python -m venv env``
 
    ```
       python3 -m venv env
    ```   
    ``
    python -m venev env
    ``
    Ahora tienes un directorio (folder)  ``env`` creado en tu terminal.

* Ejecuta el comando  para activar el entorno virtual: ``source env/bin/activate``

 ``` 
 source env/env/bin/activate 
 # windows
 env\bin\activate

 o bien: 
 env\Scripts\activate

 # Linux, WSL or macOS
 source env\bin\activate
``` 

Ahora vez en tu terminal``(env)`` . Eso significa que has activado tu entorno virtual y se ha aislado del resto de tu maquina.

![image]https//user.images.githubusercontent.com/9124597/153076991-25e857c5-a910-4d54-80b9-47fce1b62147.png

## instalar una biblioteca

Ahora que estas dentro de tu entorno virtual. puedes instalar una biblioteca y saber que la biblioteca solo existira en el entorno virtual.

* Ejecuta comando ``pip freeze`` para ver  las bibliotecas instaladas en tu entorno:

    ```
    pip freeze
    ```
     
    No deberias obtener respuesta. A continuacion, veamos como cambia la salida de pip freeze cuando se agrega una biblioteca (un paquete).

* Ejecuta el comando ``pip install`` para instalar una biblioteca:
   ```
   pip install python dateutil
   ```
* un gran mensaje de salida de texto dice que esta instalando tu biblioteca. y debe terminar con la siguiente oracion:

    ```
    Successfully installed python-dateutil-2.8.2 six-1.16.0
    ```
* Vuelve a ejecutar ```pip freeze``` para ver como a cambiado tu lista de bibliotecas:
    ```
    pip freeze 
    ```
* Ahora deberias ver la siguiente lista:
    ```
    python-deteutil==2.8.2
    six==1.16.0
    ```
### Desactivar un entorno virtual

Hata ahora, has creado un entorno virtual y le has agregado un paquete. Sin embargo, es posible que estes trabajando en varios proyectos de Python y necesites cambiar entre ellos. Para hacer eso, debes salir (desactivar) tu entorno virtual.

Ejecute el comando ``deactivate``:
```
deactive
```

Observa como cambia el mensaje de tu terminal  ``(env)`` a como se veia antes.

¡Felicidades! Has logrado crear y usar correctamente un entorno virtual.



























