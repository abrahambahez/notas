# Básicos
Ya que estás [conectado a un clúster](https://www.freecodecamp.org/espanol/news/tutorial-de-mongodb-atlas-como-empezar/)

Conectarse a una base de datos
```mongo
use <database>
```

Comando base para usar métodos
```mongo
db.<colection>.<method>({<arguments>})
```

# Métodos CRUD

- Buscar
    - `.find({})`
    - `.findOne({})`
- Editar
    - `.updateOne({}, { $set: {} })`
- Eliminar
    - `deleteOne({})`
