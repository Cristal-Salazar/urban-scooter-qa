# 🐞 Pruebas móviles | Validación de inicio de sesión

**Proyecto:** Urban Scooter  
**Aplicación:** Android para repartidores  
**Casos de prueba relacionados:** 4 y 5  
**Resultado:** NO APROBADO  
**Herramientas:** Android Studio y Jira  
**Entorno:** Android Emulator Tripleten_2 — Android 9 / API 28

## Objetivo

Verificar que la aplicación muestre un mensaje de validación adecuado cuando un repartidor intenta iniciar sesión con credenciales incorrectas.

## Descripción del defecto

Al intentar iniciar sesión con credenciales inválidas, Urban Scooter muestra el mensaje `HTTP 404 Not Found` en lugar del mensaje de validación esperado.

## Precondiciones

- La aplicación Urban Scooter está instalada y abierta.
- El servidor está activo.
- La URL del backend está configurada correctamente.
- Existe el repartidor `cristalqa`.

## Escenario 1. Usuario inválido — Caso 4

**Pasos para reproducir:**

1. Abrir Urban Scooter.
2. Introducir un usuario inválido en el campo de inicio de sesión.
3. Introducir una contraseña.
4. Pulsar «Iniciar sesión».

## Escenario 2. Contraseña incorrecta — Caso 5

**Pasos para reproducir:**

1. Introducir el usuario válido `cristalqa`.
2. Introducir una contraseña incorrecta.
3. Pulsar «Iniciar sesión».

## Resultado esperado

La aplicación debe mostrar el mensaje:

**«Usuario o contraseña no válido»**

El usuario debe permanecer en la pantalla de inicio de sesión.

## Resultado real

En ambos escenarios, la aplicación muestra:

**`HTTP 404 Not Found`**

## Análisis QA

Las pruebas permitieron identificar un comportamiento diferente al especificado en los requisitos de autenticación.

El defecto afecta la información presentada al usuario cuando introduce credenciales inválidas.

La evidencia corresponde a dos escenarios de prueba relacionados con la validación de credenciales.

## Evidencia original

Defecto documentado en Jira durante la Tarea 3 del proyecto final de QA Engineer de TripleTen.

**Casos asociados:** 4 y 5.
