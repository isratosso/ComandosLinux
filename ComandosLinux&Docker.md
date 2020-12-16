# ComandosLinux y Docker
Descripciones de algunos comandos en Linux y Docker

*******************************************************************

   *Este archivo muestra algunos comandos para la terminal de Linux y Docker*

   *Se incluye el comando, la descripción de los comandos y algunos ejemplos*

   *Elaborado por: Israel Tosso García*

   *Sistemas Operativos*

********************************************************************
# Linux
1.`pstree:` Muestra los procesos en ejecución del sistema. Se muestran en forma de árbol.

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
        ├─containerd───8*[{containerd}]
        ├─cron
        ├─cups-browsed───2*[{cups-browsed}]
        ├─cupsd
        ├─dbus-daemon
        ├─dockerd───9*[{dockerd}]
        ├─fwupd───4*[{fwupd}]
        

2.`sudo apt install + paquete` instalar apps, por ejemplo firefox, se puede instalar directamente desde la tienda de linux o descargando el instalador y usando el comando 

3.`ping google.com` Hace ping de alguna página para verificar la conexión.

    itossog964@ubuntu-ulacit:~$ ping google.com
    PING google.com (142.250.64.206) 56(84) bytes of data.
    64 bytes from mia07s56-in-f14.1e100.net (142.250.64.206): icmp_seq=1 ttl=114 time=98.2 ms
    64 bytes from mia07s56-in-f14.1e100.net (142.250.64.206): icmp_seq=2 ttl=114 time=89.1 ms
    64 bytes from mia07s56-in-f14.1e100.net (142.250.64.206): icmp_seq=3 ttl=114 time=114 ms
    64 bytes from mia07s56-in-f14.1e100.net (142.250.64.206): icmp_seq=4 ttl=114 time=90.1 ms


4.`ps -aux` ver procesos del sistema.

    itossog964@ubuntu-ulacit:~$ ps -aux
    USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
    root           1  0.5  0.3 103392 13168 ?        Ss   19:20   0:03 /sbin/init sp
    root           2  0.0  0.0      0     0 ?        S    19:20   0:00 [kthreadd]
    root           3  0.0  0.0      0     0 ?        I<   19:20   0:00 [rcu_gp]
    root           4  0.0  0.0      0     0 ?        I<   19:20   0:00 [rcu_par_gp]
    root           6  0.0  0.0      0     0 ?        I<   19:20   0:00 [kworker/0:0H
    root           8  0.0  0.0      0     0 ?        I<   19:20   0:00 [mm_percpu_wq
    root           9  0.3  0.0      0     0 ?        S    19:20   0:02 [ksoftirqd/0]
    root          10  0.0  0.0      0     0 ?        I    19:20   0:00 [rcu_sched]
    root          11  0.0  0.0      0     0 ?        S    19:20   0:00 [migration/0]
    root          12  0.0  0.0      0     0 ?        S    19:20   0:00 [idle_inject/
    root          13  0.0  0.0      0     0 ?        I    19:20   0:00 [kworker/0:1-
    root          14  0.0  0.0      0     0 ?        S    19:20   0:00 [cpuhp/0]
    root          15  0.0  0.0      0     0 ?        S    19:20   0:00 [kdevtmpfs]
    root          16  0.0  0.0      0     0 ?        I<   19:20   0:00 [netns]
    root          17  0.0  0.0      0     0 ?        S    19:20   0:00 [rcu_tasks_kt
    root          18  0.0  0.0      0     0 ?        S    19:20   0:00 [kauditd]


5.`top` ver procesos en tiempo real. 

    itossog964@ubuntu-ulacit:~$ top

    top - 19:33:50 up 13 min,  1 user,  load average: 0,08, 0,33, 0,46
    Tareas: 181 total,   3 ejecutar,  178 hibernar,    0 detener,    0 zombie
    %Cpu(s):   0,0/0,0     0[                                                     ]
    MiB Mem :   3936,4 total,   1538,1 libre,    863,4 usado,   1534,9 búfer/caché
    MiB Intercambio:   2048,0 total,   2048,0 libre,      0,0 usado.   2819,1 dispon

    PID USUARIO   PR  NI    VIRT    RES    SHR S  %CPU  %MEM     HORA+ ORDEN    
    438 root      20   0       0      0      0 I   1,4   0,0   0:02.06 kworker+ 
    1266 itossog+  20   0  229308  61448  41732 R   1,4   1,5   0:09.43 Xorg     
    1565 itossog+  20   0  157968   2764   2396 S   1,4   0,1   0:05.89 VBoxCli+ 
    1635 itossog+  20   0 3388568 306184 122504 S   1,4   7,6   0:14.51 gnome-s+ 
      1 root      20   0  103392  13168   8608 S   0,0   0,3   0:04.64 systemd  
      2 root      20   0       0      0      0 S   0,0   0,0   0:00.00 kthreadd
      
6.`htop` ver procesos con mas interfaz. 

7.`sudo apt install openssh-server` instala openssh-server para conexiones remotas.

8.`ip addr` ver ip.

    itossog964@ubuntu-ulacit:~$ ip addr
    1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
        link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
      inet 127.0.0.1/8 scope host lo
         valid_lft forever preferred_lft forever
      inet6 ::1/128 scope host 
         valid_lft forever preferred_lft forever
    2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
        link/ether 08:00:27:71:8a:8c brd ff:ff:ff:ff:ff:ff
      inet 192.168.0.11/24 brd 192.168.0.255 scope global dynamic noprefixroute enp0s3
        valid_lft 2752sec preferred_lft 2752sec
      inet6 fe80::5866:8f15:2ee5:c919/64 scope link noprefixroute 
        valid_lft forever preferred_lft forever
    3: docker0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN group default 
      link/ether 02:42:a4:e6:c5:e2 brd ff:ff:ff:ff:ff:ff
      inet 172.17.0.1/16 brd 172.17.255.255 scope global docker0
        valid_lft forever preferred_lft forever


9.`clear` limpiar la ventana de la terminal.

10.`sudo su` la sesión del terminal se vuelve en modo usuario root.

11.`whoami` saber el usuario con el que estoy en la sesión actual.

12.`exit` cerrar terminal.

13.`man + comando a preguntar` ayuda de un comando, aparece un tipo de manual para la mayoría de los comandos. 

14.`cat + ruta del archivo` mostrar contenido de un archivo.

15.`tail + -10 + ruta` ver ultimas 10 filas de un archivo.

16.`head -10 + ruta` ver primeras filas de un archivo.

17.`|` concatenar comandos entre sí.

18.`more` mostrar el resultado de la ejecución de un comando en la terminal de a una página a la vez.

19.`cd + nombre de la carpeta` cambiar de carpeta.

20.`ls` mostrar los archivos del directorio actual.

21.`pwd` saber la ruta actual.

22.`cp + ruta archivo a copiar + ruta destino` copiar archivos a otra ruta.

23.`mv + ruta archivo a copiar + ruta destino` mover archivo de una ruta a otra.

24.`rm + ruta archivo` eliminar un archivo.

25.`rm -R + ruta` borrar un directorio.

26.`sudo rm -R / --no-preserve-root` borrar toda la máquina (daña todo el sistema).

27.`history` ver historial de todos los comandos utilizados durante esa sesión del terminal.

28.`sudo add-apt-repository ppa:numix/ppa -y` crear repositorio nuevo

29.`sudo apt update` refrescar lista de repositorios.

30.`sudo dpkg -i + ruta archivo a instalar` instalar app descargada.

31.`telnet towel.blinkenlights.nl` película de star wars.

32. `tar -cvf archivo.tar + nombre del archivo` comprimir un archivo

33. `tar -xvf archivo.tar` descomprimir archivo

34. `hostname` ver el nombre del equipo

35. `reboot` reiniciar

36. `shutdown` apagar

37. `wget + URL` descargar cualquier cosa de internet

38. `curl -X GET -L script.google.com/macros/s/AKfycbztjXtmKGK6nSZ2jyqwKvvFWrsT0qEmyxKvr15SjFCVQzy83TQ/exec?data=$nombre` Agregar datos a una hoja de calculo

39. `zenity --info --text="Mensaje"` Crear ventana informativa

40. `nombre=$(zenity --entry --text"Digite su nombre")` mensaje con entrada de texto

41. `zenity --password` Digitar una contraseña

42. `zenity --question` ventana de pregunta

43. `zenity --list --tittle="Comandos" --column="comando" --text="seleccione un comandode la lista" "ls -la" "ps -aux"` lista seleccionable

44. `chmod +x script.sh` Dar permisos de ejecución

# Docker

1. `docker pull store/gitlab/gitlab.ce:10.2.4-ce.0` Servidor de software

2.`docker pull sw4iot/isc-dhcp` Servidor DHCP

3.`docker pull gartz/simple-dns` Servidor DHCP

4.`docker pull itsthenetwork/nfs-server-alpine` Servidor SSH, FTP, SAMBA

5.`docker pull stanback/alpine-samba` Servidor SSH, FTP, SAMBA

6.`docker pull stilliard/pure-ftpd` Servidor FTP y servidor web

7.`docker pull inwt/r-shiny` Servidor FTP y servidor web

8.`docker pull nextcloud` Servidor de respaldos

9.`docker pull minimum2scp/squid` servidor proxy

10.`docker pull splunk/splunk` Servidor de Logs

11.`docker pull kalilinux/kali-linux-docker` Kali linux

12.`docker pull ubuntu` ubuntu

13.`docker pull wordpress` wordpress

14.`docker pull joomla` joomla

15.`docker pull centos` centos

16.`docker images` ver las imagenes instaladas

17.`sudo docker run -it ubuntu` entrar a la consola de una maquina virtual
