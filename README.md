Sistema Seguro Automóviles
Curso: Programación 4

Descripción
El proyecto consiste en desarrollar un sistema web en Java para la venta en línea de seguros para automóviles.
Los datos se almacenarán en una base de datos. El sistema permitirá a los clientes cotizar y comprar pólizas de seguro para sus automóviles, así como revisar el estado de sus pólizas en cualquier momento. Antes de utilizar el sistema, los clientes deberán registrarse o identificarse. Por otro lado, el administrador del sistema podrá registrar los datos de marcas y modelos de autos, así como las coberturas disponibles.
Este proyecto es en grupos 
El proyecto debe cumplir con los siguientes requisitos:

El sistema seguirá una arquitectura de tres capas (Presentación, Lógica y Datos).
Se implementará utilizando páginas dinámicas en el servidor, siguiendo el patrón Modelo-Vista-Controlador mediante Servlets, JSPs (Java Server Pages) .
El sistema implementará el control de acceso mediante sesiones en el servidor, utilizando un usuario y una clave. Solo se habilitarán las funcionalidades correspondientes al rol del usuario.
En este proyecto se utilizo el framework de Sprint Boot, de ahí se utilizo lo que es Sprint Security,H2 como base de datos,
Funcionalidades
Cliente-Registro: Los clientes pueden registrarse en el sistema proporcionando su identificación, clave, nombre, teléfono, correo y medio de pago (datos de tarjeta).
Cliente-Identificación (login): Los clientes pueden identificarse utilizando su identificación y clave. Se proporcionará un enlace a la página de registro de cliente en caso de que aún no se hayan registrado. Una vez identificados, se redirigirán a su página de pólizas.
Cliente-Actualización: Los clientes pueden modificar sus datos de teléfono, correo, etc. en cualquier momento.
Cliente-Gestión de Pólizas: Los clientes pueden listar sus pólizas y filtrarlas por número de placa. También pueden ver los detalles de una póliza específica.
Cliente-Comprar (agregar) póliza: Los clientes pueden contratar una póliza para un vehículo ingresando los datos necesarios, como número de placa, marca y modelo, año, valor asegurado, plazos de pago, fecha de inicio de vigencia y coberturas seleccionadas. El sistema mostrará el costo de la póliza y permitirá su compra.
Administrador-Identificación (login): Los administradores pueden identificarse utilizando su identificación y clave. Se mostrará un menú con las opciones correspondientes.
Administrador-Listado clientes y pólizas: Los administradores pueden listar los clientes y ver las pólizas asociadas a cada cliente.
Administrador-Gestión de Marcas y Modelos: Los administradores pueden listar las marcas y modelos de autos, así como agregar nuevos registros. Al registrar un modelo de auto, se deberá incluir una imagen correspondiente.
Administrador-Gestión de Categorías y Coberturas: Los administradores pueden listar las categorías y coberturas disponibles, y también agregar nuevos registros. Cada categoría tiene una identificación autogenerada y una descripción. Cada cobertura pertenece a una categoría y tiene una identificación autogenerada, una descripción y un costo (mínimo y porcentual del valor asegurado, aplicando el mayor).
