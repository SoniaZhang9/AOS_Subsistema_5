# Arquitectura Orientada a Servicios 2021-22

## Subsistema 5: Gestión de facturas a los clientes por los trabajos realizados
- `/factura`<br /> 
POST de factura va a necesitar `clienteId` y un array de `trabajos`. Esta decisión es debido a que este subsistema sólo se encarga de la creación de facturas.<br /> 
La lógica de comprobación que todos los trabajos solicitados por un cliente están terminados y la posterior llamada a este subsistema se encargará otro sistema (que enviará los datos mencionados para la creación de una factura). <br /> <br/>
- Se ha considerado que en el esquema `factura` contenga el esquema completo de `trabajo`, en vez de una referencia a ello, debido a que desde el punto de vista del usuario, querrá visualizar en una factura, todos los detalles de los trabajos correspondientes
- Item 2
- Item 3
