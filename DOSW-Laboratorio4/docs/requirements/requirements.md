
# 📄 Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema de Bankify tiene los siguientes requerimientos (descripción a alto nivel):

### 1.1 Requerimientos funcionales

El sistema de Bankify debe tener la capacidad de:

1. Permitir la autenticación de usuarios mediante usuario y contraseña.
2. Permitir la gestión de clientes, por roles autorizados. (crear, activar, desactivar y actualizar).
3. Permitir la consulta del saldo de una cuenta bancaria por parte del cliente propietario.
4. Permitir realizar depósitos a cuentas bancarias activas.
5. Permitir la gestión de cuentas bancarias. (crear, activar, desactivar y actualizar).

### 1.2 Requerimientos no funcionales

El sistema de Bankify debe tener:

1. Validación de que los dos primeros dígitos correspondan a un banco registrado.
2. Validación estricta de que los números de cuenta tengan exactamente 10 dígitos.
3. Validación estricta de que los números de cuenta solo tengan carácteres númericos.
4. El sistema debe garantizar consistencia en las transacciones financieras.
5. El estilo de la interfaz corresponda a la identidad del banco.

## 2. Diagramas de caso de uso

### 2.1 Requerimiento Funcional 1

| Campo | Descripción |
|------|-------------|
| **ID** | RF-01 |
| **Nombre del requerimiento** | Autenticación de usurario |
| **Descripción** | *El sistema debe permitir a los usuarios autenticarse mediante usuario y contraseña válidos.* |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, Bankify debe tener previamente usuarios registrados en el sistema.* |
| **Actor** | *Cliente/Asesor/Supervisor/Gerente Financiero* |
| **Flujo principal** | 1. El actor ingresa usuario y contraseña.<br>2. El sistema valida las credenciales.<br>3. El sistema da el acceso al módulo correspondiente.|
| **Diagrama de caso de uso** | ![diagramaCasoDeUso1](/DOSW-Laboratorio4/docs/uml/diagramaCasoDeUso1.png) |
| **Poscondiciones** | *Se espera como resultado la autenticación y que el usuario pueda acceder a las funciones autorizadas.* |


### 2.2 Requerimiento Funcional 2

| Campo | Descripción |
|------|-------------|
| **ID** | RF-02 |
| **Nombre del requerimiento** | consultar saldo |
| **Descripción** | *El sistema debe permitir que el cliente pueda consultar su saldo* |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, Bankify debe asegurarse de que el ususario pueda autenticarse como cliente, también que la información del cliente este actualizada y que la cuenta del cliente esté activa* |
| **Actor** | *Cliente* |
| **Flujo principal** | 1. El actor selecciona la opción "consultar saldo" …<br>2. El sistema válida que la cuenta pertenezca al cliente y que esté activa <br>3. El sistema solicita ak servicio de base de datos la información requerida <br>4. El sistema carga una pantalla con la información solicitada |
| **Diagrama de caso de uso** | ![diageamaCasoDeUso2](/docs/uml/diagramaCasoDeUso2.png) |
| **Poscondiciones** | *Se esperá como resultado que el cliente conozca su saldo actualizado * |

### 2.3 Requerimiento Funcional 3

| Campo | Descripción |
|------|-------------|
| **ID** | RF-03 |
| **Nombre del requerimiento** | |
| **Descripción** | *El sistema debe …* |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, Bankify debe tener previamente …* |
| **Actor** | *(El actor debe estar definido en el diagrama de contexto)* |
| **Flujo principal** | 1. El actor …<br>2. El sistema …<br>3. El sistema … |
| **Diagrama de caso de uso** | *imagen y link*|
| **Poscondiciones** | *Se espera como resultado …* |

## 3. Preguntas
### a. ¿Identifica algún requerimiento que deba detallarse más? ¿cuál(es)? <br>

Si, los requerimientos con la generación de reportes tributarios requieren mayor detalle, especialmente en cuanto a la estructura y normativas exigidas por la DIAN.

### b. ¿Existen requerimientos que se contradigan entre sí? ¿cuál(es)? <br>

No se indentifican contradicciones.

### c. Si tuviera que dar una prioridad a los requerimientos, ¿cuáles deberían ser los 2 más importantes que deberían implementarse en una primera iteración del proyecto? <br>

 1. Autenticación de usuarios.
 2. Gestión y validación de las cuentas bancarias.

### d. ¿Existe algún requerimiento que no debería realizarse? <br>

No, todos los requerimientos aportan valor a la empresa.



