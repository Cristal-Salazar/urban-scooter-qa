# 📱 Resultados de pruebas móviles | Urban Scooter

**Proyecto:** Urban Scooter  
**Aplicación:** Android para repartidores  
**Herramienta:** Android Studio  
**Entorno documentado:** Emulador Android 9.0  
**Tipo de pruebas:** Funcionales móviles

## Objetivo

Verificar funcionalidades de la aplicación móvil de repartidores de Urban Scooter mediante el diseño y ejecución de casos de prueba basados en los requisitos establecidos.

## Resumen de ejecución

Se documentaron 16 casos de prueba:

- **11 APROBADOS**
- **3 NO APROBADOS**
- **2 BLOQUEADOS**

## Casos de prueba y resultados

| ID | Caso de prueba | Resultado |
|---|---|---|
| 1 | Aceptación del pedido | APROBADO |
| 2 | Inicio de sesión exitoso | APROBADO |
| 3 | Recuperación de contraseña | APROBADO |
| 4 | Validación del campo Iniciar sesión | NO APROBADO |
| 5 | Validación del campo Contraseña | NO APROBADO |
| 6 | Cambio entre las pestañas «Todos los pedidos» y «Mis pedidos» | APROBADO |
| 7 | Cambio de tarjeta corta a tarjeta completa | APROBADO |
| 8 | Completar un pedido | APROBADO |
| 9 | Visualización de pedido aceptado en «Mis pedidos» | APROBADO |
| 10 | Notificación de falta de acceso a Internet | APROBADO |
| 11 | Recepción de notificación de pedido próximo a vencer | NO APROBADO |
| 12 | Contenido de la notificación de pedido próximo a vencer | BLOQUEADO |
| 13 | Navegación desde una notificación a la pestaña «Mis pedidos» | BLOQUEADO |
| 14 | Visualización del mensaje «Sin acceso a Internet» | APROBADO |
| 15 | Cierre de la ventana «Sin acceso a Internet» mediante el botón «Aceptar» | APROBADO |
| 16 | Reaparición del mensaje «Sin acceso a Internet» cuando la conexión no está disponible | APROBADO |

## Hallazgos relevantes

### Validación de credenciales

Los casos 4 y 5 obtuvieron resultados NO APROBADOS durante las pruebas de validación de los campos de inicio de sesión y contraseña.

### Notificaciones

El caso 11, relacionado con la recepción de notificaciones de pedidos próximos a vencer, obtuvo un resultado NO APROBADO.

Los casos 12 y 13 quedaron BLOQUEADOS, por lo que no se registraron como aprobados ni como fallidos.

## Habilidades aplicadas

- Diseño y ejecución de casos de prueba funcionales.
- Definición de precondiciones y pasos de prueba.
- Validación de autenticación y gestión de pedidos.
- Pruebas de notificaciones y conectividad.
- Comparación de resultados esperados y obtenidos.
- Registro de pruebas aprobadas, no aprobadas y bloqueadas.

## Fuente

Proyecto final de QA Engineer de TripleTen, Tarea 3: pruebas de aplicaciones móviles.

Este documento resume los resultados registrados en la hoja original de casos de prueba.
