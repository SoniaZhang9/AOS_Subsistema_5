# Arquitectura Orientada a Servicios 2021-22

## Subsistema 5: Gestión de facturas a los clientes por los trabajos realizados
- `/factura`<br /> 
POST de factura va a necesitar `clienteId` y un array de `trabajos`. Esta decisión es porque se ha considerado que este subsistema se encargará solamente de la creación de facturas.<br /> 
La lógica de comprobación que todos los trabajos solicitados por un cliente están terminados y la posterior llamada a este subsistema enviando los datos mencionados, se encargará otro sistema. <br /> <br/>
- Desde el punto de vista del usuario, querrá visualizar en una factura, **todos los detalles de los trabajos correspondientes**. Por ello, se ha considerado que en el esquema `factura` contenga una lista de trabajos con el esquema completo de `trabajo`, en vez de un único identificador de trabajo. <br/><br/>
- Se ha especificado endpoints para `búsqueda de facturas` por cliente, rango de fecha y rango de importe total <br/><br/>
- Documentación de la especificación (online)
https://app.swaggerhub.com/apis-docs/SoniaZhang9/PracticaAOS-Subsistema-5/1.0.0 

## Intrucciones de despliegue
Situarse sobre el directorio principal del proyecto y escribir en la terminal `docker compose up`. <br/>
De esta manera se podrá visitar estos links:
- Frontend -> http://localhost:8000/
- Backend -> <br/>
<img width="772" alt="Captura de pantalla 2022-04-16 a las 14 36 34" src="https://user-images.githubusercontent.com/78765878/163675240-24e09782-3653-4e7d-aeaf-fbac877af12a.png"> 
