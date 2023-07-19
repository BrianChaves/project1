# Sistema Seguro Automóviles

## Descripción

El proyecto consiste en desarrollar un sistema web en Java para la venta en línea de seguros para automóviles. Los clientes podrán cotizar y comprar pólizas de seguro para sus vehículos, así como revisar el estado de sus pólizas en cualquier momento. El sistema también permitirá al administrador registrar datos de marcas, modelos y coberturas de autos.

Este proyecto se realiza en grupos como parte del curso de Programación 4.

### Requisitos

El sistema debe cumplir con los siguientes requisitos:

- Seguir una arquitectura de tres capas: Presentación, Lógica y Datos.
- Implementar páginas dinámicas en el servidor utilizando el patrón Modelo-Vista-Controlador mediante Servlets y JSPs (Java Server Pages).
- Implementar control de acceso mediante sesiones en el servidor utilizando un usuario y una clave. Solo se habilitarán las funcionalidades correspondientes al rol del usuario.
- Utilizar el framework Spring Boot, junto con Spring Security, para el desarrollo del proyecto.
- Se utilizar una base de datos H2.

### Funcionalidades

El sistema contará con las siguientes funcionalidades:

1. **Cliente-Registro**: Los clientes podrán registrarse en el sistema proporcionando su identificación, clave, nombre, teléfono, correo y medio de pago (datos de tarjeta).
2. **Cliente-Identificación (login)**: Los clientes podrán identificarse utilizando su identificación y clave. Se proporcionará un enlace a la página de registro de cliente en caso de que aún no se hayan registrado. Una vez identificados, se redirigirán a su página de pólizas.
3. **Cliente-Actualización**: Los clientes podrán modificar sus datos de teléfono, correo, etc. en cualquier momento.
4. **Cliente-Gestión de Pólizas**: Los clientes podrán listar sus pólizas y filtrarlas por número de placa. También podrán ver los detalles de una póliza específica.
5. **Cliente-Comprar (agregar) póliza**: Los clientes podrán contratar una póliza para un vehículo ingresando los datos necesarios, como número de placa, marca y modelo, año, valor asegurado, plazos de pago, fecha de inicio de vigencia y coberturas seleccionadas. El sistema mostrará el costo de la póliza y permitirá su compra.
6. **Administrador-Identificación (login)**: Los administradores podrán identificarse utilizando su identificación y clave. Se mostrará un menú con las opciones correspondientes.
7. **Administrador-Listado clientes y pólizas**: Los administradores podrán listar los clientes y ver las pólizas asociadas a cada cliente.
8. **Administrador-Gestión de Marcas y Modelos**: Los administradores podrán listar las marcas y modelos de autos, así como agregar nuevos registros. Al registrar un modelo de auto, se deberá incluir una imagen correspondiente.
9. **Administrador-Gestión de Categorías y Coberturas**: Los administradores podrán listar las categorías y coberturas disponibles, y también agregar nuevos registros. Cada categoría tendrá una identificación autogenerada y una descripción. Cada cobertura pertenecerá a una categoría y tendrá una identificación autogenerada, una descripción y un costo (mínimo y porcentual del valor asegurado, aplicando el mayor).

