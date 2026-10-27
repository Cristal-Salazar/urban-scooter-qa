# Validación de campos | Urban Scooter

**Proyecto:** Urban Scooter  
**Área:** Pruebas funcionales web  
**Técnicas:** Clases de equivalencia y análisis de valores límite

## Objetivo

Verificar que los campos del formulario acepten los datos permitidos y rechacen los valores que no cumplen con los requisitos establecidos.

## 1. Campo Nombre

**Requisito:** longitud de 2 a 15 caracteres.

| Clase de equivalencia | Dato de prueba | Resultado |
|---|---|---|
| Longitud válida | Anna | APROBADO |
| Longitud inferior al mínimo | A | APROBADO |
| Longitud superior al máximo | Alexanderthegreat | APROBADO |
| Caracteres válidos | Anna Marie, Anna-Maria | APROBADO |
| Caracteres inválidos | Anna123, @nna | APROBADO |

## 2. Campo Apellido

**Requisito:** longitud de 2 a 15 caracteres.

| Clase de equivalencia | Dato de prueba | Resultado |
|---|---|---|
| Longitud válida | Smith | APROBADO |
| Longitud inferior al mínimo | S | APROBADO |
| Longitud superior al máximo | MontgomeryRivera | NO APROBADO |
| Caracteres válidos | Smith Jones, Smith-Jones | APROBADO |
| Caracteres inválidos | Smith123, @Smith | APROBADO |

### Defecto identificado

Durante la validación del campo Apellido, la comprobación de una longitud superior al máximo permitido obtuvo un resultado **NO APROBADO**.

**Reporte de defecto:** KAN-17, documentado en Jira.

Esta incidencia muestra la importancia de comprobar los valores que se encuentran fuera de los límites definidos en los requisitos.

## 3. Campo Dirección

**Requisito:** longitud de 5 a 50 caracteres.

| Clase de equivalencia | Dato de prueba | Resultado |
|---|---|---|
| Longitud válida | Main St 45 | APROBADO |
| Longitud inferior al mínimo | Ab1 | APROBADO |
| Longitud superior al máximo | 123456789012345678901234567890123456789012345678901 | APROBADO |
| Caracteres válidos | Main-St. 45, LA | APROBADO |
| Caracteres inválidos | Main@Street#45 | APROBADO |

## Técnicas aplicadas

**Clases de equivalencia:** agrupación de datos válidos e inválidos para seleccionar valores representativos.

**Análisis de valores límite:** comprobación de los valores cercanos a las longitudes mínimas y máximas permitidas.

## Aprendizaje

Esta actividad me permitió fortalecer mis habilidades para interpretar requisitos, diseñar pruebas positivas y negativas e identificar defectos relacionados con la validación de datos.

**Fuente:** Proyecto final de QA Engineer de TripleTen, hoja «Tarea 2 validación de datos».
