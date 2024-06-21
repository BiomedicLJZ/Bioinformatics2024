
markdown
# Introducción a Linux 101

## ¿Qué es Linux?

Linux es un sistema operativo de código abierto basado en Unix. Fue creado por Linus Torvalds en 1991 y ha crecido para convertirse en uno de los sistemas operativos más utilizados en el mundo, especialmente en servidores, supercomputadoras y dispositivos móviles (como Android). Linux es conocido por su estabilidad, seguridad y flexibilidad, lo que lo convierte en una elección popular para desarrolladores y científicos.

### Ventajas de Linux

- **Código abierto**: Cualquier persona puede ver, modificar y distribuir el código fuente.
- **Estabilidad**: Ideal para servidores y aplicaciones que requieren alta disponibilidad.
- **Seguridad**: Menos susceptible a virus y malware en comparación con otros sistemas operativos.
- **Comunidad activa**: Gran cantidad de soporte y documentación disponibles.
- **Velocidad** para manejar grandes volumenes de datos
- **Control** De tu computadora recursos y sistema

## El Root File System (Sistema de Archivos Raíz)

El root file system, o sistema de archivos raíz, es el directorio principal en un sistema operativo Linux desde el cual se accede a todos los demás archivos y directorios. Es representado por el símbolo `/` y contiene todos los archivos necesarios para iniciar y operar el sistema operativo.

### Estructura del Sistema de Archivos

En linux todo es un archivo, esta filosofia a conllevado que todo aquello proceso, movimiento etc sea manejado mediante el sistema de archivos, de algunos de los directorios más importantes que se encuentran en el sistema de archivos raíz de Linux:
```
/
├── bin
├── boot
├── dev
├── etc
│   ├── systemd
│   ├── network
│   └── ...
├── home
│   ├── usuario1
│   ├── usuario2
│   └── ...
├── lib
├── media
│   ├── usb
│   ├── cdrom
│   └── ...
├── mnt
│   ├── disk1
│   ├── disk2
│   └── ...
├── opt
├── root
├── sbin
├── tmp
├── usr
│   ├── bin
│   ├── lib
│   ├── local
│   └── ...
└── var
    ├── log
    ├── mail
    └── ...

```



- `/bin`: Contiene los binarios esenciales del usuario (comandos y utilidades básicas) que son necesarios para el sistema en modo de usuario único.
  ```bash
  ls /bin
  ```

- `/boot`: Contiene los archivos necesarios para arrancar el sistema, como el cargador de arranque y el kernel.
  ```bash
  ls /boot
  ```

- `/dev`: Contiene archivos de dispositivo, que son interfaces para el hardware y los dispositivos periféricos del sistema.
  ```bash
  ls /dev
  ```

- `/etc`: Contiene archivos de configuración del sistema y scripts de inicio.
  ```bash
  ls /etc
  ```

- `/home`: Directorio que contiene los directorios personales de los usuarios.
  ```bash
  ls /home
  ```

- `/lib`: Contiene bibliotecas esenciales para los binarios ubicados en `/bin` y `/sbin`.
  ```bash
  ls /lib
  ```

- `/media` y `/mnt`: Directorios usados para montar sistemas de archivos externos, como unidades USB o discos duros adicionales.
  ```bash
  ls /media
  ls /mnt
  ```

- `/opt`: Contiene paquetes de software adicionales que no vienen preinstalados con el sistema operativo.
  ```bash
  ls /opt
  ```

- `/root`: Directorio personal del usuario root (superusuario).
  ```bash
  ls /root
  ```

- `/sbin`: Contiene binarios esenciales para la administración del sistema, accesibles solo por el superusuario.
  ```bash
  ls /sbin
  ```

- `/tmp`: Directorio para almacenar archivos temporales.
  ```bash
  ls /tmp
  ```

- `/usr`: Contiene aplicaciones y archivos utilizados por los usuarios.
  ```bash
  ls /usr
  ```

- `/var`: Contiene archivos que varían con el tiempo, como logs, bases de datos, y colas de impresión.
  ```bash
  ls /var
  ```

### Importancia del Sistema de Archivos Raíz

El sistema de archivos raíz es crucial para el funcionamiento del sistema operativo Linux. Es la estructura jerárquica donde se almacenan todos los archivos necesarios para el sistema, y su organización permite una gestión eficiente de los recursos y una navegación intuitiva para los usuarios.

## Principales comandos en Linux

A continuación, se presentan algunos de los comandos más utilizados en Linux:

### Navegación de directorios

- `pwd`: Muestra el directorio de trabajo actual. 
  ```bash
  pwd
  ```

- `ls`: Lista los archivos y directorios en el directorio actual.
  ```bash
  ls
  ```

- `cd`: Camb

io el directorio de trabajo.
  ```bash
  cd /home/usuario
  ```

### Manipulación de archivos y directorios

- `touch`: Crea un archivo vacío o actualiza la fecha de modificación de un archivo.
  ```bash
  touch archivo.txt
  ```


- `mkdir`: Crea un nuevo directorio.
  ```bash
  mkdir nuevo_directorio
  ```

- `cp`: Copia archivos o directorios.
  ```bash
  cp archivo.txt copia_archivo.txt
  ```


- `mv`: Mueve o renombra archivos o directorios.
  ```bash
  mv archivo.txt nuevo_nombre.txt
  ```

- `rm`: Elimina archivos o directorios.
  ```bash
  rm archivo.txt
  ```
  
  **Nota**: Usa `rm -r` para eliminar directorios y su contenido.
  ```bash
  rm -r directorio
  ```

### Visualización y edición de archivos

- `cat`: Muestra el contenido de un archivo.
  ```bash
  cat archivo.txt
  ```

- `nano` o `vi`: Editores de texto en la línea de comandos.
  ```bash
  nano archivo.txt
  ```

  ```bash
  vi archivo.txt
  ```

### Gestión de permisos

- `chmod`: Cambia los permisos de un archivo o directorio.
  ```bash
  chmod 755 script.sh
  ```

- `chown`: Cambia el propietario de un archivo o directorio.
  ```bash
  chown usuario:grupo archivo.txt
  ```

### Información del sistema

- `top`: Muestra los procesos en ejecución y el uso de recursos del sistema.
  ```bash
  top
  ```

- `df`: Muestra el uso del disco.
  ```bash
  df -h
  ```


- `free`: Muestra el uso de la memoria.
  ```bash
  free -m
  ```


### Gestión de paquetes

En distribuciones basadas en Debian (como Ubuntu):

- `apt-get update`: Actualiza la lista de paquetes disponibles.
  ```bash
  sudo apt-get update
  ```


- `apt-get upgrade`: Actualiza los paquetes instalados.
  ```bash
  sudo apt-get upgrade
  ```


- `apt-get install`: Instala un nuevo paquete.
  ```bash
  sudo apt-get install nombre_paquete
  ```


## Uso de Linux en Bioinformática

Linux es ampliamente utilizado en bioinformática debido a varias razones:

1. **Herramientas de código abierto**: Muchas herramientas bioinformáticas, como BLAST, BWA y Bowtie, están disponibles en Linux.
2. **Capacidad de scripting**: La capacidad de crear scripts en bash y otros lenguajes como Python permite automatizar tareas complejas y repetitivas.
3. **Potencia y rendimiento**: Linux es el sistema operativo preferido para ejecutar aplicaciones de alto rendimiento en clústeres de computadoras y supercomputadoras.
4. **Compatibilidad**: La mayoría de los software bioinformáticos y bibliotecas están diseñados para ejecutarse en Linux.
5. **Comunidad y soporte**: Una gran comunidad de usuarios y desarrolladores en bioinformática utiliza Linux, lo que facilita encontrar soporte y compartir soluciones.

### Ejemplos de uso

- **Secuenciación de ADN**: Herramientas como FASTQC, BWA, y GATK se ejecutan eficientemente en Linux para analizar datos de secuenciación.
- **Análisis de expresión génica**: Software como DESeq2 y edgeR en combinación con Linux permite analizar y visualizar datos de RNA-Seq.
- **Modelado y simulación**: Programas como GROMACS para simulaciones de dinámica molecular se ejecutan en entornos Linux debido a su eficiencia y escalabilidad.

## Conclusión

Linux es una herramienta poderosa y flexible que es esencial para el trabajo en bioinformática. Con el conocimiento básico de comandos y la capacidad de utilizar y desarrollar herramientas bioinformáticas, los científicos pueden maximizar su eficiencia y reproducibilidad en la investigación.

---

¡Gracias por su atención!
