# 📄 Requerimientos del Sistema

## 1. Sistema

* Nombre del sistema: Bankify
* Objetivo: gestionar de forma básica las cuentas bancarias de los clientes.

## 2. Problema a resolver
  No existe un sistema centralizado que realice:
  * Registrar cuentas bancarias de manera validada.
  * Consultar el saldo de una cuenta.
  * Realizar depósitos de dinero de forma controlada.
  * Generar reportes tributarios a los clientes en formato PDF.
  * Enviar reportes a la DIAN en formato JSON.

## 3. Diagrama de Contexto

### 3.1 Diagrama

![Diagrama de contexto](/docs/uml/diagramaContexto.png)

### 3.2 Actores

| Actor / Rol |          Descripción           |
|-------------|:------------------------------:|
| cliente     | Cliente del sistema de Bankify |
| Asesor      |  Empleado que guía al cliente  |
| Supervisor  | Empleado que revisa y gestiona la operación del sistema  |
|Gerente Financiero  | Empelado que revisa y gestiona las finanzas  |

### 3.3 Sistemas externos

| Sistema |                                           Descripción                                           |
|---------|:-----------------------------------------------------------------------------------------------:|
| DIAN    | Entidad pública encargado del registro y seguimiento de la actividad financiera de los clientes |
| Banco   |        Persona Juridica que emplea el sistema para gestionar las cuentas de los usuarios        |

## 4. Alcance del sistema

### 4.1 Dentro del sistema

* Registrar cuentas bancarias de forma válida
* Consultar los saldos del cliente
* Controlar los depositos de dinero
* Generar reportes tributarios al cliente (formato PDF)

### 4.2 Fuera del sistema

* Transferencias entre cuentas
* Retiros de dinero
* Integración con otros bancos