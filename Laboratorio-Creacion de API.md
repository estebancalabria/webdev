# Laboratorio : Creacion de API Rest

Crear una API Restful en Spring siguiendo la siguiente convencion de nombre

* Sustantivos, no verbos
* Plural para los recursos
* Kebab-case para palabras compuestas
* Nombres consistentes en toda la api
* Utilizar los metodos http para definir la accion
* Utilizar queryparams para orden, filtros y paginacion
* Utilizar minusculas para todo asi nos ahorramos problemas si cambiamos de servidor web

Disenio de nuestra API

Endpoints

* CONSULTAR/LISTAR CLIENTES       :     GET    /api/clientes
* CONSULTAR/LISTAR  UN CLIENTE    :     GET    /api/clientes/{id}
* CREAR CLIENTE                   :     POST   /api/clientes          (uSA EL BODY)
* MODIFICAR CLIENTE               :     PUT    /api/clientes/{id}    
* BORRAR CLIENTE                  :     DELETE /api/clientes/{id}

> Para nombres compuestos
> GET /api/ordenes-de-produccion (notacion kebab)   
> pueeede ser /api/ordenes/produccion si hay otro tipo de ordenes.....    
> pueeede ser /api/compras/clientes  (Organizacion por dominios funcionales DDD)   
