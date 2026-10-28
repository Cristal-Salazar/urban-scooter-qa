# 🔌 Prueba API REST | Creación de repartidor

**Proyecto:** Urban Scooter  
**Herramienta:** Postman  
**Método HTTP:** POST  
**Endpoint:** `/api/v1/courier`  
**Tipo de prueba:** Positiva  
**Resultado:** APROBADO

## Objetivo

Verificar que la API REST de Urban Scooter permita crear un repartidor utilizando datos válidos y devuelva una respuesta exitosa.

## Datos enviados

**Body (JSON):**

```json
{
  "login": "qaTest",
  "password": "1234",
  "firstName": "Cristal"
}
```

Los valores utilizados cumplen con las condiciones de longitud y formato documentadas para los campos evaluados.

## Resultado esperado

La API debe procesar correctamente la solicitud de creación y devolver el código HTTP `201 Created`.

## Resultado obtenido

**Código HTTP:** `201 Created`

**Tiempo de respuesta:** `3.02 s`

**Response Body:**

```json
{
  "ok": true
}
```

## Análisis QA

La respuesta obtenida coincide con el resultado esperado para una solicitud válida.

El código HTTP 201 indica que el servidor procesó exitosamente la creación del recurso, mientras que el campo `ok: true` confirma el resultado positivo de la operación.

## Técnicas y habilidades demostradas

- Construcción de solicitudes HTTP POST.
- Envío de datos en formato JSON.
- Validación de códigos de estado HTTP.
- Análisis de respuestas del servidor.
- Ejecución de pruebas positivas con Postman.

## Evidencia

Prueba ejecutada en Postman utilizando el entorno de Urban Scooter proporcionado por TripleTen.

**Resultado final:** APROBADO.
