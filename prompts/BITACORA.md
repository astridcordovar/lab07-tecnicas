# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: (escribe aqui cual usaste)

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|------|-----------------|-------------------------|------------------------------------|
| Zero-shot | 5| Tabulación con valores Positivo, Negativo, Neutral | SI |
| One-shot | 5 | Lista con valores Positivo, Negativo, Neutral  | SI |
| Few-shot | 5 | Asignar con valores Positivo, Negativo, Neutral| SI |


## Ejercicio 3: Chain of Thought

| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|--------|--------------------|---------------------------|------------------|
| Directo | 318.60 | No | Si |
| Paso a paso | 318.60 | No | Si |

Es útil ver el razonamiento de la IA ya que podemos comprobar los pasos que sigue para obtener una respuesta y poder encontrar más fácil algún error.


## Ejercicio 4: Role prompting

| Version | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo | A quien le sirve mas |
|---------|-------------------------------|-----------------------|----------------------|
| A. Sin rol | | | |
| B. Rol docente | | | |
| C. Rol senior | | | |


## Ejercicio 5: Descomposicion
**Simple Prompt:** La IA devuelve una respuesta general, con una estructura básica de clases para luego ser evidenciado en un código de Java, todo en una misma respuesta.

**Descomposición Prompt**

**Paso 1** Lista 5 requisitos con sus detalles y objetivos. 

**Paso 2** Diseña las clases con sus atributos. 

**Paso 3** Escribe los códigos en Java, utilizando las clases. 

**Paso 4** Revisa y sugiere 3 mejoras concretas.


## Ejercicio 6: Prompt estructurado y autocritica
 
| Qué revisar	Cumple |  (Sí / No) |
|---------|--------------------------|
| ¿Tiene las 4 columnas pedidas?| Si | 	
| ¿Incluye el bloqueo después de 3 intentos? | Si | 	
| ¿Incluye casos con campos vacíos?| Si | 
| Indica qué casos agregó en la autocrítica? | Si | 	
| ¿Hay algún caso repetido o que no tenga sentido? | No | 
    
```text
<rol>Actua como analista de pruebas de software.</rol>
<contexto>Login web con correo y contrasena. La cuenta se bloquea
despues de 3 intentos fallidos.</contexto>
<tarea>Piensa paso a paso que puede fallar y escribe 6 casos de prueba.</tarea>
<formato>Tabla con las columnas: ID, escenario, datos de entrada,
resultado esperado.</formato>
Revisa tu tabla: faltan casos limite como campos vacios, correo sin @
o contrasena con espacios? Agrega los que falten e indica cuales agregaste.

```
