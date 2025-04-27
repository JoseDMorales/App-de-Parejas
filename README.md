# Instrucciones para Ejecutar y Probar el Frontend

Este documento proporciona los pasos necesarios para configurar, ejecutar y probar este proyecto de React en tu entorno local.

## Prerrequisitos

Antes de comenzar, asegúrate de tener instalado lo siguiente en tu sistema:

* **Node.js:** (Se recomienda la última versión LTS) Puedes descargarlo desde [https://nodejs.org/](https://nodejs.org/)
* **npm** o **yarn:** Estos son gestores de paquetes para JavaScript que vienen instalados con Node.js (npm) o puedes instalarlo por separado (yarn: [https://yarnpkg.com/](https://yarnpkg.com/)).

## Instalación de las Dependencias (node\_modules)

El directorio `node_modules` contiene todas las bibliotecas y dependencias de las que depende este proyecto. Para instalar estas dependencias, sigue estos pasos:

1.  **Navega al directorio del proyecto:** Abre tu terminal o línea de comandos y utiliza el comando `cd` para dirigirte a la carpeta raíz del proyecto React. Por ejemplo:

    ```bash
    cd nombre-del-proyecto
    ```

2.  **Instala las dependencias usando npm o yarn:**

    * **Con npm:** Ejecuta el siguiente comando:

        ```bash
        npm install
        ```

        Este comando leerá el archivo `package.json` ubicado en la raíz del proyecto y descargará e instalará todas las dependencias listadas en la carpeta `node_modules`.

    * **Con yarn:** Si prefieres usar yarn, asegúrate de tenerlo instalado y luego ejecuta el siguiente comando:

        ```bash
        yarn install
        ```

        Similar a `npm install`, este comando leerá el archivo `yarn.lock` (o `package.json` si no existe `yarn.lock`) e instalará las dependencias en la carpeta `node_modules`.

    La instalación puede tardar unos minutos dependiendo de la cantidad de dependencias y la velocidad de tu conexión a internet.

## Ejecución del Proyecto

Una vez que las dependencias se hayan instalado correctamente, puedes ejecutar el proyecto de React en tu entorno de desarrollo local.

1.  **Asegúrate de estar en el directorio raíz del proyecto** (donde se encuentra el archivo `package.json`).

2.  **Ejecuta el script de inicio:** La mayoría de los proyectos de React utilizan un script llamado `start` definido en el archivo `package.json`. Puedes ejecutarlo con npm o yarn:

    * **Con npm:**

        ```bash
        npm start
        ```

    * **Con yarn:**

        ```bash
        yarn start
        ```
Este comando generalmente inicia un servidor de desarrollo local y abre la aplicación en tu navegador web predeterminado. Por lo general, la aplicación estará disponible en una dirección como `http://localhost:3000`.

## Ejecución de las Pruebas

Es importante asegurarse de que la aplicación funcione correctamente ejecutando las pruebas unitarias, de integración o de componentes que se hayan implementado en el proyecto.

1.  **Asegúrate de estar en el directorio raíz del proyecto** (donde se encuentra el archivo `package.json`).

2.  **Ejecuta el script de prueba:** Al igual que con el script de inicio, los proyectos de React suelen tener un script de prueba definido en `package.json`. Puedes ejecutarlo con npm o yarn:

    * **Con npm:**

        ```bash
        npm test
        ```

    * **Con yarn:**

        ```bash
        yarn test
        ```

    Este comando generalmente ejecuta un entorno de prueba (como Jest o React Testing Library) y muestra los resultados de las pruebas en tu terminal. Puede que la ejecución de las pruebas también abra un navegador para mostrar la cobertura del código u otros informes.

## Notas Adicionales

* Si encuentras errores durante la instalación o ejecución, asegúrate de tener las versiones correctas de Node.js y npm/yarn instaladas. También puedes intentar eliminar la carpeta `node_modules` y el archivo `package-lock.json` (si usas npm) o `yarn.lock` (si usas yarn) y luego ejecutar `npm install` o `yarn install` nuevamente.
* Consulta el archivo `package.json` para ver los scripts disponibles (además de `start` y `test`, puede haber otros como `build`, `eject`, etc.).

¡Esperamos que esta guía te sea útil para poner en marcha este Frontend!

# Instrucciones para Ejecutar y Probar el Backend de Node.js

Este documento describe los pasos necesarios para configurar, ejecutar y probar las diferentes rutas de este proyecto de backend de Node.js en tu entorno local.

## Prerrequisitos

Antes de comenzar, asegúrate de tener instalado lo siguiente en tu sistema:

* **Node.js:** (Se recomienda la última versión LTS) Puedes descargarlo desde [https://nodejs.org/](https://nodejs.org/)
* **npm** o **yarn:** Estos son gestores de paquetes para JavaScript que vienen instalados con Node.js (npm) o puedes instalarlo por separado (yarn: [https://yarnpkg.com/](https://yarnpkg.com/)).
* **Postman** o **Insomnia:** (Recomendado) Estas herramientas te permiten realizar solicitudes HTTP a tus rutas del backend para probarlas. Puedes descargarlos desde sus respectivos sitios web. También puedes usar `curl` en la terminal si lo prefieres.

## Instalación de las Dependencias (node\_modules)

El directorio `node_modules` contiene todas las bibliotecas y dependencias de las que depende este proyecto. Para instalar estas dependencias, sigue estos pasos:

1.  **Navega al directorio del proyecto:** Abre tu terminal o línea de comandos y utiliza el comando `cd` para dirigirte a la carpeta raíz del proyecto de backend. Por ejemplo:

    ```bash
    cd nombre-del-proyecto-backend
    ```

2.  **Instala las dependencias usando npm o yarn:**

    * **Con npm:** Ejecuta el siguiente comando:

        ```bash
        npm install
        ```

        Este comando leerá el archivo `package.json` ubicado en la raíz del proyecto y descargará e instalará todas las dependencias listadas en la carpeta `node_modules`.

    * **Con yarn:** Si prefieres usar yarn, asegúrate de tenerlo instalado y luego ejecuta el siguiente comando:

        ```bash
        yarn install
        ```

        Similar a `npm install`, este comando leerá el archivo `yarn.lock` (o `package.json` si no existe `yarn.lock`) e instalará las dependencias en la carpeta `node_modules`.

    La instalación puede tardar unos minutos dependiendo de la cantidad de dependencias y la velocidad de tu conexión a internet.

## Ejecución del Servidor Backend

Una vez que las dependencias se hayan instalado correctamente, puedes ejecutar el servidor backend de Node.js en tu entorno de desarrollo local.

1.  **Asegúrate de estar en el directorio raíz del proyecto** (donde se encuentra el archivo `package.json`).

2.  **Ejecuta el script de inicio:** La mayoría de los proyectos de Node.js tienen un script para iniciar el servidor definido en el archivo `package.json` (normalmente llamado `start` o `dev` para desarrollo). Puedes ejecutarlo con npm o yarn:

    * **Con npm:**

        ```bash
        npm start
        # o posiblemente
        npm run dev
        ```

    * **Con yarn:**

        ```bash
        yarn start
        # o posiblemente
        yarn dev
        ```

    Este comando ejecutará el script definido en `package.json`, que generalmente inicia tu servidor backend. Revisa la salida en tu terminal para ver en qué puerto está escuchando el servidor (por ejemplo, `Servidor escuchando en el puerto 3000`).

## Prueba de las Rutas de la API

Una vez que el servidor esté en funcionamiento, puedes probar las diferentes rutas de la API utilizando Postman, Insomnia o `curl`. A continuación, se describen las rutas definidas en el archivo `router.js` y cómo probarlas:

**Nota:** Asumimos que tu servidor base está corriendo en `http://localhost:3000` (o el puerto que hayas configurado). Ajusta las URLs según sea necesario.

1.  **`POST /request-reset`**: Solicitar restablecimiento de contraseña.
    * **Método:** `POST`
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con la información necesaria para identificar al usuario que solicita el restablecimiento (por ejemplo, `{"email": "usuario@ejemplo.com"}`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/request-reset` y configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa el JSON necesario y envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"email": "usuario@ejemplo.com"}' http://localhost:3000/request-reset
        ```

2.  **`POST /reset-password`**: Restablecer la contraseña.
    * **Método:** `POST`
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con el token de restablecimiento y la nueva contraseña (por ejemplo, `{"token": "alguntoken", "newPassword": "nuevaContraseña123"}`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/reset-password` y configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa el JSON necesario y envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"token": "alguntoken", "newPassword": "nuevaContraseña123"}' http://localhost:3000/reset-password
        ```

3.  **`POST /register`**: Registrar un nuevo usuario.
    * **Método:** `POST`
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con la información del nuevo usuario (definido por tu `registerSchema`, por ejemplo, `{"username": "nuevoUsuario", "email": "nuevo@ejemplo.com", "password": "contraseñaSegura"}`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/register` y configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa el JSON necesario y envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"username": "nuevoUsuario", "email": "nuevo@ejemplo.com", "password": "contraseñaSegura"}' http://localhost:3000/register
        ```

4.  **`POST /login`**: Iniciar sesión de un usuario existente.
    * **Método:** `POST`
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con las credenciales del usuario (definido por tu `loginSchema`, por ejemplo, `{"email": "usuario@ejemplo.com", "password": "contraseña"}`). La respuesta exitosa generalmente incluirá un token de autenticación.
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/login` y configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa las credenciales y envía la solicitud. Guarda el token recibido para usarlo en las rutas protegidas.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"email": "usuario@ejemplo.com", "password": "contraseña"}' http://localhost:3000/login
        ```

5.  **`POST /logout`**: Cerrar sesión de un usuario.
    * **Método:** `POST`
    * **Cuerpo:** Generalmente no requiere un cuerpo. Puede depender de tu implementación (por ejemplo, enviar el token en el cuerpo o en las cookies).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/logout`. Si requiere un token, asegúrate de incluirlo en el cuerpo, encabezados o cookies según tu implementación.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST http://localhost:3000/logout
        # Si requiere un token en el encabezado:
        # curl -X POST -H "Authorization: Bearer <tu_token>" http://localhost:3000/logout
        ```

6.  **`POST /subscription`**: Crear una suscripción.
    * **Método:** `POST`
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con los detalles de la suscripción (los campos dependerán de tu lógica, por ejemplo, `{"userId": "algunaId", "plan": "premium"}`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `POST` a `http://localhost:3000/subscription` y configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa los detalles de la suscripción y envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"userId": "algunaId", "plan": "premium"}' http://localhost:3000/subscription
        ```

7.  **`PUT /updateUser`**: Actualizar la información del usuario.
    * **Método:** `PUT`
    * **Encabezado:** Requiere un token de autenticación válido en el encabezado (probablemente `Authorization: Bearer <tu_token>`).
    * **Cuerpo (JSON):** Necesitarás enviar un cuerpo JSON con los campos que deseas actualizar (por ejemplo, `{"name": "Nuevo Nombre", "email": "nuevoEmail@ejemplo.com"}`). El `user` que se pasa en el controlador `updateUser` probablemente se extrae del token verificado.
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `PUT` a `http://localhost:3000/updateUser`. En la sección de encabezados, agrega la clave `Authorization` con el valor `Bearer <tu_token>`. Configura el cuerpo de la solicitud como `raw` y formato `JSON`. Ingresa los campos a actualizar y envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X PUT -H "Content-Type: application/json" -H "Authorization: Bearer <tu_token>" -d '{"name": "Nuevo Nombre", "email": "nuevoEmail@ejemplo.com"}' http://localhost:3000/updateUser
        ```

8.  **`GET /profile`**: Obtener la información del perfil del usuario.
    * **Método:** `GET`
    * **Encabezado:** Requiere un token de autenticación válido en el encabezado (`Authorization: Bearer <tu_token>`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `GET` a `http://localhost:3000/profile`. En la sección de encabezados, agrega la clave `Authorization` con el valor `Bearer <tu_token>`. Envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X GET -H "Authorization: Bearer <tu_token>" http://localhost:3000/profile
        ```

9.  **`GET /check-subscription`**: Verificar el estado de la suscripción del usuario.
    * **Método:** `GET`
    * **Encabezado:** Requiere un token de autenticación válido en el encabezado (`Authorization: Bearer <tu_token>`).
    * **Prueba con Postman/Insomnia:** Crea una nueva solicitud `GET` a `http://localhost:3000/check-subscription`. En la sección de encabezados, agrega la clave `Authorization` con el valor `Bearer <tu_token>`. Envía la solicitud.
    * **Prueba con `curl`:**

        ```bash
        curl -X GET -H "Authorization: Bearer <tu_token>" http://localhost:3000/check-subscription
        ```

## Notas Adicionales

* Asegúrate de consultar cualquier documentación adicional o archivos de configuración (`.env`, etc.) para obtener información sobre variables de entorno, bases de datos u otras configuraciones específicas del proyecto.
* Si encuentras errores, revisa los logs del servidor en tu terminal para obtener más detalles sobre el problema.
* Es posible que algunas rutas requieran autenticación (como `/profile`, `/updateUser` y `/check-subscription`). Para probar estas rutas, primero deberás obtener un token de inicio de sesión exitoso a través de la ruta `/login` y luego incluir ese token en el encabezado de tus solicitudes (generalmente como `Authorization: Bearer <tu_token>`).

¡Esperamos que esta guía te sea útil para configurar y probar tu backend de Node.js!
