# Aplicaciones Desarrollo
## Versión 1.3.0.0
## Script de Inno Setup. Paquete de Aplicaciones de Desarrollo.

### Software.

* **Arduino IDE 1.6.7 x32 JVM:** The open-source Arduino Software (IDE) makes it easy to write code and upload it to the board.
* **Eclipse Java Mars 2 x64:** The essential tools for any Java developer, including a Java IDE, a Git client, XML Editor, Mylyn, Maven integration and WindowBuilder.
* **IntelliJ IDEA Community Edition 15.0.4 x64:** Capable and Ergonomic Java IDE.
* **JDeveloper 12c Java SE 12.2.1.0.0 x64:** Oracle JDeveloper is a free integrated development environment that simplifies the development of Java-based applications
* **NetBeans IDE 8.1 x64:** NetBeans IDE is FREE, Open source. Quickly and easily develop desktop, mobile and web applications with Java, JavaScript, HTML5, PHP, C/C++ and more.
* **SQL Developer 4.1.3 x64:** Oracle SQL Developer is a free integrated development environment that simplifies the development and management of Oracle Database in both traditional and Cloud deployments.
* **Android Studio 1.5.1 x64:** The official IDE for Android development.
* **Xampp 7.0.4-0 VC14 x32:** Completely free, easy to install Apache distribution containing MariaDB, PHP, and Perl.

### Common Files.

* **ApiGen 4.1:** Smart and Readable Documentation for your PHP project.
* **phpDocumentor 2:** Tool that makes it possible to generate documentation directly from your PHP source code.
* **Apache Tomcat 9 x64:** Open source software implementation of the Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket technologies.
* **GlassFish 4.1.1:** Open-source application server project started by Sun Microsystems for the Java EE platform and now sponsored by Oracle Corporation.
* **Java SE Development Kit:** jdk1.8.0_74 x64
* **Install icon:** [jozef89](http://www.iconarchive.com/show/services-flat-icons-by-jozef89/responsive-web-icon.html)

### Notes

#### Modificaciones en Android Studio:

Misma configuracion que IntelliJ Idea.
Creamos la carpeta `var` donde el ide almacena la configuracion, plugins y logs.
Agregamos una variable de entorno para que cargue el jdk en `commonfiles\jdk`.

`SET IDEA_JDK_64={APP-DIR}\commonfiles\jdk`

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

#### Modificaciones en Arduino Studio:

Creamos la carpeta `portable` y por defeto el ide almacena en ella la configuracion.

#### Modificaciones en Eclipse Mars 2:

Agregamos la ruta del jdk de `commonfiles\jdk` en el archivo de configuracion de eclipse.
Editamos el archivo **eclipse.ini**.

```
-vm
.\..\commonfiles\jdk\bin
```

#### Modificaciones en IntelliJ Idea:

Misma configuracion que Android Studio.
Creamos la carpeta `var` donde el ide almacena la configuracion, plugins y logs.
Agregamos una variable de entorno para que cargue el jdk en `commonfiles\jdk`.

`SET IDEA_JDK_64={APP-DIR}\commonfiles\jdk`

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

#### Modificaciones en JDeveloper:

Agregamos la ruta del jdk en `commonfiles\jdk` en el archivo de configuracion de jDeveloper.

Editamos el archivo **jdev.conf**.

```
#SetJavaHome @JAVA_HOME@
SetJavaHome .\..\..\..\commonfiles\jdk
```

#### Modificaciones en SQL Developer:

Agregamos la ruta del jdk en `commonfiles\jdk` en el archivo de configuracion de SQL Developer.

Editamos el archivo **sqldeveloper.conf**.

```
#SetJavaHome ../../jdk
#Agregamos la ruta del jdk
SetJavaHome .\..\..\..\commonfiles\jdk
```

#### Modificaciones en NetBeans:

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

AppDes.
