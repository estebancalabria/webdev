# Formas de Autenticacion de una API

##  Baisc Authentication

Se manda en el header http un header 
> Authorization : Basic dsfhskdfhjskfhskfsdfhdjhksfkd=
El codigo es el usuario:clave codificado en base64
Si la usamos por https es relativamente segura.
Muchos le agregan una capa mas de seguridad encriptando la informacion
No se suele usar mucho

## Autenticacion por API Key

Se manda en el header una clave de api 
> x-api-key : 123453343
Si se filtra la clave secreta cualqueira puede usar la api en nuestro nombre
Es un estandar que se utiliza mucho con api publicas

## Autenticacion por Token (OAuth 2.0)

El cliente obtiene priro un token (access token) y lo envia en el header en caa peticion para autizar
> Authorization : Bearer dhdfjfhjhfjkshfksdhfk
Si el token lo provee un servicio de terceros como Google, Microsoft, Facebook tenemos la base del estandar OAuth 2.0

## JWT (Jason Web Token)

Es una forma mas que de autenticacion de codificar datos en un token que puede ser decodificado por el servidor
> https://jwt.io/


