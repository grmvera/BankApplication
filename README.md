# BankApplication

Este proyecto es una API RESTful desarrollada en Java con Spring Boot para la gestión de clientes, cuentas y transacciones bancarias. Forma parte de un reto técnico de microservicios.

## Características

- Gestión de *Personas, **Clientes, **Cuentas* y *Transacciones*
- Endpoints CRUD para cada entidad
- Registro de movimientos y actualización automática de saldo
- Control de saldo insuficiente
- Reporte de estado de cuenta por cliente y rango de fechas
- Pruebas unitarias e integración incluidas

## Estructura de carpetas


BankApplication/
 ├── account/
 └── client/


Cada módulo es un microservicio independiente con su propio pom.xml.

## Ejecución

Desde la raíz del proyecto, puedes ejecutar los microservicios usando Maven:

bash
cd account
./mvnw spring-boot:run

cd ../client
./mvnw spring-boot:run


## Pruebas

Para ejecutar las pruebas unitarias:

bash
cd account
./mvnw test

cd ../client
./mvnw test


## Endpoints principales

- /api/clients - CRUD de clientes
- /api/accounts - CRUD de cuentas
- /api/transactions - CRUD de transacciones
- /api/transactions/clients/{clientId}/report?dateTransactionStart=fecha&dateTransactionEnd=fecha - Reporte de estado de cuenta

## Autor

Reto técnico Backend Developer Spring
