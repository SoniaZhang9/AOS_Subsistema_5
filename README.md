# Arquitectura Orientada a Servicios 2021-22

## Subsistema 5: Gestión de facturas a los clientes por los trabajos realizados
- `/factura`<br /> 
Post de factura va a necesitar `clienteId` y un array de `trabajos`. Esta decisión es debido a que este subsistema sólo se encarga de la creación de facturas.<br /> 
La lógica de comprobación que todos los trabajos solicitados por un cliente están terminados y la posterior llamada a este subsistema se encargará otro sistema (que enviará los datos necesarios) 

- Item 2
- Item 3
