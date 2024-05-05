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



# 💙 APOYA ESTE PROYECTO 💙
<p>
Recuerda que puedes apoyar este proyecto suscribiéndote a mis canales de YouTube <a href="https://www.youtube.com/channel/UCRMJ0vxtnHh_UAq1Yx9BYWQ?sub_confirmation=1" target="_blank">CARLOS ALFARO</a> & <a href="https://www.youtube.com/channel/UCSKQJ3n2_CNjgB3sb2fvTdQ?sub_confirmation=1" target="_blank">DESIGNLOPERS</a>, tu apoyo es muy importante para seguir desarrollando este software y para traer nuevos proyectos.
</p>
