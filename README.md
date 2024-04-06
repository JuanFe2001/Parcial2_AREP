## Escuela Colombiana de Ingeniería
### Arquitecturas Empresariales – AREP
# Parcial2-AREP

Diseñe un prototipo de sistema de microservicios que tenga un servicio (En la figura se representa con el nombre Math Services) para computar las funciones de ordenamiento.  El servicio de las funciones de ordenamiento debe estar desplegado en al menos dos instancias virtuales de EC2. Adicionalmente, debe implementar un service proxy que reciba las solicitudes de llamado desde los clientes  y se las delega a las dos instancias del servicio de ordenamiento usando un algoritmo de round-robin. El proxy deberá estar desplegado en otra máquina EC2. Asegúrese que se pueden configurar las direcciones y puertos de las instancias del servicio en el proxy usando variables de entorno del sistema operativo.  Finalmente, construya un cliente Web mínimo con un formulario que reciba el valor y de manera asíncrona invoke el servicio en el PROXY. Puede hacer un formulario para cada una de las funciones. El cliente debe ser escrito en HTML y JS.

 ## El prototipo cuenta con 2 clases principales las cuales son:

  **SearchFunctions**: Esta clase proporciona un servidor web que permite realizar búsquedas lineales y binarias a través de dos rutas HTTP /linear-search y /binary-search, respectivamente. Los resultados se devuelven en formato JSON.
  **ServiceProxy**: proporciona funcionalidad para agregar usuarios, calcular y verificar contraseñas hash, así como para configurar y ejecutar un servidor seguro de autenticación de usuario utilizando HTTPS.
