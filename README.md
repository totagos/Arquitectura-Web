# Gestor de contraseñas

## Descripción del proyecto
Este proyecto trata del desarrollo de una aplicación web sencilla para el manejo de contraseñas, orientada a ciberseguridad.  
El objetivo principal es que cada usuario pueda almacenar, consultar y gestionar sus credenciales/contraseñas de manera segura.

## Funcionalidades
- Login de usuarios  
  - Autenticación con validación de credenciales  
  - Uso de hash para proteger contraseñas  

- Gestionar las contraseñas  
  - Guardar contraseñas asociadas a un tema (por ejemplo redes sociales, bancos, etc).  
  - Encriptación antes de almacenarlas en la base de datos.  
  - Posibilidad de buscarlas y visualizarlas en la interfaz.  

- Validar  
  - Reglas básicas: longitud mínima, uso de mayúsculas, números y caracteres especiales.  
  - Indicador de fortaleza (fácil, media, fuerte).  

## Endpoints de la API

### Usuarios
- POST `/api/user` → Registrar un nuevo usuario  
- GET `/api/user/:id` → Obtener información de un usuario  

### Sesión
- POST `/api/login` → Iniciar sesión  
- POST `/api/logout` → Cerrar sesión  

### Credenciales
- GET `/api/credenciales` → Listar todas las credenciales  
- POST `/api/credenciales` → Crear una credencial  
- GET `/api/credenciales/:id` → Ver una credencial  
- PUT `/api/credenciales/:id` → Actualizar una credencial  
- DELETE `/api/credenciales/:id` → Eliminar una credencial  

### Utilidades
- POST `/api/strength` → Evaluar fortaleza de contraseña  
- GET `/api/estado` → Estado del servicio  
