# ComandosLinux
Descripciones de algunos comandos en Linux

*******************************************************************

   *Este archivo muestra algunos comandos para la terminal de Linux*

   *Se incluye el comando y la descripción de los comandos*

   *Elaborado por: Israel Tosso García*

   *Sistemas Operativos*

********************************************************************

1.`pstree:` Muestra los procesos en ejecución del sistema. Se muestran en forma de árbol.

2.`sudo apt install + paquete:` instalar apps, por ejemplo firefox, se puede instalar directamente desde la tienda de linux o descargando el instalador y usando el comando 

3.`ping:` google.com    Hace ping de alguna página para verificar la conexión.

4.`ps -aux:` ver procesos del sistema.

5.`top:` ver procesos en tiempo real. 

6.`htop:` ver procesos con mas interfaz. 

7.`sudo apt install openssh-server:` instala openssh-server para conexiones remotas.

8.`ip addr:` ver ip.

9.`clear:` limpiar la ventana de la terminal.

10.`sudo su:` la sesión del terminal se vuelve en modo usuario root.

11.`whoami:` saber el usuario con el que estoy en la sesión actual.

12.`exit:` cerrar terminal.

13.`man + comando a preguntar:` ayuda de un comando, aparece un tipo de manual para la mayoría de los comandos. 

14.`cat + ruta del archivo:` mostrar contenido de un archivo.

15.`tail + -10 + ruta:` ver ultimas 10 filas de un archivo.

16.`head -10 + ruta:` ver primeras filas de un archivo.

17.`|:` concatenar comandos entre sí.

18.`more:` mostrar el resultado de la ejecución de un comando en la terminal de a una página a la vez.

19.`cd + nombre de la carpeta:` cambiar de carpeta.

20.`ls:` mostrar los archivos del directorio actual.

21.`pwd:` saber la ruta actual.

22.`cp + ruta archivo a copiar + ruta destino:` copiar archivos a otra ruta.

23.`mv + ruta archivo a copiar + ruta destino:` mover archivo de una ruta a otra.

24.`rm + ruta archivo:` eliminar un archivo.

25.`rm -R + ruta:` borrar un directorio.

26.`sudo rm -R / --no-preserve-root:` borrar toda la máquina (daña todo el sistema).

27.`history:` ver historial de todos los comandos utilizados durante esa sesión del terminal.

28.`sudo add-apt-repository ppa:numix/ppa -y:` crear repositorio nuevo

29.`sudo apt update:` refrescar lista de repositorios.

30.`sudo dpkg -i + ruta archivo a instalar:` instalar app descargada.

31.`telnet towel.blinkenlights.nl:` película de star wars.

32. `tar -cvf archivo.tar + nombre del archivo:` comprimir un archivo

33. `tar -xvf archivo.tar:` descomprimir archivo

34. `hostname:` ver el nombre del equipo

35. `reboot:` reiniciar

36. `shutdown:` apagar

37. `wget + URL:` descargar cualquier cosa de internet

38. `curl -X GET -L script.google.com/macros/s/AKfycbztjXtmKGK6nSZ2jyqwKvvFWrsT0qEmyxKvr15SjFCVQzy83TQ/exec?data=$nombre` Agregar datos a una hoja de calculo

39. `zenity --info --text="Mensaje"` Crear ventana informativa

40. `nombre=$(zenity --entry --text"Digite su nombre")` mensaje con entrada de texto

41. `zenity --password` Digitar una contraseña

42. `zenity --question` ventana de pregunta

43. `zenity --list --tittle="Comandos" --column="comando" --text="seleccione un comandode la lista" "ls -la" "ps -aux"` lista seleccionable

44. `chmod +x script.sh` Dar permisos de ejecución
