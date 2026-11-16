# Tarea: Mi prompt avanzado

## Tarea elegida
Diseñar las clases de un sistema de notas.

## Version 1: prompt basico
```text
Diseñar las clases de un sistema de notas
```

**Prompt básico** Crea las clases necesarias y también me envía el código.

## Version 2
```text
Actua como un estudiante de Desarrollo de software y diseña las clases de un sistema de notas.
```

**Role prompting** Lista las clases, con el formato que cada clase, con sus métodos y atributos. Además envía un diagrama UML

## Version 3: prompt final
```text
<rol> Actúa como estudiante de diseño de software. </rol>
<contexto> Sistema de notas académicas con clases. </contexto>
<tarea> Revisa las clases, atributos, métodos. </tarea>
<formato> Presenta las clases modificadas, atributos, métodos en código de Java y diagrama UML </formato>

Autocrítica: Revisa si se contempló el retiro de un estudiante de un curso. Si falta, agrega los elementos necesarios para gestionar el retiro, conservar sus notas y controlar el estado de la matrícula.
```

**Prompt estructurado y autocrítica** Considera la mejora que propuse y edita las clases, además envía en código y un nuevo diagrama UML.

## Tecnicas usadas en el prompt final
| Técnica | Donse se aplicó |
|---------|-----------------|
|Role Prompting| Actúa como estudiante de diseño de software. |
|Prompt estructurado| <rol> Actúa como estudiante de diseño de software. </rol>
<contexto> Sistema de notas académicas con clases. </contexto>
<tarea> Revisa las clases, atributos, métodos. </tarea>
<formato> Presenta las clases modificadas, atributos, métodos en código de Java y diagrama UML </formato> | 
|Autocrítica| Revisa si se contempló el retiro de un estudiante de un curso. Si falta, agrega los elementos necesarios para gestionar el retiro, conservar sus notas y controlar el estado de la matrícula. |


## Evaluacion del resultado

## Por que elegi estas tecnicas
