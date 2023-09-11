# Prueba práctica ProContacto
*Una vez realizada la instalación del ambiente, se procede a resolver los ejercicios propuestos a partir del punto 2.*
## Ejercicio 2
#### ¿Que es un servidor HTTP?
*Un servidor HTTP (Hypertext Transfer Protocol Server) es un software o hardware que recibe y procesa solicitudes de navegadores web, dispositivos u otras aplicaciones para entregar contenido web, como páginas HTML, imágenes y archivos, a través de la red utilizando el protocolo HTTP.*
#### ¿Qué son los verbos HTTP? Mencionar los más conocidos
*Los verbos HTTP, también conocidos como métodos HTTP, son comandos utilizados en el protocolo HTTP para indicar la acción que se debe realizar en un recurso web. Los más conocidos son:*

**GET:** *Solicita y recupera datos de un recurso web.*
**POST:** *Envía datos al servidor para ser procesados y, generalmente, crear un nuevo recurso.*
**PUT:** *Actualiza un recurso web o crea uno nuevo si no existe.*
**DELETE:** *Elimina un recurso web especificado.*

#### ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?

*Un "request" (solicitud) en una comunicación HTTP es un mensaje enviado por un cliente (como un navegador web) al servidor para solicitar un recurso o realizar una acción en el servidor. Un "response" (respuesta) es el mensaje que el servidor envía de vuelta al cliente con la información solicitada o una confirmación de la acción realizada.*

*Los "headers" (encabezados) son componentes de estos mensajes que contienen información adicional sobre la solicitud o la respuesta. Los encabezados proporcionan detalles como el tipo de contenido, la longitud del contenido, la fecha de la solicitud, la codificación utilizada y más. Ayudan a los clientes y servidores a entender y procesar adecuadamente las solicitudes y respuestas HTTP.*

#### ¿Qué es un queryString? (En el contexto de una url)

*Un "queryString" es una parte de una URL que se utiliza para enviar datos al servidor como parte de una solicitud HTTP GET. Consiste en una cadena de texto que sigue al signo de interrogación "?" en una URL y contiene parámetros clave-valor separados por el símbolo "&". Estos parámetros se utilizan para transmitir información al servidor, como filtros de búsqueda, opciones de configuración o datos de identificación.*

#### ¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?

*El "responseCode" se refiere al código de estado HTTP que un servidor web envía como parte de la respuesta a una solicitud HTTP. Este código de estado proporciona información sobre el resultado de la solicitud y puede ayudar al cliente (por ejemplo, un navegador web) a comprender lo que sucedió con la solicitud. Algunos de los códigos de estado HTTP más comunes incluyen:*

- **200 OK:** *Indica que la solicitud se ha realizado correctamente, y la respuesta contiene la información solicitada.*

- **201 Created:** *Se utiliza para indicar que la solicitud ha llevado a la creación exitosa de un nuevo recurso en el servidor.*

- **204 No Content:** *Significa que la solicitud se ha realizado con éxito, pero no hay contenido para devolver en la respuesta.*

- **400 Bad Request:** *Indica que la solicitud del cliente es incorrecta o incomprensible para el servidor.*

- **401 Unauthorized:** *El cliente no está autorizado para acceder al recurso solicitado.*

- **403 Forbidden:** *El servidor entiende la solicitud, pero el acceso al recurso está prohibido.*

- **404 Not Found:** *El servidor no puede encontrar el recurso solicitado.*

- **500 Internal Server Error**: *Indica un error interno en el servidor que impide que la solicitud se complete correctamente.*

#### ¿Cómo se envía la data en un Get y cómo en un POST?

*En una solicitud HTTP GET, los datos se envían como parte de la URL en el "queryString". Los datos se adjuntan a la URL como parámetros clave-valor separados por el símbolo "&". Por ejemplo, en la URL "https://ejemplo.com/recurso?nombre=Juan&edad=30", los datos se envían como "nombre=Juan" y "edad=30" en el queryString.*

*En una solicitud HTTP POST, los datos se envían en el cuerpo (body) de la solicitud, en lugar de estar expuestos en la URL. Esto permite enviar datos más grandes y complejos, como formularios web. Los datos suelen estar codificados en un formato específico, como JSON o form-urlencoded. El servidor espera que los datos se encuentren en el cuerpo del mensaje y los procesa en consecuencia.*

#### ¿Qué verbo http utiliza el navegador cuando accedemos a una página?

*Cuando accedes a una página web en tu navegador, generalmente se utiliza el verbo HTTP GET para solicitar y recuperar la página y su contenido desde el servidor web. El navegador envía una solicitud GET al servidor web correspondiente para obtener la página HTML y otros recursos asociados, como imágenes, scripts y hojas de estilo. Esta es la acción más común cuando se navega por la web y se utiliza para obtener información del servidor para su visualización en el navegador.*

#### Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles

*JSON (JavaScript Object Notation) y XML (Extensible Markup Language) son dos formatos utilizados para representar datos estructurados:*

*JSON: Es un formato ligero y legible por humanos que se utiliza para transmitir datos. Los datos se representan en pares clave-valor y se asemeja a la estructura de los objetos en JavaScript*.

*Ejemplo:*

    {
      "nombre": "Juan",
      "edad": 30,
      "ciudad": "New Jork"
    }

*XML: Es un lenguaje de marcado que utiliza etiquetas para definir elementos y sus relaciones. Se utiliza en una amplia variedad de aplicaciones, incluidos documentos y datos estructurados.*

*Ejemplo de estructura XML:*

    <persona>
      <nombre>Juan</nombre>
      <edad>30</edad>
      <ciudad>New Jork</ciudad>
    </persona>

#### Explicar brevemente el estándar SOAP

*SOAP (Simple Object Access Protocol) es un protocolo estándar utilizado para la comunicación entre aplicaciones en la web. Está basado en XML y se utiliza para intercambiar mensajes estructurados entre sistemas distribuidos, independientemente de la plataforma o el lenguaje de programación que utilicen.*

*Las características clave de SOAP son:*

1. **Basado en XML**: *Los mensajes SOAP se escriben en formato XML, lo que los hace legibles por máquinas y humanos.*

3. **Protocolo independiente**: *SOAP puede ser utilizado sobre varios protocolos de transporte, incluyendo HTTP, SMTP, y otros, lo que lo hace altamente flexible.*

5. **Estructura de mensaje**: *Un mensaje SOAP consta de un encabezado opcional que contiene información de metadatos y un cuerpo que contiene los datos reales que se están transmitiendo.*

7. **Interoperabilidad**: *SOAP se enfoca en la interoperabilidad entre diferentes sistemas y plataformas, lo que lo hace adecuado para entornos heterogéneos.*

9. **Uso en servicios web**: *SOAP se utiliza comúnmente en servicios web, donde las aplicaciones pueden exponer funcionalidades a través de interfaces web estándar.*

#### Explicar brevemente el estándar REST Full

*REST (Representational State Transfer) es un estilo de arquitectura de software que se utiliza para diseñar sistemas web y servicios web. Cuando se habla de "RESTfull", se hace referencia a la aplicación de los principios REST en el diseño de una API web o un sistema web.*

*Los conceptos clave de un sistema RESTful son:*

1. **Recursos:** *En un sistema RESTful, los datos se modelan como recursos, que son identificados por URLs únicas. Por ejemplo, un recurso podría ser una entidad como un usuario, una publicación o un producto.*

3. **Verbos HTTP:** *REST utiliza los verbos HTTP estándar, como GET (para recuperar datos), POST (para crear datos), PUT (para actualizar datos) y DELETE (para eliminar datos), para interactuar con los recursos.*

5. **Estado de Representación:** *Los recursos pueden tener múltiples representaciones, como JSON o XML, y el cliente puede solicitar la representación deseada utilizando encabezados HTTP.*

7. **Sin estado:** *REST es "sin estado", lo que significa que cada solicitud del cliente al servidor debe contener toda la información necesaria para comprender y procesar la solicitud. No se almacena información de estado del cliente en el servidor entre solicitudes.*

9. **Interfaz uniforme:** *REST promueve una interfaz uniforme para interactuar con recursos, lo que facilita la comprensión y el uso de la API.*

11. **Cliente-Servidor:** *REST separa la interfaz del usuario (cliente) de la lógica del servidor, lo que permite que ambas partes evolucionen de manera independiente.*

#### ¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?

*Tal como mencionamos anteriormente, los "headers" (encabezados) en una solicitud HTTP son componentes de la solicitud que proporcionan información adicional sobre la misma. Los encabezados se componen de pares clave-valor y se utilizan para transmitir metadatos importantes sobre la solicitud. Algunos de los encabezados comunes en una solicitud HTTP incluyen:*

- **User-Agent**: *Identifica el tipo de navegador o cliente que realiza la solicitud.*
- **Host:** *Indica el nombre de dominio del servidor al que se está accediendo.*
- **Accept**: *Especifica el tipo de contenido que el cliente está dispuesto a aceptar como respuesta.*
- **Authorization:** *Contiene información de autenticación, como credenciales de usuario.*
- **Content-Type:** *Especifica el tipo de medios (media type) del contenido en el cuerpo de la solicitud.*

*El encabezado "Content-Type" es especialmente importante en las solicitudes que tienen un cuerpo (como las solicitudes POST) y en las respuestas. Indica el tipo de contenido que se encuentra en el cuerpo de la solicitud o respuesta, lo que permite al servidor o al cliente procesar los datos de manera adecuada.*

## Ejercicio 3

*Procedemos a realizar la solicitud del tipo **GET** y obtenemos los siguientes resultados del recurso WEB.*

![Get1](https://github.com/tomascampi14/ProContacto/assets/144504388/4b9bd56b-e0fe-4a45-8189-be67943a81b9)

*Luego realizamos la solicitud del tipo **POST** con el body indicando nombre y email.*

![Post](https://github.com/tomascampi14/ProContacto/assets/144504388/a995df84-a01b-4935-9e0f-a28b23e9e54a)

*Por ultimo, realizamos nuevamente un request  **GET** para obtener los nuevos resultados del recurso WEB.*

![Get2](https://github.com/tomascampi14/ProContacto/assets/144504388/f86974fa-2e71-43a9-bd50-42ac70833d02)

#### Diferencia entre el primer y ultimo GET
*Podemos observar que luego de realizar el request **POST** hemos enviado nuestros datos al servidor y hemos modificado los recursos originales que nos ofrecia la web.
Ahora podemos visualizar nuestros datos en el JSON que nos muestra el link original*

## Ejercicio 4

*Luego de haber realizado los 6 modulos solicitados de Trailheado, adjunto link para verificar las 6 insignias.*

`<link>` : <https://www.salesforce.com/trailblazer/tomascampilones>

## Ejercicio 5

- **Lead:** *Cliente Potencial. Es una persona o empresa que ha mostrado interés en los productos o servicios ofrecidos.*
- **Account:** *Cuenta. Es una entidad comercial o cliente con la que una empresa mantiene una relación continua.*
- **Contact:** *Contacto. Persona especifica asociada a una cuenta.*
- **Opportunity:** *Oportunidad. Es una posibilidad de negocio con un cliente potencial o existente.*
- **Product:** *Producto. Es un articulo o servicio que una empresa ofrece a sus clientes.*
- **PriceBook:** *Catálogo de precios. Es una lista de productos o servicios junto con sus precios asociados.*
- **Quote:** *Cotización. Es un documento que detalla los productos o servicios que una empresa esta dispuesta a proporcionar a un cliente.*
- **Asset:** *Activo. Representa un articulo o recurso que una empresa posee o administra.*
- **Case:** *Caso. Un caso se utiliza para registrar y dar seguimiento a las solicitudes, problemas o consultas de los clientes.*
- **Article:** *Artículo. Es una unidad de información que proporciona detalles sobre un tema en especifico.*

![Diagrama sin título](https://github.com/tomascampi14/ProContacto/assets/144504388/d1dcd937-6bed-4340-a81a-0374dbd38b54)
