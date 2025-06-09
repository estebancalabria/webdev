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
