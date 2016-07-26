# Paquete de Aplicaciones de Desarrollo (AppDev).
## Versión 2.0.0.0
## Script de Inno Setup. Paquete de Aplicaciones de Desarrollo.

### Software.

* **Arduino IDE 1.6.9 x32 JVM:** The open-source Arduino Software (IDE) makes it easy to write code and upload it to the board.
* **Eclipse Java Neon x64:** The essential tools for any Java developer, including a Java IDE, a Git client, XML Editor, Mylyn, Maven integration and WindowBuilder.
* **NetBeans IDE 8.1 x64:** NetBeans IDE is FREE, Open source. Quickly and easily develop desktop, mobile and web applications with Java, JavaScript, HTML5, PHP, C/C++ and more.
* **Android Studio 2.1.2 x64:** The official IDE for Android development.
* **Xampp 7.0.8 VC14 x32:** Completely free, easy to install Apache distribution containing MariaDB, PHP, and Perl.

### Common Files.

* **ApiGen 4.1:** Smart and Readable Documentation for your PHP project.
* **phpDocumentor 2:** Tool that makes it possible to generate documentation directly from your PHP source code.
* **Apache Tomcat 8.5.4 x64:** Open source software implementation of the Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket technologies.
* **GlassFish 4.1.1:** Open-source application server project started by Sun Microsystems for the Java EE platform and now sponsored by Oracle Corporation.
* **Java SE Development Kit:** Java Jdk-8u102 x64
* **Android SDK:** Android Sdk r24.4.1 x64
* **Install icon:** [jozef89](http://www.iconarchive.com/show/services-flat-icons-by-jozef89/responsive-web-icon.html)

### Notes


#### Modificaciones en el Registro de Windows.

Agregamos unas entradas en la variable de entorno **Path**.

`{olddata};{APP-DIR}\commonfiles\jdk\bin`

`{olddata};{APP-DIR}\commonfiles\sdk\tools`

`{olddata};{APP-DIR}\commonfiles\sdk\platform-tools`

Agregamos una variable de entorno para que cargue el JDK en `commonfiles\jdk`.

`SET JAVA_HOME={APP-DIR}\commonfiles\jdk`

Agregamos una variable de entorno para que Android Studio cargue el JDK en `commonfiles\jdk`.

`SET IDEA_JDK_64={APP-DIR}\commonfiles\jdk`

Agregamos una variable de entorno para que Android Studio cargue el SDK en `commonfiles\sdk`.

`SET ANDROID_HOME={APP-DIR}\commonfiles\sdk`


#### Modificaciones en Android Studio 2.1.2.

Creamos la carpeta `var` donde el ide almacena la configuracion, plugins y logs.

Agregamos las rutas en **idea.properties**.

```
#---------------------------------------------------------------------
# Customize path to IDE config folder.
#---------------------------------------------------------------------
idea.config.path=${idea.home.path}/var/config

#---------------------------------------------------------------------
# Customize path to IDE system folder.
#---------------------------------------------------------------------
idea.system.path=${idea.home.path}/var/system

#---------------------------------------------------------------------
# Customize path to user installed plugins folder.
#---------------------------------------------------------------------
idea.plugins.path=${idea.home.path}/var/config/plugins

#---------------------------------------------------------------------
# Customize path to IDE logs folder.
#---------------------------------------------------------------------
idea.log.path=${idea.home.path}/var/system/log
```


#### Modificaciones en Arduino Studio 1.6.9.

Creamos la carpeta `portable` y por defeto el ide almacena en ella la configuracion.

El Ide Arduido dispone de su propia version de jre.


#### Modificaciones en Eclipse Neon.

Agregamos la ruta del jdk de `commonfiles\jdk` en el archivo de configuracion de eclipse.
Editamos el archivo **eclipse.ini**.

```
-vm
.\..\commonfiles\jdk\bin
```


#### Modificaciones en NetBeans 8.1.

Agregamos la ruta del jdk en `commonfiles\jdk` en **netbenas.conf**.

`netbeans_jdkhome="../../commonfiles/jdk"`

### License.

* All software is free, open source or evaluated for free.
* Rights are owned by their respective developers.
* Aplicaciones Desarrollo it is a package to facilitate installation of these programs.
* It is free and nonprofit.

### Download.

Download a full copy of Aplicaciones Desarrollo: [AppDes](http://www.4shared.com/file/Yids9mEZce/AppDesIns.html)

All applications are free and are distributed also free.

AppDev.
