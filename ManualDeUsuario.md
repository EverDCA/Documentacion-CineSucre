### Manual de Usuario del Aplicativo Web de Gestión de Contenidos Audiovisuales **Cine Sucre**

---

#### **1. Introducción**  
Este manual de usuario tiene como objetivo guiar a los usuarios en el uso del **Aplicativo Web de Gestión de Contenidos Audiovisuales Cine Sucre**. A través de este documento, los usuarios aprenderán a navegar por la plataforma, gestionar películas, categorías, empleados, clientes, facturas y planes, así como utilizar las distintas funcionalidades disponibles. La plataforma está diseñada para ser accesible, económica y enfocada en el contenido local, especialmente para el departamento de Sucre y otras regiones de Colombia con acceso limitado a servicios de streaming.

---

#### **2. Instalación y Configuración**  
Antes de utilizar la aplicación, es necesario instalar y configurar el entorno de desarrollo.

##### **2.1 Requisitos Previos**  
- **Python 3.10 o superior**: Necesario para ejecutar la aplicación Flask.  
- **Flask**: Framework web utilizado para construir la aplicación.  
- **MySQL Server**: Sistema de gestión de bases de datos relacional utilizado para almacenar la información de la plataforma.  
- **MySQL Workbench**: Herramienta gráfica para gestionar la base de datos MySQL.  
- **Tailwind CSS 4**: Framework de CSS utilizado para diseñar la interfaz de usuario.  
- **Navegador web compatible**: Google Chrome, Mozilla Firefox, Microsoft Edge o Safari.

##### **2.2 Instalación del Proyecto**  
1. **Clonar el repositorio**:  
   ```bash
   git clone https://github.com/usuario/cinesucre.git
   cd cinesucre
   ```

2. **Crear y activar un entorno virtual**:  
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   ```

3. **Instalar dependencias**:  
   ```bash
   pip install -r requirements.txt
   ```

4. **Configurar la base de datos**:  
   - Crear una base de datos en MySQL con el nombre `cinesucre_db`.  
   - Importar el archivo `cinesucre.sql` incluido en el proyecto para crear las tablas y datos iniciales.

5. **Ejecutar la aplicación**:  
   ```bash
   flask run
   ```

6. **Acceder a la aplicación**:  
   - Abra su navegador y vaya a `http://127.0.0.1:5000`.

---

#### **3. Requisitos del Sistema**  
Antes de comenzar a utilizar la aplicación, asegúrese de cumplir con los siguientes requisitos:  
- **Navegador web**: Google Chrome, Mozilla Firefox, Microsoft Edge o Safari.  
- **Conexión a Internet estable**: Aunque la plataforma está optimizada para funcionar en zonas con baja conectividad, se recomienda una conexión estable para una mejor experiencia.  
- **Cuenta de usuario**: Un administrador debe proporcionarle un usuario y contraseña para acceder.

---

#### **4. Acceso al Sistema**  

##### **4.1 Inicio de Sesión**  
1. Abra su navegador web y acceda a la URL de la aplicación.  
2. Ingrese su nombre de usuario y contraseña en los campos correspondientes.  
3. Haga clic en el botón **"Iniciar sesión"**.  
4. Si sus credenciales son correctas, será redirigido al panel principal.

##### **4.2 Recuperar Contraseña**  
1. En la pantalla de inicio de sesión, haga clic en **"¿Olvidó su contraseña?"**.  
2. Ingrese su correo electrónico y haga clic en **"Enviar"**.  
3. Siga las instrucciones enviadas a su correo para restablecer la contraseña.

---

#### **5. Navegación en la Aplicación**  
Al ingresar al sistema, encontrará un menú principal con las siguientes opciones:  
- **Dashboard**: Resumen de la actividad de la plataforma, como el número de películas, clientes y facturas registradas.  
- **Gestión de Películas**: Registro, edición y eliminación de películas.  
- **Gestión de Categorías**: Administración de categorías de películas.  
- **Gestión de Empleados**: Registro y administración del personal.  
- **Gestión de Clientes**: Registro y administración de clientes.  
- **Gestión de Facturas**: Registro y seguimiento de facturas.  
- **Gestión de Planes**: Creación y administración de planes de suscripción.  
- **Configuración**: Opciones para modificar información personal y ajustes de seguridad.

---

#### **6. Uso de Funcionalidades**  

##### **6.1 Gestión de Películas**  
1. **Listar películas**:  
   - Diríjase a la sección **"Gestión de Películas"**.  
   - Verá una lista paginada de películas activas.  
   - Puede filtrar y buscar películas por título o categoría.

2. **Agregar una película**:  
   - Haga clic en el botón **"Agregar Película"**.  
   - Complete los campos requeridos:  
     - **Título**: Nombre de la película.  
     - **Descripción**: Breve descripción del contenido.  
     - **Imagen**: Suba una imagen representativa de la película.  
     - **Calificación**: Seleccione la calificación (por ejemplo, PG-13, R, etc.).  
     - **Categoría**: Seleccione la categoría a la que pertenece la película.  
   - Presione **"Guardar"** para registrar la nueva película.

3. **Editar una película**:  
   - En la lista de películas, haga clic en el botón **"Editar"** junto a la película que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar una película**:  
   - En la lista de películas, haga clic en el botón **"Eliminar"** junto a la película que desea desactivar.  
   - La película no se eliminará físicamente, sino que se marcará como inactiva.

##### **6.2 Gestión de Categorías**  
1. **Listar categorías**:  
   - Diríjase a la sección **"Gestión de Categorías"**.  
   - Verá una lista paginada de categorías activas.  
   - Puede filtrar y buscar categorías por nombre.

2. **Agregar una categoría**:  
   - Haga clic en el botón **"Nueva Categoría"**.  
   - Complete los campos requeridos:  
     - **Nombre**: Nombre de la categoría.  
     - **Descripción**: Breve descripción de la categoría.  
   - Presione **"Guardar"** para registrar la nueva categoría.

3. **Editar una categoría**:  
   - En la lista de categorías, haga clic en el botón **"Editar"** junto a la categoría que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar una categoría**:  
   - En la lista de categorías, haga clic en el botón **"Eliminar"** junto a la categoría que desea desactivar.  
   - La categoría no se eliminará físicamente, sino que se marcará como inactiva.

##### **6.3 Gestión de Empleados**  
1. **Listar empleados**:  
   - Diríjase a la sección **"Gestión de Empleados"**.  
   - Verá una lista paginada de empleados activos.  
   - Puede filtrar y buscar empleados por nombre o cargo.

2. **Agregar un empleado**:  
   - Haga clic en el botón **"Nuevo Empleado"**.  
   - Complete los campos requeridos:  
     - **Nombre**: Nombre del empleado.  
     - **Correo**: Correo electrónico del empleado.  
     - **Teléfono**: Número de teléfono del empleado.  
     - **Cargo**: Cargo del empleado (por ejemplo, Administrador, Vendedor).  
   - Presione **"Guardar"** para registrar el nuevo empleado.

3. **Editar un empleado**:  
   - En la lista de empleados, haga clic en el botón **"Editar"** junto al empleado que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar un empleado**:  
   - En la lista de empleados, haga clic en el botón **"Eliminar"** junto al empleado que desea desactivar.  
   - El empleado no se eliminará físicamente, sino que se marcará como inactivo.

##### **6.4 Gestión de Clientes**  
1. **Listar clientes**:  
   - Diríjase a la sección **"Gestión de Clientes"**.  
   - Verá una lista paginada de clientes activos.  
   - Puede filtrar y buscar clientes por nombre o correo.

2. **Agregar un cliente**:  
   - Haga clic en el botón **"Nuevo Cliente"**.  
   - Complete los campos requeridos:  
     - **Nombre**: Nombre del cliente.  
     - **Correo**: Correo electrónico del cliente.  
     - **Teléfono**: Número de teléfono del cliente.  
     - **Dirección**: Dirección del cliente.  
   - Presione **"Guardar"** para registrar el nuevo cliente.

3. **Editar un cliente**:  
   - En la lista de clientes, haga clic en el botón **"Editar"** junto al cliente que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar un cliente**:  
   - En la lista de clientes, haga clic en el botón **"Eliminar"** junto al cliente que desea eliminar.  
   - El cliente se eliminará físicamente de la base de datos.

##### **6.5 Gestión de Facturas**  
1. **Listar facturas**:  
   - Diríjase a la sección **"Gestión de Facturas"**.  
   - Verá una lista paginada de facturas activas.  
   - Puede filtrar y buscar facturas por cliente, empleado o plan.

2. **Agregar una factura**:  
   - Haga clic en el botón **"Nueva Factura"**.  
   - Complete los campos requeridos:  
     - **Fecha**: Fecha de la factura.  
     - **Total**: Monto total de la factura.  
     - **Cliente**: Seleccione el cliente asociado a la factura.  
     - **Empleado**: Seleccione el empleado asociado a la factura.  
     - **Plan**: Seleccione el plan asociado a la factura.  
   - Presione **"Guardar"** para registrar la nueva factura.

3. **Editar una factura**:  
   - En la lista de facturas, haga clic en el botón **"Editar"** junto a la factura que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar una factura**:  
   - En la lista de facturas, haga clic en el botón **"Eliminar"** junto a la factura que desea desactivar.  
   - La factura no se eliminará físicamente, sino que se marcará como inactiva.

##### **6.6 Gestión de Planes**  
1. **Listar planes**:  
   - Diríjase a la sección **"Gestión de Planes"**.  
   - Verá una lista paginada de planes activos.  
   - Puede filtrar y buscar planes por nombre o precio.

2. **Agregar un plan**:  
   - Haga clic en el botón **"Nuevo Plan"**.  
   - Complete los campos requeridos:  
     - **Nombre**: Nombre del plan (por ejemplo, Básico, Premium).  
     - **Precio**: Costo del plan.  
     - **Calidad**: Calidad del streaming (por ejemplo, SD, HD).  
     - **Número de dispositivos**: Cantidad de dispositivos permitidos para el plan.  
   - Presione **"Guardar"** para registrar el nuevo plan.

3. **Editar un plan**:  
   - En la lista de planes, haga clic en el botón **"Editar"** junto al plan que desea modificar.  
   - Realice los cambios necesarios y presione **"Guardar"**.

4. **Eliminar un plan**:  
   - En la lista de planes, haga clic en el botón **"Eliminar"** junto al plan que desea desactivar.  
   - El plan no se eliminará físicamente, sino que se marcará como inactivo.

---

#### **7. Cierre de Sesión**  
1. Seleccione la opción **"Cerrar sesión"**.  
2. Será redirigido a la pantalla de inicio de sesión.

---

#### **8. Preguntas Frecuentes**  

**¿Qué hago si no puedo iniciar sesión?**  
- Verifique que su usuario y contraseña sean correctos.  
- Restablezca su contraseña siguiendo los pasos de la sección 4.2.

**¿Cómo puedo cambiar mi contraseña?**  
1. Ingrese a **"Configuración"** en el menú.  
2. Seleccione **"Cambiar contraseña"**.  
3. Ingrese su contraseña actual y la nueva.  
4. Guarde los cambios.

**¿Cómo descargo reportes?**  
1. Acceda a la sección **"Reportes"**.  
2. Seleccione el tipo de informe.  
3. Haga clic en **"Generar Reporte"**.  
4. Descargue el archivo generado.

**¿Cómo puedo agregar contenido local?**  
1. Diríjase a la sección **"Gestión de Películas"**.  
2. Haga clic en **"Agregar Película"**.  
3. Complete los campos con la información del contenido local.  
4. Presione **"Guardar"** para registrar la película.

---

#### **9. Contacto y Soporte**  
Si tiene problemas con la aplicación, contacte al equipo de soporte:  
- **Correo electrónico**: soporte@cinesucre.com  
- **Teléfono**: +123 456 7890  

Este manual le ayudará a familiarizarse con el uso del sistema. Para dudas adicionales, consulte con el administrador de la plataforma.

---

#### **10. Tecnologías Utilizadas**  
- **Backend**: Flask (Python).  
- **Frontend**: HTML, CSS, JavaScript, Tailwind CSS 4.  
- **Base de Datos**: MySQL (Flask-SQLAlchemy).  
- **Control de Versiones**: Git/GitHub.  

---

#### **11. Limitaciones y Mejoras Futuras**  
- **Integración con pasarelas de pago**: En esta fase inicial, no se incluye la integración con pasarelas de pago como PayPal o Stripe.  
- **Aplicaciones móviles nativas**: La plataforma está diseñada para ser accesible a través de navegadores web, pero en el futuro se podrían desarrollar aplicaciones móviles nativas.  
- **Notificaciones en tiempo real**: No se implementó un sistema de notificaciones en tiempo real, pero es una mejora futura propuesta.  

---

Este manual le proporciona una guía detallada para utilizar el aplicativo web **Cine Sucre**. Para más información, consulte la documentación técnica o contacte al equipo de soporte.