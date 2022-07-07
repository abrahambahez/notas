# Gestión de conocimiento
## Tipos de notas

### Referencias

Todas las notas que comienzan con el prefijo `@` representan notas de literatura.

Las que comienzan con el prefijo `+ ` son *memos*, referencias de estudio, cosas que no quiero olvidar, guías de herramientas, snippets de código, etc.

Las notas que tienen el patrón de fecha (`YYYY-MM-DD`) son mi *diario de trabajo*, que funciona como diario de campo y es exclusivo para el registro de observaciones, descripciones densas y registro de material empírico interesante.

Referencias de entidades particulares, nombres de personas, lugares, poblaciones, etc. deben empezar siempre con mayúscula, de modo que el query `file:/^[A-Z]/` con la opción `Match case` activa pueda filtrarlos. El query más exacto podría ser:

```
file:/^[A-Z].+\.md/ -path:Recursos
```

Las notas temporales son referencias que necesito sólo por un periodo específico y después perderán su valor (p.e. la bibliografía de un curso o el programa de una materia), comienzan con el prefijo `- `

### Notas permanentes

Algunas notas son registros, suelen ser las más generales o abstractas. Deberían vincular una lista curada de otras notas con más densidad de links que permitan caminos interesantes por la red.

### Notas de proyecto

Las notas de proyecto comienzan con el prefijo `~` y el *código del proyecto*, que es una secuencia breve de caracteres que pretende emular el nombre completo, pero no lo hace para poder referenciarla más fácilmente en las tareas asignadas a él. El nombre real del proyecto se encuentra siempre en el campo `aliases` de los metadatos.

Puede haber más de una nota de proyecto por proyecto en general. La nota sencilla (es decir, la que sólo tiene la forma `~PROYECTO`) debe contener el contexto y referir a las tareas asociadas, así como los recursos necesarios del proyecto. Habrá una nota del tipo `~PROYECTO index` para el índice de contenido y si el proyecto es largo, valdrá la pena usar varios *logs*

- log de cambios siguiendo la especificación de [*keep a changelog*](https://keepachangelog.com/en/1.0.0/)
    - En este caso, el log de cambios implica un log de **cambios de decisión**, que no rompen el software pero sí pueden romper el argumento
- log de decisiones siguiendo la especificaión de [madr](https://adr.github.io/madr/) (*markdown architectural decision records*) o de su variante, [adr](https://medium.com/olzzio/adr-any-decision-record-916d1b64b28d), *any decision record*

>Las notas de proyecto sólo pueden citar, pero nos ser citadas 

## Recursos

La carpeta Plantillas tiene las plantillas que ayudan a componer notas en Obsidian. La carpeta Archivo tiene notas de proyectos terminados y otras notas consideradas temporales (en el sentido de no relevantes en el presente) pero con suficiente valor histórico para guardarlas 

# Ágil

## Usa Kanban como metodología principal

Las reglas de Kanban deben seguirse:

- Definición de fases o pasos (en este caso)
- Visualizar el trabajo
- Definir lo hecho
- Limitar el trabajo
- Seguir el flujo (jalar)

## Kanban en Obsidian

- Describe los pasos y su definición de hecho en un comentario
- Usa el plugin de Kanban para visualizar
- Usa el plugin de recordatorios para establecer fechas
- Refiere al proyecto al que pertenece el item (a través de backlinks)
- Limita el trabajo en el nombre de la columna `(2)`
- Describe la acción correctamente en cada item, añade más si es necesario (`<br>`)

### Sintaxis de tareas

Ejemplo de [todo-md](https://github.com/todo-md/todo.md)

`- Work on the website ~3d #feat @john 2020-03-20`

Prototipo inicial:

`VERBO + OBJETO [[p; NOM. PROYECTO]] @{FECHA} @@{HORA} <br> DESCRIPCIÓN DETALLADA`
