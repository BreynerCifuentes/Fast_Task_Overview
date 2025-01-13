# Fast Task: API para Gestión de Tareas 📝

¡Bienvenido a la documentación de Fast Task! Este proyecto es una API para la gestión de tareas, desarrollada con Python (Flask) y bases de datos SQL (MySQL). A continuación, se describen sus funcionalidades y cómo funciona.

## Descripción del Proyecto
Fast Task permite:
- Crear, leer, actualizar y eliminar (CRUD) Tableros, listas y tareas.
- Manejo de datos en formato JSON para la comunicación con la API.

## Tecnologías Utilizadas
- **Python**: Lenguaje principal.
- **Flask**: Framework para la creación de APIs RESTful.
- **MySQL**: Base de datos ligera para almacenamiento de datos.
- **GitHub**: Control de versiones.

## Capturas de Pantalla
### 1. Fotos de la app
![Inicio](ruta/a/la/imagen1.png)


## ¿Cómo funciona?
### **Endpoints principales:**
- `GET /Fast_Task/iniciar_sesion/<correo>/<contrasena>`: Inicia sesión con un usuario de la base de datos.
- `POST /Fast_Task/agregar_usuario`: Agrega un usrario a la base de datos.
- `GET /Fast_Task/buscar_tablero/<nombre_tablero>/<id_usuario>`: Busca un tablero en especifico.
- `GET /Fast_Task/tableros/<id_usuario>`: Busca todos los tableros de un usuario.
- `POST /Fast_Task/agregar_tablero/<id_usuario>`: Agrega un tablero a un usuario.
- `PUT /Fast_Task/editar_tablero/<id_tablero>`: Edita un tablero en especifico.
- `DELETE /Fast_Task/eliminar_tablero/<id_tablero>`: Elimina un talbero en esepecifico.
- `GET /Fast_Task/buscar_lista/<nombre_lista>/<id_tablero>`: Busca una lista en especifico.
- `GET /Fast_Task/listas_tablero/<id_tablero>`: Busca todas las listas de un tablero.
- `POST /Fast_task/agregar_lista/<id_tablero>`: Agrega una lista a un tablero.
- `PUT /Fast_Task/editar_lista/<id_lista>`: Edita una lista en especifico.
- `DELETE /Fast_Task/eliminar_lista/<id_lista>`: Elimina una lista en especifico.
- `GET /Fast_Task/buscar_tarea/<nombre_tarea>/<id_lista>`:  Busca una tarea en especifico.
- `GET /Fast_Task/tareas_lista/<id_lista>`: Busca todas las tareas de una lista.
- `POST /Fast_Task/agregar_tarea/<id_lista>`: Agrega una tarea a una lista.
- `PUT /Fast_Task/editar_tarea/<id_tarea>`: Edita una tarea en especifico.
- `DELETE /Fast_Task/eliminar_tarea/<id_tarea>`: Elimina una tarea en especifico.

### Ejemplo de JSON para Crear una Tarea
```json
{
  "nombre_tarea": "Primera tarea",
  "contenido": "Descripción de mi primera tarea"
}
