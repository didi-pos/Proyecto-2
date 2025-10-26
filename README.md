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
      Al descargar la imagen (.iso) desde la página oficial de Rocky Linux, uno ingresa a qemu para descargar la máquina virtual, se hacen los procesos como colocar al ubicación de la imagen (.iso), también de         asignarle una partición del disco, asignarle memoria RAM y núcleos de la CPU del pc. Luego de ese proceso ahora sí debe aparecer este mensaje donde pide instalar o testear el pc para saber si corre el            sistema operativo en el pc
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/7c3b7d74-288d-475b-892a-7dcf704d3031"/></p>
    </div>
    <p>
      Aquí se muestra la configuración de la instalación de Rocky Linux.  
      La imagen <b>(.iso)</b> ya reconoce automáticamente el idioma, el teclado y otras configuraciones por defecto.  
      Sin embargo, es necesario elegir el disco donde se almacenará el sistema operativo (el que se asignó desde Virtual Manager).  
      Además, se debe decidir si se habilita la cuenta <b>root</b> y crear el usuario principal con su respectiva contraseña.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/518480eb-3598-49f3-b3a2-b18b1095d38e"/></p>
    </div>
    <p>
      Luego comienza la instalación del sistema operativo según el software seleccionado.  
      Generalmente se deja el modo <b>default</b>, que es una versión más liviana y práctica.
      Este proceso demora un buen tiempo ya que serían todos los paquetes del sistema
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/c573519f-9a81-4698-9803-ee7bc12c6866"/></p>
    </div>
    <p>
      Si todo sale bien, el sistema se reiniciará automáticamente y mostrará el usuario que se creó durante la instalación.
    </p>
  </li>

  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/08ba15d4-6ad7-4c08-810c-7349a8ce1690"/></p>
    </div>
    <p>
      Finalmente, aparece la interfaz principal de Rocky Linux, ofreciendo un pequeño tutorial opcional y la bienvenida en el terminal.
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
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/49b5fed5-b2e9-4edc-8471-24f66b05c4e9"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/baafee4f-3b03-45ae-a924-b29cd9c92306"/></p>
    </div>
    <p>
      
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
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/cb4fd365-7325-4579-a923-f8bd2bb81b11"/></p>
    </div>
    <p>
      
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
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/ff019db1-a72a-4d70-9f50-d2c60457c351"/></p>
    </div>
    <p>
      
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
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<h2>Instalación Contenedor Debian</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>

<h2>Instalación MV Alma Linux</h2>

<ol>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/e1d671ea-49cd-44ac-b2de-2c13c34058c7"/></p>
    </div>
    <p>
      
    </p>
  </li>
</ol>
