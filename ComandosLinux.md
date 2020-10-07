# ComandosLinux
Descripciones y ejemplo de algunos comandos en Linux

*******************************************************************

   *Este archivo muestra algunos comandos para la terminal de Linux*

   *Se incluye el comando, descripción y ejemplos de los comandos*

   *Elaborado por: Israel Tosso García*

   *Sistemas Operativos*

********************************************************************

1.`pstree:` Muestra los procesos en ejecución del sistema.

systemd─┬─ModemManager───2*[{ModemManager}]

        ├─NetworkManager───2*[{NetworkManager}]
        
        ├─3*[VBoxClient───VBoxClient───2*[{VBoxClient}]]
        
        ├─VBoxClient───VBoxClient───3*[{VBoxClient}]
        
        ├─VBoxService───8*[{VBoxService}]
        
        ├─accounts-daemon───2*[{accounts-daemon}]
        
        ├─acpid
        
        ├─anacron
        
        ├─avahi-daemon───avahi-daemon
        
        ├─colord───2*[{colord}]
        
        ├─cron
        
        ├─cups-browsed───2*[{cups-browsed}]
        
        ├─cupsd
        
        ├─dbus-daemon
        
        ├─fwupd───4*[{fwupd}]
        
        ├─gdm3─┬─gdm-session-wor─┬─gdm-x-session─┬─Xorg───{Xorg}
        
        │      │                 │               ├─gnome-session-b─┬─ssh-agent
        
        │      │                 │               │                 └─2*[{gnome-+
        
        │      │                 │               └─2*[{gdm-x-session}]
        
        │      │                 └─2*[{gdm-session-wor}]
        
        │      └─2*[{gdm3}]


2.`sudo apt install + paquete:` instalar apps 

3.`ping:` google.com

4.`ps -aux:` ver procesos 

5.`top:` ver procesos en tiempo real 

6.`htop:` ver procesos con mas interfaz 

7.`sudo apt install openssh-server:`

8.`ip addr:` ver ip 

9.`clear:` limpiar la ventana terminal

10.`sudo su:` root 

11.`whoami:` saber el usuario con el que estoy 

12.`exit:` cerrar terminal 

13.`man + comando a preguntar:` ayuda de un comando 

14.`cat + ruta del archivo:` mostrar contenido de un archivo 

15.`tail + -10 + ruta:` ver ultimas 10 filas de un archivo

16.`head -10 + ruta:` ver primeras filas de un archivo

17.`|:` concatenar comando con el símbolo

18.`more:` visualizar archivos concatenar con

19.`cd + nombre de la carpeta:` cambiar de carpeta 

20.`ls:` mostrar archivos directorio actual

21.`pwd:` saber la ruta actual

22.`cp +ruta archivo a copiar + ruta destino:` copiar archivos

23.`mv + ruta archivo + destino:` mover archivo 

24.`rm + ruta archivo:` eliminar archivo

25.`rm -R + ruta:` borrar un directorio

26.`sudo rm -R / --no-preserve-root:` borrar toda la máquina (daña todo el sistema)

27.`history:` ver historial de comandos

28.`sudo add-apt-repository ppa:numix/ppa -y:` crear repositorio nuevo

29.`sudo apt update:` refrescar lista de repositorios

30.`sudo dpkg -i + ruta archivo a instalar:` instalar app descargada

31.`telnet towel.blinkenlights.nl:` película de star wars
