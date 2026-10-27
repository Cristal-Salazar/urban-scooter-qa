# 🐞 Bug Report KAN-17 | Validación del campo Apellido

**Proyecto:** Urban Scooter  
**Área:** Aplicación web  
**Tipo de prueba:** Validación de campos  
**Técnica:** Análisis de valores límite  
**Herramienta de seguimiento:** Jira  
**Identificador:** KAN-17

## Descripción del defecto

El campo «Apellido» permite ingresar más de 15 caracteres sin mostrar el error de validación esperado.

## Precondiciones

- La aplicación web de Urban Scooter está disponible.
- El usuario se encuentra en el formulario de creación de un pedido.

## Pasos para reproducir

1. Abrir la aplicación web de Urban Scooter.
2. Ir al formulario para crear un pedido.
3. Localizar el campo «Apellido».
4. Introducir un apellido de más de 15 caracteres.
5. Quitar el foco del campo.
6. Observar el comportamiento del campo «Apellido».

## Resultado esperado

El campo «Apellido» debe aceptar entre 2 y 15 caracteres.

Al introducir más de 15 caracteres, la aplicación debe mostrar un error de validación.

## Resultado real

Al introducir un apellido de más de 15 caracteres, la aplicación no muestra el error de validación esperado.

## Análisis QA

El defecto fue identificado al comprobar un valor fuera del límite máximo permitido para el campo.

Este caso demuestra la aplicación del análisis de valores límite para detectar incumplimientos de los requisitos funcionales.

## Evidencia

Reporte documentado en Jira con el identificador KAN-17, durante el proyecto final de QA Engineer de TripleTen.
