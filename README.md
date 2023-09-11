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

*Luego de haber realizado los 6 modulos solicitados de Trailhead, adjunto link para verificar las 6 insignias.*

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

*Luego, realizamos el diagrama que muestra la relación entre cada concepto*

![Diagrama sin título](https://github.com/tomascampi14/ProContacto/assets/144504388/d1dcd937-6bed-4340-a81a-0374dbd38b54)

## Ejercicio 6

### Soluciones de Salesforce
#### ¿Qué es Salesforce?
*Salesforce es una empresa de tecnología líder en el mundo que se especializa en el desarrollo de software y servicios en la nube relacionados con la gestión de relaciones con los clientes (CRM por sus siglas en inglés, Customer Relationship Management). Salesforce ofrece una amplia gama de productos y soluciones diseñados para ayudar a las empresas a administrar sus relaciones con los clientes, automatizar procesos comerciales y mejorar la toma de decisiones.*
#### ¿Qué es Sales Cloud?
*Sales Cloud es una plataforma de Salesforce diseñada para la gestión de ventas y relaciones con clientes. Ayuda a las empresas a automatizar procesos de ventas, administrar contactos y oportunidades, y mejorar la eficiencia en el ciclo de ventas.*
#### ¿Qué es Service Cloud?
*Service Cloud es una plataforma de Salesforce centrada en la atención al cliente. Permite a las empresas gestionar casos de servicio, brindar soporte técnico y ofrecer experiencias de atención al cliente más personalizadas.*
#### ¿Qué es Health Cloud?
*Health Cloud es una plataforma de Salesforce diseñada específicamente para la industria de la salud y el cuidado médico. Proporciona herramientas para la gestión de pacientes, el seguimiento de historias clínicas electrónicas y la coordinación de la atención médica, lo que permite a las organizaciones de atención médica ofrecer un mejor servicio y una atención más eficiente a los pacientes.*
#### ¿Qué es Marketing Cloud?
*Marketing Cloud es una plataforma de Salesforce que se enfoca en la gestión de marketing y la automatización de marketing. Permite a las empresas crear campañas de marketing, enviar correos electrónicos, analizar el rendimiento de las campañas y personalizar la interacción con los clientes para mejorar las estrategias de marketing.*

### Funcionalidades de Salesforce
#### ¿Qué es un RecordType?
*Un RecordType es un concepto utilizado en Salesforce para definir diferentes categorías o tipos de registros dentro de un objeto personalizado o estándar. Cada tipo de registro tiene sus propios campos y configuraciones específicas, lo que permite personalizar cómo se capturan y almacenan los datos en Salesforce para diferentes propósitos.*
#### ¿Qué es un ReportType?
*Un ReportType en Salesforce es un concepto que define la estructura o el modelo de datos que se utilizará para crear informes en la plataforma. Determina qué objetos están relacionados y qué campos están disponibles para incluir en un informe específico.*
#### ¿Qué es un Page Layout?
*Un Page Layout en Salesforce es una configuración que define cómo se muestra y se organiza la información en la interfaz de usuario de un registro de un objeto en particular. En otras palabras, determina la apariencia y la disposición de los campos y la información en la página de detalle de un registro.*
#### ¿Qué es un Compact Layout?
*Un Compact Layout en Salesforce es una configuración que define qué campos y acciones se muestran de manera rápida y resumida en la parte superior de un registro de un objeto cuando se ve en una lista o en una vista de lista, como una lista de registros en una vista de lista de un objeto personalizado o estándar.*
#### ¿Qué es un Perfil?
*Un Perfil en Salesforce es una configuración que define qué acciones y datos pueden realizar y ver los usuarios en la plataforma. Cada usuario de Salesforce se asocia con un perfil que determina sus permisos y nivel de acceso a objetos y registros en la aplicación.*
#### ¿Qué es un Rol?
*Un Rol en Salesforce es una entidad que se utiliza para definir la jerarquía de acceso en una organización. Los roles son parte integral del modelo de seguridad de Salesforce y determinan qué registros pueden ver y editar los usuarios en función de su posición en la jerarquía y su relación con otros registros.*
#### ¿Qué es un Validation Rule?
*Una Validation Rule (Regla de Validación) en Salesforce es una lógica personalizada que se utiliza para verificar y garantizar que los datos ingresados o modificados por los usuarios cumplan con ciertas condiciones o criterios específicos antes de permitir que se guarden en la base de datos. Las Validation Rules son una parte importante de la configuración de Salesforce para mantener la integridad y la consistencia de los datos.*
#### ¿Qué diferencia hay entre una relación Master Detail y Lookup?
*En Salesforce, las relaciones Master-Detail y Lookup son dos tipos diferentes de relaciones que se utilizan para conectar objetos (tablas) en la base de datos. Aquí tienes las diferencias clave entre ambas:*
##### *Relación Master-Detail:*

**Jerarquía de Propietario/Subordinado:** *En una relación Master-Detail, existe una jerarquía clara de propietario/subordinado entre los objetos. El objeto "Maestro" (Master) es el propietario y controla el ciclo de vida de los registros relacionados en el objeto "Detalle" (Detail).*

**Integridad Referencial Fuerte:** *Una relación Master-Detail establece una integridad referencial fuerte, lo que significa que los registros en el objeto "Detalle" dependen directamente de los registros en el objeto "Maestro". Si se elimina un registro maestro, todos los registros detallados relacionados se eliminan automáticamente (en cascada). Esto garantiza la consistencia de los datos.*

**Campos Obligatorios:** *Puedes hacer campos en el objeto "Detalle" obligatorios cuando tienen una relación Master-Detail. Esto significa que los registros detallados deben estar vinculados a un registro maestro y no pueden existir de forma independiente.*

##### Relación Lookup:

**Sin Jerarquía de Propietario/Subordinado:** *En una relación Lookup, no existe una jerarquía de propietario/subordinado. Los registros en el objeto relacionado (objeto "Lookup") no dependen de los registros en el objeto principal (objeto "Maestro"). Los registros Lookup pueden existir de forma independiente.*

**Integridad Referencial Flexible:** *A diferencia de Master-Detail, una relación Lookup no establece una integridad referencial fuerte. Si se elimina un registro en el objeto "Maestro," los registros relacionados en el objeto "Lookup" no se eliminan automáticamente. En su lugar, los campos de búsqueda simplemente se quedan vacíos.*

**Campos Opcionales:** *Los campos de búsqueda en un objeto "Lookup" suelen ser opcionales, lo que significa que los registros pueden o no estar vinculados a un registro principal.*
#### ¿Qué es un Sandbox?
*Un Sandbox es un entorno de desarrollo y pruebas aislado y separado en Salesforce que permite a los equipos de desarrollo probar cambios, personalizaciones y configuraciones en un ambiente seguro antes de implementarlos en su instancia de Salesforce en producción. Los Sandboxes son esenciales para garantizar la calidad y la estabilidad de las personalizaciones y las actualizaciones en Salesforce sin afectar directamente a la instancia en producción.*
#### ¿Qué es un ChangeSet?
*Un Change Set es una herramienta de Salesforce que se utiliza para recopilar, gestionar y migrar personalizaciones y configuraciones de un entorno Salesforce a otro, generalmente desde un entorno de desarrollo o pruebas a un entorno de producción. Los Change Sets facilitan el proceso de implementar cambios de manera controlada y aseguran que las personalizaciones y configuraciones se muevan de manera segura y coherente entre diferentes instancias de Salesforce.*
#### ¿Para qué sirve el import Wizard de Salesforce?
*El Import Wizard de Salesforce es una herramienta que permite a los usuarios cargar datos masivamente en una instancia de Salesforce desde fuentes externas, como hojas de cálculo de Excel o archivos CSV (valores separados por comas). Esta herramienta es útil para agilizar la importación de datos y garantizar la precisión de la información en Salesforce sin necesidad de programación o conocimientos técnicos avanzados.*
#### ¿Para qué sirve la funcionalidad Web to Lead?
*La funcionalidad "Web to Lead" en Salesforce es una herramienta que permite a las empresas capturar automáticamente información de clientes potenciales o prospectos que llenan formularios en su sitio web y convertirla en registros de clientes potenciales dentro de su instancia de Salesforce. Esta función es especialmente útil para la generación de clientes potenciales y la gestión de ventas, ya que automatiza la entrada de datos y facilita el seguimiento de clientes potenciales generados en línea.*
#### ¿Para qué sirve la funcionalidad Web to Case?
*La funcionalidad "Web to Case" en Salesforce es una herramienta que permite a las empresas automatizar la creación de casos de servicio al cliente a partir de solicitudes o consultas enviadas por los usuarios a través de formularios en línea en su sitio web. Esta función es esencial para agilizar la gestión de solicitudes de servicio al cliente, mejorar la eficiencia y ofrecer una experiencia de atención al cliente más rápida y efectiva.*

#### ¿Para qué sirve la funcionalidad Omnichannel?
*La funcionalidad Omnichannel en Salesforce es una herramienta que se utiliza para gestionar y optimizar la experiencia de atención al cliente a través de múltiples canales de comunicación de manera integrada y coherente. La idea principal detrás del enfoque Omnichannel es brindar a los clientes una experiencia fluida y consistente, independientemente del canal que elijan para interactuar con una empresa.*
#### ¿Para qué sirve la funcionalidad Chatter?
*La funcionalidad Chatter en Salesforce es una plataforma de colaboración y comunicación social empresarial que sirve para mejorar la comunicación interna y la colaboración entre los equipos de una organización. Chatter facilita la interacción entre los usuarios en la plataforma Salesforce y puede utilizarse para diversos propósitos en una empresa.*

## Ejercicio 7

*Consultamos nuestro ID haciendo el **GET** con **POSTMAN***

![Id_json](https://github.com/tomascampi14/ProContacto/assets/144504388/3e639088-6e4f-4485-9ed4-d2aa96898f1c)

*Luego, agregamos el campo al objeto Contact*

![Idprocontacto](https://github.com/tomascampi14/ProContacto/assets/144504388/0a6b240d-3568-4836-a678-ee6b09ca907c)

*Por último desarrollamos el Trigger solicitado*


```
trigger idprocontacto on Contact (after insert, after update) {
    // Lista para almacenar los IDs de contacto que cumplen con el criterio
    List<Id> contactIdsToUpdate = new List<Id>();
    
    // Recorre todos los registros de contacto que se han insertado o actualizado
    for (Contact con : Trigger.new) {
        if (con.idprocontacto != null) {
            contactIdsToUpdate.add(con.Id);
        }
    }
    
    if (!contactIdsToUpdate.isEmpty()) {
        // Realiza una solicitud al servicio web para obtener datos de correo electrónico
        // Utiliza la URL del servicio web y pasa los IDs de contacto como parámetros
        
        // Ejemplo de cómo hacer una solicitud HTTP en Apex (puede variar según la implementación):
        HttpRequest req = new HttpRequest();
        req.setEndpoint('https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json');
        req.setMethod('POST');
        req.setHeader('Content-Type', 'application/json');
        req.setBody(JSON.serialize(contactIdsToUpdate));
        
        // Enviar la solicitud y manejar la respuesta
        HttpResponse res = new Http().send(req);
        
        if (res.getStatusCode() == 200) {
            // Analizar la respuesta JSON para obtener los correos electrónicos
            List<Map<String, Object>> responseData = (List<Map<String, Object>>) JSON.deserializeUntyped(res.getBody());
            
            // Actualizar los contactos con los correos electrónicos obtenidos
            List<Contact> contactsToUpdate = new List<Contact>();
            for (Map<String, Object> data : responseData) {
                Contact con = new Contact(Id = (Id)data.get('ContactId'));
                con.Email = (String)data.get('Email');
                contactsToUpdate.add(con);
            }
            
            // Actualizar los contactos en Salesforce
            update contactsToUpdate;
        }
    }
}
```
