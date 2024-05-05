# Kioann Valencia Santibañez
## 191064129
### Cordero Ocampo Martin
#### Ensayo de un Modelo Vista Controlador
##### Instituto Tecnológico De Tláhuac
###### Ingeniería En Sistemas Computacionales
###### Grupo: 8S2 Programación web PHP/MVC
###### 21 de marzo 2024

## Tabla de contenido
- [RESUMEN](#resumen)
- [INTRODUCCIÓN](#introducción)
  - [Contexto y Justificación](#contexto-y-justificación)
  - [Objetivos del Proyecto](#objetivos-del-proyecto)
  - [Metodología de Desarrollo](#metodología-de-desarrollo)
  - [Alcance del Proyecto](#alcance-del-proyecto)
- [CUERPO/ DESARROLLO](#cuerpo--desarrollo)
  - [ORDEN MVC](#orden-mvc)
  - [INDEX](#index)
  - [MODELO](#modelo)
  - [VISTA](#vista)
  - [CONTROLADOR](#controlador)
  - [ASSETS](#assets)
  - [CONFIG](#config)
  - [DIAGRAMAS](#diagramas)
- [CONCLUSIONES](#conclusiones)
- [BIBLIOGRAFÍA](#bibliografía)

## RESUMEN
<p>El Modelo-Vista-Controlador (MVC) es un patrón arquitectónico ampliamente utilizado en el desarrollo de software, que busca estructurar las aplicaciones de una manera clara y organizada. Este enfoque divide una aplicación en tres componentes principales: el modelo, la vista y el controlador. Cada uno de estos componentes tiene un rol específico en el funcionamiento y la presentación de la aplicación, lo que permite una mejor organización del código y una mayor facilidad para el mantenimiento y la escalabilidad.</p>

El modelo representa la lógica de negocio y los datos subyacentes de la aplicación. Es responsable de la manipulación y gestión de los datos, así como de la implementación de la lógica de negocio. Por ejemplo, en una aplicación de gestión de usuarios, el modelo podría incluir clases y métodos para crear, actualizar, eliminar y recuperar usuarios de una base de datos.

La vista es la interfaz de usuario que presenta la información al usuario final. Es responsable de mostrar los datos proporcionados por el modelo de una manera comprensible y atractiva. Por ejemplo, en una aplicación de redes sociales, la vista podría ser la página de perfil de un usuario, que muestra su información personal, sus publicaciones y sus amigos de una manera visualmente atractiva.

El controlador actúa como intermediario entre el modelo y la vista. Es responsable de recibir las solicitudes del usuario desde la vista, procesarlas utilizando la lógica de negocio apropiada en el modelo y actualizar la vista en consecuencia. Por ejemplo, en una aplicación de comercio electrónico, el controlador podría manejar las solicitudes de agregar productos al carrito de compras, calcular el total de la compra y actualizar la vista del carrito de compras con los nuevos datos.

La separación de responsabilidades entre el modelo, la vista y el controlador proporciona una serie de beneficios significativos en el desarrollo de software. En primer lugar, facilita la modularidad y la reutilización del código, ya que cada componente puede ser desarrollado y probado de forma independiente. Esto permite a los desarrolladores trabajar en diferentes partes de la aplicación simultáneamente, lo que acelera el proceso de desarrollo.

Además, la separación clara de responsabilidades facilita las pruebas unitarias y de integración, ya que cada componente puede ser probado por separado para garantizar su correcto funcionamiento. Esto mejora la calidad y la confiabilidad del software desarrollado, ya que los errores pueden ser identificados y corregidos de manera más eficiente.

Otro beneficio importante del patrón MVC es su capacidad para adaptarse a los cambios en los requisitos del negocio y escalar según sea necesario. La modularidad y la separación de responsabilidades permiten a los desarrolladores incorporar nuevas funcionalidades y expandir la aplicación sin afectar su integridad.

Aquí un código del INDEX que es el que tiene la acción principal:
$accionTmp(); ` `} ?>


## INTRODUCCIÓN
### Contexto y Justificación

Los establecimientos minoristas enfrentan una serie de desafíos operativos y de gestión, que van desde el seguimiento preciso del inventario hasta la gestión eficiente de las transacciones de ventas y la fidelización de los clientes. Con el crecimiento del comercio electrónico y la demanda de una experiencia de compra más fluida y personalizada, es imperativo que los minoristas adopten soluciones tecnológicas avanzadas que les permitan competir en un mercado en constante evolución.

El sistema de punto de venta basado en MVC surge como respuesta a estas necesidades, ofreciendo una plataforma integral y escalable que abarca todas las facetas de la operación minorista. Desde la gestión de inventario hasta el procesamiento de pagos y la generación de informes analíticos, el sistema está diseñado para mejorar la eficiencia operativa, reducir los errores y optimizar la experiencia del cliente.

## INSTALACIÓN
- Paso 1:
  Ejecutar Xampp y activar Apache y MySQL
  
  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/5bdc46e7-bae6-41a2-8b36-c97a64dd9038)2:

- Paso 2:
  Extraer la carpeta del proyecto.
  
  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/72c08bc9-6f35-4fe8-8584-279c0272cf1b)
  
  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/35a1a315-1fff-4b2c-83eb-101941e68d4b)


- Paso 3:
  copiar la carpeta extraida "Tienda-suplementos-MVC-PHP-main" en la carpeta de xampp ( guiate por la siguiente direccion que se muestra en la imagen)

  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/5953bef6-996f-4bcc-9493-1370429de015)

- Paso 4: abre tu PHPMyadmind con la siguiente direccion  en tu navegador http://localhost/phpmyadmin/index.php?route=/server/databases, crea una nueva vase de datos con el nombre de             "tienda" junto con la configuracion que se muestra en la imagen.
  
  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/051ce94a-d633-4063-b099-2ab4a9f12b42)

- Paso 5: una vez creada la base de datos importa la base de datos en el apartado de importar, selecciona el archivo "sto" que esta en la carpeta del proyecto anteriormente copiada en la carpeta htdocs de xampp

  ![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/4344e7e6-3f1e-4f99-a09a-5cdf19c9eb54)

- Paso 6: 
  en tu navegador copia la siguiente direccion http://localhost/Tienda-suplementos-MVC-PHP-main/
  
  
### Objetivos del Proyecto

Desarrollar un sistema de punto de venta robusto y fácil de usar, que permita a los minoristas gestionar de manera eficiente todas las actividades relacionadas con la venta y el control de inventario. Entre los objetivos específicos se incluyen:

- Diseñar una interfaz de usuario intuitiva y amigable que facilite la navegación y el uso del sistema por parte de los usuarios finales.
- Implementar funcionalidades avanzadas de gestión de inventario, incluyendo seguimiento de productos, ajustes de inventario y alertas de stock bajo.
- Integrar un módulo de procesamiento de pagos seguro y confiable, que admita múltiples métodos de pago y garantice transacciones rápidas y seguras.
- Desarrollar un sistema de generación de informes analíticos y estadísticas de ventas, que proporcione a los administradores una visión completa y detallada del rendimiento del negocio.
- Garantizar la escalabilidad y la flexibilidad del sistema, permitiendo su adaptación a las necesidades cambiantes del negocio y el crecimiento futuro de la empresa.

### Metodología de Desarrollo

El proyecto seguirá una metodología ágil de desarrollo de software, que permitirá una entrega iterativa y continua de funcionalidades y mejoras. Se establecerán reuniones regulares con los stakeholders para recopilar retroalimentación y realizar ajustes según sea necesario. Además, se llevará a cabo un riguroso proceso de pruebas y control de calidad para garantizar la fiabilidad y el rendimiento del sistema.

### Alcance del Proyecto

El alcance del proyecto incluirá el diseño, desarrollo e implementación del sistema de punto de venta, así como la capacitación del personal en su uso y mantenimiento. Se proporcionará soporte técnico continuo y se realizarán actualizaciones periódicas para garantizar la funcionalidad y la seguridad del sistema a lo largo del tiempo.

## CUERPO/ DESARROLLO

### ORDEN MVC
![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/ca503574-7ef4-418f-9572-e6fa1a4c7669)

### INDEX
En nuestro index va a ser el principal, ya que este manda a traer a los controladores y a los demás archivos:
![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/887932cd-7783-4822-9fe8-a9773fe3d5ea)

En esta parte veremos el código en donde manda a traer todos los archivos:
![image](https://github.com/Kioannvalencia/Tienda-suplementos-MVC-PHP/assets/167829988/579c429d-9c4b-44a2-8b70-da661003a2f1)

## MODELO
El modelo representa la lógica de negocio y los datos subyacentes de la aplicación.

## VISTA
Es la interfaz de usuario que presenta la información al usuario final, ya que en esta carpeta se muestran todos los archivos que son las vistas:

## CONTROLADOR
Actúa como intermediario entre el modelo y la vista. Es responsable de recibir las solicitudes del usuario desde la vista, procesarlas utilizando la lógica de negocio apropiada en el modelo y actualizar la vista en consecuencia, como se puede ver a continuación:

## ASSETS
En los assets encontraremos los JS y los estilos CSS que son los que le van a a dar la forma y funciones a nuestro sistema.
- JS
- CSS

## CONFIG
En esta carpeta tenemos nuestra conexión a nuestra base de datos

## DIAGRAMAS

## CONCLUSIONES
En resumen, el proyecto de punto de venta implementado con el patrón de arquitectura Modelo-Vista-Controlador (MVC) resultó ser una elección acertada. La división clara entre la lógica de negocio, la presentación y el control del flujo de la aplicación facilitó su desarrollo, mantenimiento y escalabilidad.

## BIBLIOGRAFÍA
- Victor. (2019, 3 abril). [MVC (Modelo Vista Controlador) en PHP nativo](https://victorroblesweb.es/2013/11/18/tutorial-mvc-en-php-nativo/). Victor Robles.
- Rincón, J. G. (s. f.). [Jairo García Rincón](https://www.jairogarciarincon.com/clase/programacion-orientada-a-objetos-en-php/patron-mvc).
- Redactor. (2022, 10 febrero). [Modelo vista controlador (MVC) en PHP [Actualizado 2022]](https://www.adaweb.es/modelo-vista-controlador-mvc-en-php-actualizado-2022/) - Adaweb. Adaweb.
- [Designlopers | Plantillas web gratis | sistemas web gratis](https://designlopers.com/post/Mi-primer-sistema-PHP-y-MVC/#!)
- [Free Course: CURSO de PHP & MVC: Mi primer SISTEMA [PHP, MVC, POO, MYSQL] from Udemy | Class Central](https://www.classcentral.com/course/udemy-mi-primer-sistema-php-mvc-mysql-69592). Class Central.


