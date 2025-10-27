<div align="center">
<h1>Proyecto 2</h1>
  <p>
    Ingeniería Electrónica · Universidad Santo Tomás
    <br>
    <b>Didier Posse</b>
    <br>
    <em>Instalación</em>
  </p>
</div>

<hr>

<div align="center">
  <h2>Instalación del Administrador (MV Debian)</h2>
</div>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/53cde341-d1c2-41a4-9733-c5c73dabc977"/></p>
    </div>
    <p>
      El proceso inicia con la configuración básica de la instalación. Es fundamental elegir primero el <b>idioma del sistema</b> y la <b>distribución del teclado</b>. 
      Normalmente, estos pasos se realizan en una interfaz por consola bastante sencilla, asegurando que el instalador entienda nuestras preferencias regionales para continuar correctamente con la instalación.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/cf4476f8-daa8-43de-b89f-d5a23311b4d3"/></p>
    </div>
    <p>
      Tras establecer el idioma, el sistema comienza a <b>cargar los componentes adicionales de instalación</b>. 
      Este paso permite continuar con la descarga y preparación de los paquetes esenciales que más adelante formarán parte del sistema operativo una vez finalizada la instalación.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/1b456f08-81e8-450c-b036-5d3299a496ca"/></p>
    </div>
    <p>
      Luego, se nos pide ingresar el <b>nombre de la máquina</b>. Este no corresponde ni al nombre del superusuario ni al del usuario principal, 
      sino simplemente al nombre con el cual se identificará la computadora o máquina virtual dentro de la red o el entorno del sistema.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/bf0ce814-2666-4440-b235-4b7f39defda5"/></p>
    </div>
    <p>
      A partir de este punto, el instalador solicita datos importantes para la seguridad del sistema. 
      Primero pide el <b>nombre del dominio</b> que tendrá el sistema operativo, luego se define la <b>contraseña del usuario Root</b> (la cuenta con máximos privilegios). 
      Después, se ingresan el <b>nombre completo del nuevo usuario</b>, el <b>nombre de usuario</b> (identificador corto) y finalmente la <b>contraseña personal</b>. 
      Es decir, en esta etapa configuramos tanto la cuenta de superusuario como la cuenta de uso diario de manera ordenada y segura.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b19fd2c7-f537-4b25-b0eb-6633e72876df"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/d1006cb0-138b-45c1-b75a-4256c634f236"/></p>
    </div>
    <p>
      Luego llegamos a la parte de <b>particionado del disco</b>. En este punto, <b>Debian</b> ofrece varias opciones para gestionar el disco asignado desde <b>Virtual Manager</b>. 
      En mi caso, utilicé la opción <b>"Guiado - Utilizar todo el disco"</b>, ya que es la forma más sencilla y automática de particionar. 
      El instalador realiza este proceso por nosotros.<br>
      Después de elegir esta opción, el sistema pide confirmar la unidad (la asignada al crear la VM) y aceptar <b>escribir los cambios en el disco</b> para continuar con la instalación.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/475708ce-a467-4ee2-a7a8-fab277d964b4"/></p>
    </div>
    <p>
      A continuación, se inicia la <b>instalación base del sistema</b>. 
      Este proceso instala los componentes esenciales que permiten que el sistema operativo funcione. 
      Aquí todavía no se incluyen el entorno gráfico ni las aplicaciones adicionales, solo se configura el sistema principal en su forma más básica.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/48c5f138-ee71-4495-a7e9-4c503f3abb05"/></p>
    </div>
    <p>
      Una vez confirmado el particionado, el instalador solicita elegir los <b>paquetes de software</b> que queremos incluir. 
      Esta es la parte donde decidimos si instalamos un <b>entorno gráfico</b> (como <b>GNOME</b> o <b>Xfce</b>) y otros servicios opcionales.<br>
      Para optimizar el rendimiento y mantener un sistema más liviano, elegí <b>Xfce</b>, un entorno gráfico ligero pero muy cómodo. 
      Además, seleccioné el <b>servicio SSH</b> (necesario para la comunicación entre entornos del proyecto) y las <b>utilidades estándar del sistema</b>, por si son necesarias más adelante.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/367a2976-9e63-4821-a36f-c0517b3a406c"/></p>
    </div>
    <p>
      En este punto, el sistema pregunta si queremos <b>instalar el cargador de arranque GRUB</b> en el registro principal del disco. 
      Esto es esencial para que la máquina virtual pueda iniciar correctamente el sistema operativo. 
      Debemos seleccionar <b>"Sí"</b> y luego elegir el disco donde se instaló Debian para completar este paso.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/5b9f3657-72ca-480d-83b0-f3fbeb9eeb42"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/ad6747e5-403d-49e1-96e1-1d8cfe005b70"/></p>
    </div>
    <p>
      Si todo ha salido bien, la máquina virtual se reinicia y nos solicita ingresar las <b>credenciales del usuario</b> que creamos previamente. 
      Una vez dentro, se muestra la <b>interfaz principal del escritorio de Debian</b>, confirmando que la instalación fue exitosa y que ya podemos empezar a trabajar normalmente dentro del sistema.
    </p>
  </li>
</ol>

<hr>

<div align="center">
  <h2>Instalación de Dependencia Recursos Humanos</h2>
</div>

<h2>Instalación MV Arch Linux (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/9115ce50-29b8-442f-8abb-4aefb5dd0cd1"/></p>
    </div>
    <p>
      El primer paso es ir a la <b>página oficial de Arch Linux</b>, donde aparece la opción para <b>descargar la imagen (.iso)</b> del sistema operativo.  
      Luego se selecciona la región donde se desea instalar y la versión del sistema operativo; por facilidad, elegí la más reciente (v10.01).  
      La imagen pesa aproximadamente <b>1.4 GB</b>, lo cual no es mucho.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/c56bf092-b92d-47e7-9d7b-662432e4fdc8"/></p>
    </div>
    <p>
      El siguiente paso, si se quiere instalar como máquina virtual, es tener ya configurado el <b>virtualizador</b>; en mi caso utilicé <b>QEMU</b>.  
      Aquí se realiza todo el proceso de creación de la VM: seleccionar la ubicación de la imagen <b>(.iso)</b>, el sistema operativo a instalar, la <b>memoria RAM</b> y los <b>núcleos de CPU</b> que se le asignarán.  
      Con eso listo, se puede iniciar el arranque del booteable y continuar con la instalación.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/516913c7-616f-4c5a-b5d6-e8c94801c46b"/></p>
    </div>
    <p>
      Al iniciar y seleccionar la opción <b>"Arch Linux install"</b>, se abre una <b>terminal</b> desde donde se deben ejecutar los comandos de instalación y configuración.  
      Esto permite instalar exactamente lo que uno necesita, logrando un sistema operativo más <b>ligero y optimizado</b>.  
      Sin embargo, también requiere cuidado, ya que es más fácil cometer errores.  
      En caso de duda, se puede consultar la <b>guía oficial</b> de instalación en la página de Arch Linux.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/ea80567f-5f8a-4cd9-9cbb-e7f2eedc3309"/></p>
    </div>
    <p>
      Luego, con el comando <code>cfdisk /dev/vda</code>, se abre la herramienta para <b>crear la partición</b> donde se instalará Arch Linux.  
      Aquí se debe elegir el tipo de tabla de particiones (GPT, DOS, SGI o SUN).  
      La opción más recomendable es <b>DOS</b>, ya que las demás pueden generar errores en algunos casos.  
      Después, se crea una nueva partición, se guardan los cambios y se sale para continuar con la instalación.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/f3afe47a-c5b8-4f98-893b-cedd3894e907"/></p>
    </div>
    <p>
      Una vez creada la partición, se formatea con <code>mkfs.ext4 /dev/vda1</code>.  
      Luego se monta el disco con <code>mount /dev/vda1 /mnt</code> para poder configurarlo directamente.  
      Después se instala el sistema base con el comando:  
      <code>pacstrap /mnt base linux linux-firmware nano networkmanager grub</code>.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/12438c10-17dd-48b9-ad9b-d5e1f20fb936"/></p>
    </div>
    <p>
      Aquí se puede ver cómo debería aparecer la instalación base.  
      En mi caso, tuve un error por escribir mal un comando, ya que el <b>teclado por defecto</b> en esta terminal es el <b>US</b> (inglés), porque aún no se ha configurado el idioma.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/01c443a8-ce32-4f27-87c5-42229c0a8523"/></p>
    </div>
    <p>
      Luego se genera el archivo <b>fstab</b> con el comando  
      <code>genfstab -U /mnt >> /mnt/etc/fstab</code>.  
      Después, se puede entrar al sistema montado con  
      <code>arch-chroot /mnt</code> para continuar con la configuración.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/e78d8a19-9fd9-45e0-9aac-42a79671b745"/></p>
    </div>
    <p>
      Una vez dentro del sistema, se configura la <b>zona horaria</b> con los comandos:  
      <code>ln -sf /usr/share/zoneinfo/America/Bogota /etc/localtime</code> y <code>hwclock --systohc</code>.  
      Luego se instala el <b>bootloader</b> (GRUB), que es el encargado de iniciar los sistemas operativos.  
      Para instalarlo junto a sus herramientas se usa:  
      <code>pacman -S grub dhcpcd</code>.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/98e23a58-5f61-4bd9-ac82-bae7b07a0345"/></p>
    </div>
    <p>
      También se puede instalar el <b>GRUB</b> directamente con el comando <code>grub-install /dev/vda</code>, aunque no es necesario usar ambos métodos.  
      Luego de instalarlo, se debe generar su configuración con  
      <code>grub-mkconfig -o /boot/grub/grub.cfg</code>.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/34624e05-573c-49f9-b909-cdeb7a970373"/></p>
    </div>
    <p>
      Después de configurar el GRUB, se habilita la red con  
      <code>systemctl enable NetworkManager</code>.  
      Si se instaló el GRUB con herramientas, también se puede activar con  
      <code>systemctl enable dhcpcd</code>.  
      Luego se instala el <b>entorno gráfico</b> con:  
      <code>pacman -S xorg xfce4 lightdm lightdm-gtk-greeter</code>.  
      Este entorno es <b>ligero y eficiente</b>, ideal si no se quiere usar GNOME, que es más pesado.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/a6ff8826-ce11-43dd-82a3-67425a3cab1e"/></p>
    </div>
    <p>
      Ya para finalizar, se habilita el entorno gráfico con <code>systemctl enable lightdm</code>.  
      Si se desea agregar una <b>contraseña al usuario root</b>, se usa <code>passwd</code>.  
      Para crear un nuevo usuario:  
      <code>useradd -m -G wheel &lt;nombre_usuario&gt;</code>,  
      y para asignarle una contraseña:  
      <code>passwd &lt;nombre_usuario&gt;</code>.  
      Finalmente, se sale con <code>exit</code>, se desmonta todo con <code>umount -R /mnt</code> y se reinicia el sistema con <code>reboot</code>.  
      Al hacerlo, el sistema ya arrancará con el entorno gráfico completamente funcional.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width=850 src="https://github.com/user-attachments/assets/179a83df-883b-4221-94af-c2e396089b4e"/></p>
      <p><img width=850 src="https://github.com/user-attachments/assets/16157070-5b5b-4f73-b46f-efe6ba3638e6"/></p>
    </div>
    <p>
      Finalmente, se debería ver la <b>pantalla de inicio de sesión</b> y el <b>entorno gráfico</b> funcionando correctamente.  
      Aquí aparecen las aplicaciones y configuraciones por defecto del sistema, manteniendo un <b>bajo consumo de recursos</b>.
    </p>
  </li>
</ol>

<h2>Instalación Contenedor CentOS</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/582fb4b8-dc77-49b4-bc88-45009d46f773"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/2dd191c4-1839-4e2d-9975-4b2828beecff"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<hr>

<div align="center">
  <h2>Instalación de Dependencia Tecnológica</h2>
</div>

<h2>Instalación Maquina Virtual Rocky Linux (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      Al descargar la imagen <b>(.iso)</b> desde la página oficial de <b>Rocky Linux</b>, se ingresa a <b>QEMU</b> para crear la máquina virtual. 
      En este proceso, se debe definir la <b>ubicación de la imagen (.iso)</b>, asignar una <b>partición del disco</b>, memoria <b>RAM</b> y los <b>núcleos de la CPU</b> del PC.  
      <br><br>
      Luego de completar esta configuración inicial, aparecerá el mensaje donde se puede elegir entre <b>instalar</b> o <b>testear</b> el sistema para comprobar si el hardware es compatible y todo funciona             correctamente antes de proceder con la instalación.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7c3b7d74-288d-475b-892a-7dcf704d3031"/></p>
    </div>
    <p>
      Aquí se muestra la <b>configuración de la instalación</b> de Rocky Linux.  
      La imagen <b>(.iso)</b> detecta automáticamente el <b>idioma</b>, la <b>distribución del teclado</b> y otras configuraciones básicas por defecto.  
      <br><br>
      Sin embargo, es necesario seleccionar el <b>disco de instalación</b> (el que se asignó previamente desde Virtual Manager), además de configurar la <b>cuenta root</b> y crear el <b>usuario principal</b> junto con su respectiva contraseña.  
      Estas configuraciones son esenciales para garantizar el acceso y la administración del sistema después de la instalación.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/518480eb-3598-49f3-b3a2-b18b1095d38e"/></p>
    </div>
    <p>
      Luego comienza la <b>instalación del sistema operativo</b> según el conjunto de software seleccionado.  
      Generalmente, se deja el modo <b>default</b>, que corresponde a una versión más liviana y práctica para entornos virtualizados.  
      <br><br>
      Este proceso puede tardar varios minutos, ya que se instalan todos los <b>paquetes del sistema</b> necesarios para el correcto funcionamiento de Rocky Linux.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/c573519f-9a81-4698-9803-ee7bc12c6866"/></p>
    </div>
    <p>
      Si todo sale correctamente, el sistema se <b>reiniciará automáticamente</b> y mostrará la pantalla de inicio de sesión con el <b>usuario creado</b> durante la instalación.  
      A partir de este punto, ya es posible ingresar al entorno de Rocky Linux.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/08ba15d4-6ad7-4c08-810c-7349a8ce1690"/></p>
    </div>
    <p>
      Finalmente, se carga la <b>interfaz principal de Rocky Linux</b>, mostrando una pequeña <b>guía de bienvenida</b> y algunas configuraciones iniciales opcionales.  
      <br><br>
      Desde aquí, también se puede acceder al <b>terminal</b> para comenzar a trabajar con comandos y configuraciones del sistema, confirmando que la instalación se realizó de manera exitosa.
    </p>
  </li>
</ol>

<h2>Instalación MV Kali Linux</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b68413ce-5d28-4bbc-9f17-f26bc814783c"/></p>
    </div>
    <p>
      Al iniciar el arranque del booteable, se muestran varias opciones de instalación.  
      Normalmente se recomienda la primera, ya que es la más cómoda y automática.  
      Sin embargo, por error seleccioné la segunda opción, que realiza la instalación mediante consola.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/0b372c81-e021-4189-9421-b515b4156809"/></p>
    </div>
    <p>
      Luego, aparece una interfaz por consola donde se debe escoger el idioma general, el idioma del teclado y la región.  
      Las selecciones se realizan escribiendo el número correspondiente a cada opción.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/c578defc-becb-41cb-a0fc-5ecc8845d4b9"/></p>
    </div>
    <p>
      Tras elegir el idioma y la región, el instalador pide el <b>nombre del dominio</b>, el <b>nombre completo del usuario</b>, 
      el <b>nombre de usuario</b> como tal y finalmente la <b>contraseña</b> para esa cuenta.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/ce92977e-e279-4c42-8001-c8755e1576c9"/></p>
    </div>
    <p>
      A continuación, se muestran las particiones disponibles, donde debe aparecer la que se asignó en Virtual Manager.  
      Se selecciona y se confirma la instalación en esa unidad cuando el sistema lo pregunte por seguridad.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/2aafe68e-5b4e-46e4-8f44-2d4f5d5dda18"/></p>
    </div>
    <p>
      Una vez seleccionada la partición, el sistema la formatea automáticamente y solicita elegir qué tipo de entorno gráfico instalar.  
      <b>GNOME</b> y <b>KDE Plasma</b> son más pesados, así que se recomienda <b>Xfce</b>, que es más liviano.  
      También se pueden instalar las <b>default tools</b> (herramientas más comunes de Kali).
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b4839564-3a81-48cd-87da-d837c8566d01"/></p>
    </div>
    <p>
      Tras seleccionar las opciones deseadas, el sistema inicia la instalación y, una vez completada, se reinicia para cargar el entorno de Kali Linux.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/f775cc95-2152-4041-9235-c0c70d466f8a"/></p>
    </div>
    <p>
      Finalmente, al iniciar sesión con el usuario y contraseña creados, se muestra la interfaz de inicio con las aplicaciones 
      y herramientas instaladas según la configuración elegida durante la instalación.
    </p>
  </li>
</ol>

<hr>

<div align="center">
  <h2>Instalación de Dependencia Financiera</h2>
</div>

<h2>Instalación Contenedor Garuda (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/f69ed6e7-dee7-4dfb-b30f-32c870c5e50f"/></p>
    </div>
    <p>
      Primero, para crear el contenedor de <b>Garuda</b> (aunque el proceso es similar para los demás contenedores), se empieza creando una carpeta donde se van a colocar todos los proyectos de contenedores.           Luego, dentro de esa carpeta, se crea otra carpeta dedicada a la <b>dockerización</b> de Garuda. Una vez dentro, se procede a crear el archivo <b>Dockerfile</b>. En la siguiente imagen se muestra y explica       su contenido.  
      <br><br>
      Después, se construye la imagen de Docker para poder ejecutarla como contenedor mediante el comando:  
      <code>docker build -t &lt;nombre_imagen&gt; .</code>
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/49b5fed5-b2e9-4edc-8471-24f66b05c4e9"/></p>
    </div>
    <p>
      <ul>
        <li><code>FROM archlinux:latest</code> → Indica que la <b>imagen base</b> será la versión más reciente de Arch Linux, sobre la cual se construirá el contenedor.</li>
        <li><code>RUN pacman -Sy --noconfirm && \</code> → Actualiza la base de datos de paquetes de Arch Linux sin pedir confirmación del usuario (<code>--noconfirm</code>).</li>
        <li><code>pacman -S --noconfirm base-devel git wget curl net-tools openssh && \</code> → Instala los <b>paquetes esenciales</b> para desarrollo y administración del sistema: compiladores, Git,                    herramientas de red y el servidor SSH.</li>
        <li><code>pacman -Scc --noconfirm</code> → Limpia la caché de paquetes de pacman para reducir el tamaño final de la imagen Docker.</li>
        <li><code>RUN ssh-keygen -A</code> → Genera las <b>claves del servidor SSH</b> necesarias para poder iniciar el servicio <code>sshd</code> dentro del contenedor.</li>
        <li><code>RUN echo "root:password123" | chpasswd</code> → Asigna una <b>contraseña al usuario root</b> (en este caso “password123”) para permitir el acceso mediante SSH.</li>
        <li><code>EXPOSE 22</code> → Expone el <b>puerto 22</b>, el estándar utilizado por el protocolo SSH, permitiendo conexiones externas al contenedor.</li>
        <li><code>CMD ["/usr/sbin/sshd", "-D"]</code> → Define el <b>comando por defecto</b> al ejecutar el contenedor: inicia el servicio SSH en modo demonio para mantener el contenedor activo.</li>
      </ul><br>
      Se usa la imagen de <b>Arch Linux</b> porque Garuda no cuenta con una versión oficial en Docker Hub. Arch es su base, por lo tanto, utilizar <code>archlinux:latest</code> permite obtener una imagen               <b>limpia, ligera y actualizada</b>, sobre la cual se pueden instalar los paquetes y configuraciones necesarias para simular el entorno de Garuda.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/baafee4f-3b03-45ae-a924-b29cd9c92306"/></p>
    </div>
    <p>
      Aquí ya se ejecuta el contenedor con <code>docker run</code>, pero de una forma más detallada, ya que se especifican parámetros importantes como el puerto, los recursos del sistema y la configuración de          red para que funcione correctamente junto a otros equipos. A continuación se explica cada parámetro:
      <ul>
      <ul>
        <li><code>-d</code> →  
        Ejecuta el contenedor en <b>modo desapegado (detached)</b>, es decir, en segundo plano, permitiendo seguir usando la terminal.</li>
        <li><code>--name fin-garuda</code> →  
        Asigna el nombre <b>fin-garuda</b> al contenedor.  
        Esto facilita identificarlo o ejecutarlo más tarde sin tener que usar el ID largo del contenedor.</li>
        <li><code>--hostname fin-garuda</code> →  
        Define el <b>nombre de host</b> que el contenedor usará internamente.  
        Este es el nombre que se mostrará dentro del contenedor al ejecutar comandos como <code>hostname</code> o <code>ping</code>.</li>
        <li><code>--network red_empresa</code> →  
        Conecta el contenedor a la red de Docker llamada <b>red_empresa</b>.  
        Esto permite la comunicación con otros contenedores dentro de esa misma red virtual.</li>
        <li><code>--ip 172.20.2.10</code> →  
        Asigna una <b>dirección IP fija</b> dentro de la red de Docker especificada.  
        De esta manera, el contenedor siempre tendrá la misma IP y será más fácil ubicarlo o conectarlo con otros servicios.</li>
        <li><code>-m 1g</code> →  
        Limita la cantidad máxima de <b>memoria RAM</b> que puede usar el contenedor a <b>1 GB</b>.</li>
        <li><code>--cpus="1"</code> →  
        Restringe al contenedor para que use solo <b>1 núcleo de CPU</b> del sistema host.</li>
        <li><code>-p 2202:22</code> →  
        Mapea el puerto <b>22</b> del contenedor (donde corre el servicio SSH) al puerto <b>2202</b> del equipo host.  
        Así puedes conectarte por SSH al contenedor usando <code>ssh -p 2202 usuario@localhost</code>.</li>
        <li><code>financiera-garuda</code> →  
        Es el <b>nombre de la imagen</b> que se usa para crear el contenedor.  
        En este caso, es una imagen personalizada basada en <b>Garuda Linux</b>.</li>
      </ul>
    </p>
  </li>
</ol>

<h2>Instalación Contenedor Ubuntu</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b26516e3-1b6d-42f0-a1d9-5fb0a275a5f2"/></p>
    </div>
    <p>
      Para crear este contenedor, primero se genera la carpeta donde se va a <b>dockerizar</b> este sistema operativo, dentro de la misma carpeta <b>“contenedores”</b>, ya que ahí se colocarán todos los                contenedores que se vayan a crear.  
      Luego, se realiza el <b>Dockerfile</b>, que será el encargado de configurar toda la construcción de la imagen.  
      Finalmente, se construye la imagen del sistema operativo con el comando:  
      <code>docker build -t &lt;nombre_imagen&gt; .</code>  
      <br><br>
      Después de eso, se corre el contenedor con las especificaciones que se le asignen.  
      A este se le dieron menos recursos ya que no actúa como nodo principal ni como administrador de la subred.  
      En la imagen se puede ver el contenedor corriendo con las configuraciones dadas.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/cb4fd365-7325-4579-a923-f8bd2bb81b11"/></p>
    </div>
    <p>
      En esta parte se muestra el <b>Dockerfile</b> del sistema operativo.  
      Aquí se evidencia que no fue necesario realizar el mismo proceso que con el anterior sistema, ya que Ubuntu sí cuenta con una imagen oficial en <b>Docker Hub</b>.  
      Por eso se puede usar directamente sin recurrir al sistema base (Debian).  
      <br><br>
      Aunque tiene algunos comandos diferentes, su función es muy similar. A continuación, se explica cada uno:
      <ul>
        <li><code>RUN apt-get update</code> actualiza la lista de paquetes disponibles.</li>
        <li><code>apt-get install</code> instala herramientas esenciales como <code>net-tools</code> (para ifconfig), <code>iputils-ping</code> (para ping), <code>openssh-server</code> (para habilitar SSH), <code>curl</code> y <code>wget</code> (para descargas).</li>
        <li><code>apt-get clean</code> elimina los archivos temporales de instalación, reduciendo el tamaño final de la imagen.</li>
        <li><code>RUN mkdir /var/run/sshd</code> → Crea el directorio donde el servicio SSH almacenará sus archivos de ejecución (<code>sshd.pid</code>).</li>
        <li><code>RUN sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config</code> → Modifica el archivo de configuración del servicio SSH para <b>permitir el inicio de sesión como root</b>.</li>
      </ul>
    </p>
  </li>
</ol>

<h2>Instalación Contenedor Alpine</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/acdc7d1c-abb8-479c-b6fc-0adc8b782b91"/></p>
    </div>
    <p>
      Aquí se sigue el mismo proceso de crear una carpeta para la <b>dockerización</b> del sistema operativo dentro de la carpeta <b>“contenedores”</b>, donde se están almacenando todos los contenedores.  
      Luego se crea el <b>Dockerfile</b> correspondiente para construir la imagen, y finalmente se genera con el comando:  
      <code>docker build -t &lt;nombre_imagen&gt; .</code>
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/ff019db1-a72a-4d70-9f50-d2c60457c351"/></p>
    </div>
    <p>
      Este es el <b>Dockerfile</b> de Alpine. Aunque su estructura es similar, tiene algunos detalles diferentes que permiten que funcione correctamente con su propio gestor de paquetes:
      <ul>
        <li><code>RUN apk add --no-cache bash openssh net-tools curl wget</code> → Instala paquetes usando el <b>gestor de paquetes de Alpine (apk)</b>:
          <ul>
            <li><code>--no-cache</code> evita almacenar caché para mantener la imagen liviana.</li>
            <li><code>bash</code> instala la shell Bash (ya que Alpine usa <code>ash</code> por defecto).</li>
            <li><code>openssh</code> instala el servidor SSH.</li>
            <li><code>net-tools</code> agrega utilidades de red como <code>ifconfig</code>.</li>
            <li><code>curl</code> y <code>wget</code> permiten realizar descargas desde la terminal.</li>
          </ul>
        </li>
      </ul>
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/1c8b05b3-d718-4e43-b0a6-ae0dfa0b898a"/></p>
    </div>
    <p>
      Finalmente, se corre el contenedor con las especificaciones solicitadas.  
      Los recursos asignados son los mismos que los del contenedor de Ubuntu, ya que este pertenece a la misma rama dentro de la subred <b>Financiera</b>.
    </p>
  </li>
</ol>

<hr>

<div align="center">
  <h2>Instalación de Dependencia Comercial y Ventas</h2>
</div>

<h2>Instalación Contenedor Fedora (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/582fb4b8-dc77-49b4-bc88-45009d46f773"/></p>
    </div>
    <p>
      El proceso es el mismo que en los anteriores contenedores, a pesar de que se utilice otra distribución, ya que todos se instalan dentro de la carpeta <b>"contenedores"</b>.
      Luego, se crea el archivo <b>Dockerfile</b> correspondiente para construir la imagen, y finalmente se genera con el comando: <code>docker build -t &lt;nombre_imagen&gt; .</code>.
      <br><br>
      Después de eso, se ejecuta el contenedor con las especificaciones asignadas.
      A este se le otorgaron más recursos, ya que actúa como el <b>nodo principal (admin)</b> de la subred.
      En la imagen se puede observar el contenedor corriendo con las configuraciones establecidas.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/2dd191c4-1839-4e2d-9975-4b2828beecff"/></p>
    </div>
    <p>
      Este dockerfile es muy similar, pero toca configurar el SO a su manera, que seria asi:
      <ul>
        <li><code>dnf update -y</code> actualiza todos los paquetes del sistema sin pedir confirmación (<code>-y</code>).</li>
        <li><code>dnf install -y</code> instala los paquetes necesarios para el contenedor</li>
        <li><code>dnf clean all</code> elimina los archivos temporales y la caché del gestor para <b>mantener la imagen ligera</b>.</li>
    </p>
  </li>
</ol>

<h2>Instalación Contenedor Debian</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7981c12c-468c-4100-9dee-3bbedf60df6b"/></p>
    </div>
    <p>
      El proceso es el mismo que los anteriores contenedores, ya que se van a instalar en la misma carpeta "contenedores".
      Después se crea el <b>Dockerfile</b> correspondiente para construir la imagen, y finalmente se genera con el comando:  
      <code>docker build -t &lt;nombre_imagen&gt; .</code>.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/474c6321-a2d8-45d8-a940-bdfb75569bdd"/></p>
    </div>
    <p>
      El <b>Dockerfile</b> de este sistema operativo es prácticamente el mismo que el de Ubuntu, ya que, como se mencionó antes, <b>Ubuntu está basado en Debian</b>.
      Por lo tanto, comparten muchos comandos y configuraciones, lo que hace que el proceso de creación e instalación de la imagen sea casi idéntico.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b30c3cfe-8963-4d7c-9b2e-8e2756ad40ca"/></p>
    </div>
    <p>
      En esta imagen se puede evidenciar que <b>todos los contenedores están conectados</b> a la red llamada <b>"red_empresa"</b>.
      También se muestran los puertos asignados a cada contenedor, los cuales son distintos entre sí.
      Sin embargo, la comunicación entre ellos se realiza a través del <b>puerto 22 (SSH)</b>, que es el encargado de permitir la conexión segura entre los contenedores.
    </p>
  </li>
</ol>

<h2>Instalación MV Alma Linux</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7910c900-26fd-4df4-92a1-5b345d30b1a8"/></p>
    </div>
    <p>
      Al descargar la imagen <b>(.iso)</b> desde la página oficial de <b>Alma Linux</b>, se ingresa a <b>QEMU</b> para crear la máquina virtual.  
      En este proceso se deben realizar pasos como <b>seleccionar la ubicación de la imagen (.iso)</b>, asignar una <b>partición del disco</b>, definir la cantidad de <b>memoria RAM</b> y los <b>núcleos de CPU</b> del PC.  
      <br><br>
      Luego de configurar todo, aparecerá el mensaje inicial donde se puede <b>instalar</b> o <b>testear</b> el sistema para comprobar si el hardware es compatible y todo funciona correctamente.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/bcdca4fc-17c0-45aa-aa98-d3c34cd54daf"/></p>
    </div>
    <p>
      Luego aparece la opción para escoger el <b>idioma del sistema</b> y el <b>idioma del teclado</b>, permitiendo continuar con la instalación de manera clara y comprensible.  
      Estas configuraciones iniciales aseguran que el entorno sea más accesible durante todo el proceso.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/eaee87e0-2dde-4192-b41d-1395e0cd1a1e"/></p>
    </div>
    <p>
      En esta parte se muestra el <b>disco o partición</b> que fue asignado al sistema operativo desde QEMU.  
      De esta manera, se puede seleccionar directamente la unidad de instalación sin confusiones, garantizando que Alma Linux se instale en el espacio correcto.
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/a20b56c3-a4a7-45d4-b26e-7b7569c1d68f"/></p>
    </div>
    <p>
      En este paso se crea el <b>usuario principal</b> que podrá ingresar al sistema.  
      Es necesario ingresar el <b>nombre completo</b>, el <b>nombre de usuario</b> y establecer una <b>contraseña segura</b>.  
      <br><br>
      Esto permite personalizar el entorno de trabajo y garantizar el acceso protegido al sistema operativo.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7ec3513a-a4ba-43b8-85ab-33359b7c1265"/></p>
    </div>
    <p>
      Una vez configurado todo, se procede a <b>instalar el sistema</b>.  
      Este proceso puede tardar varios minutos, ya que se instalan todos los <b>paquetes y dependencias</b> necesarias para el funcionamiento completo de Alma Linux.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/de796da9-8f2d-422d-bf6f-d5bcf6c76092"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/4eba450f-bb75-473d-9645-61954b591b01"/></p>
    </div>
    <p>
      Finalmente, después de <b>reiniciar el sistema</b>, aparecerá el <b>usuario creado</b> para iniciar sesión.  
      <br><br>
      Una vez dentro, se mostrará la <b>pantalla de bienvenida</b> de Alma Linux, junto con un pequeño <b>tour inicial</b> para familiarizarse con el entorno del sistema.  
      Desde este punto, el sistema operativo queda listo para usarse de forma completa.
    </p>
  </li>
</ol>

<hr>

<div align="center">
  <p><em>Conexión de la Red</em></p>
</div>

<hr>

<div align="center">
  <h2>Conexión Red, Subred Dependencia Financiera, Subred Comercial y Ventas</h2>
</div>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/4d1ca026-2552-423f-9bf7-f5b50869ac8b"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/13edfd85-5b19-4092-a64d-c41f6e2300e2"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7f17505b-7b25-4794-a267-203c7b2eef6f"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/f4831df6-f715-499c-8ff3-18509bb8bc35"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/5812d3db-59d4-4057-b4b9-883e33a8361a"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/5227204c-a753-4bd5-9cf2-d88719879220"/></p>
    </div>
    <p>
      
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/725ff284-f2d2-4a50-8813-68cc3ca7571d"/></p>
    </div>
    <p>
      
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/2367addc-c9f4-4fb6-89fd-ed0a75548e55"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/4b883c08-6db9-4b4a-aa3b-76f5ff23548d"/></p>
    </div>
    <p>
      
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/28871441-35cc-436b-943e-1a6ed88eaca7"/></p>
    </div>
    <p>
      
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/94e477b0-6fa7-4c4b-ab04-00ef22c501b3"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/7e2b51a0-4a4f-4c0d-b53e-e99916cddd15"/></p>
    </div>
    <p>
      
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/23ae1ad6-3d07-40ff-bd13-c5955f586863"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<div align="center">
  <h2>Pruebe de Conexión Red, Subred Dependencia Financiera, Subred Comercial y Ventas</h2>
</div>

<h2>Prueba Ubuntu (Host)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/01ea665e-362f-45be-9edd-b4306da5b697"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/d24181d7-077a-434e-a1b9-e1708c148389"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<h2>Prueba Debian (Admin)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/39e49951-af53-4ff1-b786-655d4a1f9100"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/4e04d1ca-e2c8-4fe1-8618-e8d1c0268239"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<h2>Prueba Garuda (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d48c66-c8a2-4747-b2c9-5872ed17b8de"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e342e0b2-1703-4e25-ab2e-ede23f16f4bc"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<h2>Prueba Fedora (Nodo)</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/4475c1b5-cbb2-4d04-9682-37231c8fdf7c"/></p>
    </div>
    <p>
      
    </p>
  </li>
  
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/38e6a1ae-ef1f-42c1-9f6d-3db30ad2826d"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>
