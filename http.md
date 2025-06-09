# HTTP
---

## Peticiones HTTP (REQUEST)

  [Linea de Solicitud]         GET /      

  [Headers]                    Content-type : application/json  o text/html o image/png
   			       User-Agent : Mozilla/5.0

  [Renglone en blanco]

  [Body]                       { nombre : "Esteban" }
  (para POST/ PUT)

Ejemplo peticion (reuest)

```
   GET /      
   Content-type : application/json  o text/html
   User-Agent : Mozilla/5.0

   { nombre : "Esteban" }
```


## Respuesta HTTP (Response)


  [Linea de Estado]           HTTP/<version> <codigo> <mensaje>
  
  [Headers]                   Content-type : text/html
                              Content-Length : Longitud tespuesta
                              Set-Cookie: ....

  [Renglone en blanco]

  [Body]                      <html>
				  ....
                              </html>

Ejemplo Respuesta

```
   HTTP/1.1 200 OK
   Content-type : text/html
   Content-Length : Longitud tespuesta
   
   <html>
        ...
   </html>
```
---
## Headers

### Headers Comunes en Requests

* Content-Type
* Usert-Agent
* Cookie
* Origin
* Accept
* Accept-Languange
* Authorization
  
### Headers Comunes en Response

* Content-Type
* Content-Length
* Set-Cookie

---

## Status Code (Codigos de Respuesta)

* 1xx   Informativos
* 2xx   Exito
* 3xx   Redireccioens (Se necesita una accion adicional)
* 4xx   Errores del cliente
* 5xx   Errores del servidor

### Status code 200

* 200 OK
* 201 Created
* 204 No content

### Status code 400

* 400 Bad Request      ?pagina=10000 y la pagina 10000 no existe
* 401 Unauthorized     sin Login
* 403 Forbiden         sin permiso
* 404 Not Found

### Status code 500

* 500 Internar Server Error
* 502 Bad gateway   (proxy, firewall)
* 503 Service Unavailable

