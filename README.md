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
      El proceso arranca con la configuración inicial de la instalación. Es fundamental elegir primero el <b>idioma del sistema</b> y la <b>distribución del teclado</b>. Normalmente, estos pasos se hacen en una        interfaz por consola muy sencilla, asegurando que el instalador entienda nuestras preferencias regionales para el siguiente paso.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/cf4476f8-daa8-43de-b89f-d5a23311b4d3"/></p>
    </div>
    <p>
      Tras establecer el idioma, el sistema carga los componente adicionales de instalación, este ayuda a seguir con la descarga y además son componentes que se van a evidenciar después de la instalación               necesarios del sistema operativo.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/1b456f08-81e8-450c-b036-5d3299a496ca"/></p>
    </div
    <p>
      Luego nos pide el nombre dela maquina, este no es ni el nombre de superusuario ni el de usuario, este simplemente para saber como se va a llamar la maquina o pc.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/bf0ce814-2666-4440-b235-4b7f39defda5"/></p>
    </div>
    <p>
      A partir de este punto, el instalador pide datos críticos para la seguridad del sistema, primero pide el nombre del dominioo que va a tener el sistema operativo, luego se asigna la <b>contraseña del              usuario Root</b> (la cuenta con máximos privilegios), luego el <b>nombre completo del nuevo usuario</b>, el <b>nombre de usuario</b> (el identificador corto) y, finalmente, la <b>contraseña para esa cuenta       personal</b>. Es decir, el sistema nos obliga a configurar la cuenta de superusuario y la cuenta de uso diario en secuencia.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/b19fd2c7-f537-4b25-b0eb-6633e72876df"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/d1006cb0-138b-45c1-b75a-4256c634f236"/></p>
    </div>
    </div>
    <p>
      Luego llegamos a la parte de particionado. En este punto, <b>Debian</b> nos da varias opciones para usar el disco que asignamos desde <b>Virtual Manager</b>. Yo usé la opción de <b>"Guiado - Utilizar todo        el disco"</b>, que es la forma más fácil y automática de particionar, ya que el instalador lo hace por nosotros.<br>
      Al seleccionar esta opción, el sistema nos pide confirmar la unidad (la que asignamos en la creación de la VM) y la confirmación final de que estamos de acuerdo con <b>escribir los cambios en el disco</b>.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/475708ce-a467-4ee2-a7a8-fab277d964b4"/></p>
    </div>
    <p>
      Después se inicia la instalacion base del sistema, el cuel es practicamente lo que hace que el SO se ejecute, esto quiere decir que no es la instalaciones adicionales, como lo es el entorno grafico o las aplicaciones del sistema y mucho menos las aplicaciones recomendadas, este simplemente es el sistema principal y el más básico.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/48c5f138-ee71-4495-a7e9-4c503f3abb05"/></p>
    </div>
    <p>
      Una vez confirmado el particionado, el instalador solicita elegir los <b>paquetes de software</b> que queremos incluir. Esta es la parte donde decidimos si instalamos el entorno gráfico (como <b>GNOME</b>        o <b>Xfce</b>) y otros servicios (como aplicaciones recomendadas).<br>
      Por comodidad y para hacer que el sistema sea mucho menos pesado que con la configuracion default, yo elegi Xfce que es el entorno grafico mas liviano, pero bastante comodo a diferencia de tener el SO en         terminal simplemente, y tambíen ecogi el servicio SSH, ya que se necesita para el proyecto lo cual nos va hacer comunicar con los demás entornos, y utilidades estandar del sistema por si es de utilidad.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/367a2976-9e63-4821-a36f-c0517b3a406c"/></p>
    </div>
    <p>
      Aquí el sistema nos pregunta si queremos <b>instalar el cargador de arranque GRUB</b> en el registro principal del disco. Esto es             esencial para que la máquina virtual pueda iniciar el sistema         operativo correctamente, así que hay que decirle que <b>sí</b> y seleccionar el disco que usamos para la instalación.
    </p>
  </li>
  <li><br>
    <div align="center">
      <p><img width="850" src="https://github.com/user-attachments/assets/5b9f3657-72ca-480d-83b0-f3fbeb9eeb42"/></p>
      <p><img width="850" src="https://github.com/user-attachments/assets/ad6747e5-403d-49e1-96e1-1d8cfe005b70"/></p>
    </div>
    <p>
      Si todo ha salido bien, la VM se reinicia y nos pide ingresar las <b>credenciales del usuario</b> que creamos previamente. Una vez dentro, se muestra la interfaz principal del escritorio de <b>Debian</b>,        confirmando que la instalación fue exitosa y ya podemos empezar a trabajar con la máquina virtual de manera normal.
    </p>
  </li>
</ol>
