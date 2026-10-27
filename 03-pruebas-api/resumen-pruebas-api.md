# 🔌 Resultados de pruebas API REST | Urban Scooter

**Proyecto:** Urban Scooter  
**Tipo de pruebas:** API Testing  
**Herramienta:** Postman  
**Proyecto académico:** QA Engineer – TripleTen

## Objetivo

Validar el comportamiento de la API REST de Urban Scooter mediante solicitudes HTTP, verificando el cumplimiento de los requisitos funcionales y la gestión adecuada de datos válidos e inválidos.

## Funcionalidades evaluadas

| Área | Comprobaciones realizadas |
|---|---|
| Creación de repartidores | Validación de campos login, firstName y password |
| Autenticación | Inicio de sesión con credenciales válidas e inválidas |
| Eliminación de repartidores | Eliminación mediante identificador |
| Creación de pedidos | Validación de datos y generación del número de seguimiento |
| Búsqueda de pedidos | Consultas mediante número de seguimiento |
| Aceptación de pedidos | Asignación de pedidos a repartidores |
| Cancelación de pedidos | Cancelación y comprobación del estado |
| Finalización de pedidos | Finalización y comprobación del estado |
| Obtención de pedidos | Filtros por estación, repartidor y paginación |
| Pedidos completados | Consulta de cantidades de pedidos completados |
| Estados de pedidos | Validación de estados y reglas de prioridad |
| Funcionamiento del backend | Comprobación de disponibilidad y respuesta HTTP 200 |
| Estaciones de metro | Búsquedas con coincidencias y sin resultados |

## Ejemplo 1. Creación de repartidores

**Método HTTP:** POST  
**Endpoint:** `/api/v1/courier`

### Pruebas positivas

Se comprobaron solicitudes con datos válidos para los campos:

- `login`: longitudes válidas de 2, 5 y 10 letras latinas.
- `firstName`: longitudes válidas de 2, 5 y 10 letras latinas.
- `password`: exactamente 4 números enteros.

Los escenarios anteriores obtuvieron resultados APROBADOS.

### Pruebas negativas

Se evaluaron entradas fuera de los requisitos establecidos, incluyendo:

- Longitudes inválidas en `login`.
- Caracteres numéricos en `login`.
- Longitudes inválidas en `firstName`.
- Caracteres numéricos y especiales en `firstName`.
- Contraseñas con longitudes y tipos de caracteres inválidos.

Varios escenarios obtuvieron resultados NO APROBADOS, por lo que se documentaron incidencias.

## Ejemplo 2. Gestión de pedidos

Se realizaron pruebas relacionadas con:

- Creación de pedidos con datos válidos.
- Consulta de pedidos mediante su número de seguimiento.
- Aceptación de pedidos por repartidores.
- Cancelación de pedidos.
- Finalización de pedidos.
- Consulta de pedidos mediante filtros y paginación.

Se identificaron resultados NO APROBADOS en algunas comprobaciones de estados y operaciones de pedidos.

## Ejemplo 3. Validación de estados

Se comprobaron diferentes estados de los pedidos:

- `0`: pedido creado.
- `1`: pedido aceptado.
- `-1`: pedido cancelado.
- `2`: pedido completado.

También se realizaron comprobaciones de prioridad cuando se presentan varias condiciones de estado.

Algunos escenarios relacionados con la cancelación y la prioridad de estados obtuvieron resultados NO APROBADOS.

## Técnicas aplicadas

- Análisis de requisitos funcionales.
- Diseño de pruebas positivas y negativas.
- Clases de equivalencia.
- Análisis de valores límite.
- Validación de solicitudes y respuestas HTTP.
- Comprobación de datos obligatorios y opcionales.
- Identificación y documentación de defectos.

## Herramientas

**Postman:** envío de solicitudes HTTP y revisión de respuestas.

**Jira:** documentación y seguimiento de defectos identificados.

## Fuente

Tarea 4 del proyecto final de QA Engineer de TripleTen.

Este documento presenta un resumen de las funcionalidades evaluadas y los resultados observados durante las pruebas de API REST.
