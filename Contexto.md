
---
0. **Resumen del proyecto archivos.py** 
    Aquí tienes un **resumen de las funcionalidades de cada archivo `.py`** para que puedas usarlo como contexto :

---

### **app.py**  
Este archivo es el núcleo de la aplicación Flask. Contiene las rutas y la lógica del backend. Aquí están las funcionalidades principales:

1. **Autenticación y gestión de usuarios**:
   - **Login**: Permite a los usuarios iniciar sesión con su correo y contraseña.
   - **Registro**: Permite a los usuarios registrarse con un nombre de usuario, correo y contraseña.
   - **Recuperación de contraseña**: Permite a los usuarios solicitar un enlace de recuperación si olvidan su contraseña.
   - **Cerrar sesión**: Cierra la sesión del usuario.

2. **Gestión de películas**:
   - **Listar películas**: Muestra una lista paginada de películas activas.
   - **Crear película**: Permite agregar una nueva película con título, descripción, imagen, calificación y categoría.
   - **Editar película**: Permite modificar los detalles de una película existente.
   - **Eliminar película**: Desactiva una película (no la elimina físicamente).

3. **Gestión de categorías**:
   - **Listar categorías**: Muestra una lista paginada de categorías activas.
   - **Crear categoría**: Permite agregar una nueva categoría con nombre y descripción.
   - **Editar categoría**: Permite modificar los detalles de una categoría existente.
   - **Eliminar categoría**: Desactiva una categoría (no la elimina físicamente).

4. **Gestión de empleados**:
   - **Listar empleados**: Muestra una lista paginada de empleados activos.
   - **Crear empleado**: Permite agregar un nuevo empleado con nombre, correo, teléfono y cargo.
   - **Editar empleado**: Permite modificar los detalles de un empleado existente.
   - **Eliminar empleado**: Desactiva un empleado (no lo elimina físicamente).

5. **Gestión de clientes**:
   - **Listar clientes**: Muestra una lista paginada de clientes activos.
   - **Crear cliente**: Permite agregar un nuevo cliente con nombre, correo, teléfono y dirección.
   - **Editar cliente**: Permite modificar los detalles de un cliente existente.
   - **Eliminar cliente**: Elimina físicamente un cliente de la base de datos.

6. **Gestión de facturas**:
   - **Listar facturas**: Muestra una lista paginada de facturas activas.
   - **Crear factura**: Permite agregar una nueva factura con fecha, total, cliente, empleado y plan asociado.
   - **Editar factura**: Permite modificar los detalles de una factura existente.
   - **Eliminar factura**: Desactiva una factura (no la elimina físicamente).

7. **Gestión de planes**:
   - **Listar planes**: Muestra una lista paginada de planes activos.
   - **Crear plan**: Permite agregar un nuevo plan con nombre, precio, calidad y número de dispositivos permitidos.
   - **Editar plan**: Permite modificar los detalles de un plan existente.
   - **Eliminar plan**: Desactiva un plan (no lo elimina físicamente).

8. **API de películas**:
   - **/api/peliculas**: Devuelve un JSON con las primeras 50 películas registradas en la base de datos.

9. **Páginas estáticas**:
   - **Home**: Página principal del sitio.
   - **Planes**: Página que muestra los planes disponibles.
   - **Interface**: Página protegida solo para usuarios autenticados.

10. **Paginación**:
    - Todas las listas (películas, categorías, empleados, clientes, facturas, planes) están paginadas para mejorar la usabilidad.

11. **Manejo de sesiones**:
    - Uso de `session` para mantener al usuario logueado y proteger rutas.

12. **Manejo de errores**:
    - Uso de `try-except` para capturar errores y mostrar mensajes flash al usuario.

---

### **bd.py**  
Este archivo define los modelos de la base de datos utilizando SQLAlchemy. Aquí están las funcionalidades principales:

1. **Modelo Usuario**:
   - Almacena información de los usuarios (nombre de usuario, correo, contraseña y estado activo/inactivo).

2. **Modelo Categoria**:
   - Almacena categorías de películas (nombre, descripción y estado activo/inactivo).
   - Relación con el modelo `Pelicula`.

3. **Modelo Pelicula**:
   - Almacena información de películas (título, descripción, imagen, calificación, categoría y estado activo/inactivo).

4. **Modelo Empleado**:
   - Almacena información de empleados (nombre, correo, teléfono, cargo y estado activo/inactivo).

5. **Modelo Cliente**:
   - Almacena información de clientes (nombre, correo, teléfono, dirección, fecha de registro y estado activo/inactivo).
   - Relación con el modelo `Facturacion`.

6. **Modelo Facturacion**:
   - Almacena información de facturas (fecha, total, estado activo/inactivo, cliente, empleado y plan asociado).

7. **Modelo Planes**:
   - Almacena información de planes (nombre, precio, calidad, número de dispositivos y estado activo/inactivo).
   - Relación con el modelo `Facturacion`.

---

### **config.py**  
Este archivo contiene la configuración de la aplicación Flask:

1. **Configuración de la base de datos**:
   - Define la URI de conexión a la base de datos MySQL (`mysql+pymysql://root:@localhost/cinesucre`).

2. **Clave secreta**:
   - Define una clave secreta para las sesiones y mensajes flash.

---

### **Resumen general**  
El proyecto "Cine Sucre" es una aplicación web que permite gestionar una plataforma de streaming de películas. Incluye funcionalidades CRUD para películas, categorías, empleados, clientes, facturas y planes, además de un sistema de autenticación y una API para consultar películas. La interfaz está diseñada para ser responsiva y moderna, utilizando Tailwind CSS 4. La base de datos se gestiona con MySQL y Flask-SQLAlchemy.




---

