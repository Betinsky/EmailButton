# Boton que envia Emails

## Descripción
Este componente Java, denominado `EmailButton`, facilita el envío de correos electrónicos a través de una interfaz gráfica en aplicaciones Java Swing. Su integración en un JFrame o JDialog es sencilla, permitiendo al usuario enviar mensajes de manera rápida y eficiente.

La clase EmailButton se encarga de gestionar el envío del correo electrónico, interactuando con los datos proporcionados por el usuario, como la dirección de correo electrónico de destino, el asunto del mensaje y el cuerpo del mismo. Además, ofrece una interfaz intuitiva al mostrar mensajes de confirmación o errores mediante ventanas emergentes utilizando JOptionPane.

El componente utiliza el protocolo SMTP para enviar los correos electrónicos y está configurado para trabajar con el servidor de Gmail. Requiere la autenticación del usuario mediante un nombre de usuario y contraseña proporcionados en el código.


## Usos
El componente EmailButton se puede utilizar en una variedad de aplicaciones Java Swing que requieran funcionalidades de envío de correos electrónicos. Algunos de los usos más comunes incluyen:
1. **Aplicaciones de gestión de contactos**: Permite a los usuarios enviar correos electrónicos directamente desde la aplicación a los contactos almacenados en su base de datos.
2. **Sistemas de soporte al cliente**: Facilita el envío de respuestas rápidas a consultas de clientes o notificaciones sobre el estado de los tickets de soporte.
3. **Aplicaciones de productividad**: Integra la capacidad de enviar correos electrónicos como parte de las funciones de productividad, como recordatorios automáticos, informes de estado o notificaciones de eventos.
4. **Plataformas de redes sociales**: Permite a los usuarios compartir contenido a través del correo electrónico directamente desde la aplicación, como compartir publicaciones, fotos o enlaces.
5. **Herramientas de colaboración**: Facilita la comunicación entre usuarios al permitir el envío de mensajes de correo electrónico desde la aplicación, lo que puede ser útil en herramientas de gestión de proyectos, plataformas de trabajo en equipo, etc.
6. **Aplicaciones de marketing**: Ofrece una manera fácil de enviar campañas de correo electrónico directamente desde la aplicación, permitiendo a los usuarios comunicarse con clientes potenciales o existentes de manera efectiva.

## Características
Envío de Correos Electrónicos: Permite enviar correos electrónicos de manera rápida y sencilla directamente desde una aplicación Java Swing.
Interfaz Gráfica Intuitiva: Incorpora una interfaz gráfica amigable que facilita al usuario proporcionar la dirección de correo electrónico de destino, el asunto del mensaje y el cuerpo del correo electrónico.
Gestión de Errores: Maneja los posibles errores durante el proceso de envío de correos electrónicos, proporcionando mensajes claros de error y de confirmación al usuario.
Configuración de SMTP Personalizable: Permite configurar el servidor SMTP y el puerto según las necesidades específicas del entorno de correo electrónico del usuario.
Autenticación Segura: Utiliza autenticación con nombre de usuario y contraseña para garantizar la seguridad y la privacidad en el proceso de envío de correos electrónicos.

## Requisitos
Java Swing: El componente está diseñado para ser integrado en aplicaciones Java Swing, por lo que se requiere un entorno de desarrollo compatible con esta tecnología.
Conexión a Internet: Para enviar correos electrónicos, se necesita una conexión activa a Internet para establecer la comunicación con el servidor SMTP.
Cuenta de Correo Electrónico: Se requiere una cuenta de correo electrónico válida para autenticarse en el servidor SMTP y enviar correos electrónicos.

## API
### EmailButton

#### Descripción
La clase `EmailButton` simplifica el proceso de envío de correos electrónicos dentro de aplicaciones Java Swing. Proporciona una interfaz gráfica intuitiva para que los usuarios ingresen la dirección de correo electrónico del destinatario, el asunto del correo electrónico y el cuerpo del mensaje. Además, maneja la configuración del servidor SMTP y la autenticación del usuario para garantizar un envío seguro. Con mensajes claros de confirmación o errores, esta clase facilita la comunicación efectiva a través del correo electrónico en las aplicaciones Java Swing.


### Campos

| Tipo | Campo | Descripción |
|------|-------|-------------|
| `String` | `email` | Almacena la dirección de correo electrónico del destinatario. |
| `String` | `subject` | Almacena el asunto del correo electrónico. |
| `String` | `message` | Almacena el cuerpo del mensaje del correo electrónico. |

#### Métodos

| Nombre | Tipo de Dato que Retorna | Tipo de dato que Recibe | Descripción |
|--------|---------------------------|-------------------------|-------------|
| `setEmail` | `void` | `String email` | Establece la dirección de correo electrónico del destinatario. |
| `setSubject` | `void` | `String subject` | Establece el asunto del correo electrónico. |
| `setMessage` | `void` | `String message` | Establece el cuerpo del mensaje del correo electrónico. |
| `sendEmail` | `void` | - | Envía el correo electrónico utilizando las configuraciones de servidor SMTP proporcionadas y los datos ingresados por el usuario. |



### EmailButton

#### Descripción
`EmailButton` es un componente GUI diseñado como un botón en aplicaciones Java Swing que facilita el envío de correos electrónicos. Permite a los usuarios enviar mensajes de manera rápida y sencilla, gestionando la configuración del servidor SMTP y la autenticación del usuario.

#### Campos
| Tipo | Campo | Descripción |
|------|-------|-------------|
| `String` | `email` | Almacena la dirección de correo electrónico del destinatario. |
| `String` | `subject` | Almacena el asunto del correo electrónico. |
| `String` | `message` | Almacena el cuerpo del mensaje del correo electrónico. |

#### Constructores
| Constructor | Descripción |
|-------------|-------------|
| `EmailButton()` | Inicializa el botón y configura su tamaño predeterminado. |

#### Métodos
| Nombre | Tipo de Dato que Retorna | Tipo de dato que recibe | Descripción |
|--------|---------------------------|-------------------------|-------------|
| `setEmail` | `void` | `String email` | Establece la dirección de correo electrónico del destinatario. |
| `setSubject` | `void` | `String subject` | Establece el asunto del correo electrónico. |
| `setMessage` | `void` | `String message` | Establece el cuerpo del mensaje del correo electrónico. |
| `sendEmail` | `void` | - | Envía el correo electrónico utilizando las configuraciones de servidor SMTP proporcionadas y los datos ingresados por el usuario. |


## Instalación

Para utilizar este componente en tu proyecto, sigue estos pasos:

1. **Obtener el Repositorio:**
   Clona el repositorio con el siguiente comando:

   ```bash
   git clone https://github.com/Betinsky/EmailButton
O bien, descarga el ZIP desde la interfaz de GitHub.

Importar el Proyecto:
Importa el proyecto en tu IDE preferido (NetBeans, Eclipse, IntelliJ, etc.).
Compilar el Proyecto:
Asegúrate de que el proyecto se compila sin errores para crear el archivo .jar según la versión de tu Java.


## Uso

### Configurar Correo Electrónico:
Antes de utilizar el componente, asegúrate de configurar el correo electrónico desde el cual se enviarán los mensajes, así como el servidor SMTP. 
Para hacer esto, busca en el código del componente la sección donde se especifica el servidor SMTP y el puerto del correo electrónico:

String smtpServer = "smtp.example.com"; // Cambia "smtp.example.com" por tu servidor SMTP 

String smtpPort = "el puerto"; // Cambia "el puerto" por el puerto SMTP correspondiente 

Antes de utilizar el componente, asegúrate de configurar el correo electrónico desde el cual se enviarán los mensajes. 
Para hacer esto, busca en el código del componente la sección donde se especifica el nombre de usuario y la contraseña del correo electrónico:


String username = "tucorreo@gmail.com"; // Cambia por tu dirección de correo electrónico 

String password = "tupassword"; // Cambia por tu contraseña 


### Agregar Componente a la Paleta:
1. Compila tu proyecto para crear el archivo .jar.
2. Agrega el componente a tu paleta de componentes. Para hacer esto, sigue los pasos adecuados para tu IDE. Por ejemplo, en NetBeans:
3. Da clic derecho en la paleta de componentes y selecciona Palette Manager.
4. Selecciona Add From Jar.
5- Navega hasta la carpeta dist del proyecto y selecciona el archivo .jar generado.

## Utilizar el Componente:
Arrastra y suelta el componente EmailButton en tu diseño de interfaz de usuario.
Configura el destinatario, asunto y cuerpo del mensaje utilizando los métodos proporcionados por el componente:

emailButton.setEmail("destinatario@example.com");

emailButton.setSubject("Asunto del correo");

emailButton.setMessage("Cuerpo del correo");

### Envía el correo electrónico utilizando el método 
sendEmail():


## Funcionamiento
¡Descubre cómo funciona este componente visual *Boton que envia Emails*!

Haz clic para ver el video ahora mismo ---> [EmailButton](https://youtu.be/VPbEidsRFiM) 

## Contribuir
Si deseas contribuir a este proyecto, por favor sigue los siguientes pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama para tu característica o corrección de errores.
3. Haz tus cambios.
4. Envía un pull request.

## Autores
- Mario Alberto Barbosa Santiago- *Estudiante del ITO* - [Contacto](https://github.com/Betinsky])
- Bolivar Garcia Osorio - *Estudiante del ITO* - [Contacto](https://github.com/Blvrr12])





