# release-plugin-test

## Goals

Para comprobar como quedaría un **release:prepare** usamos la opcion **-DdryRun=true**

```
mvn release:prepare -DdryRun=true
```

Eliminar release:

```
mvn release:clean
```

En caso de haber pusheado ya el release y querer deshacerlo, siempre y cuando no hayamos ya hecho un **release:clean**:

```
mvn release:rollback
```

Para que se actualizen las versiones de los hijos y no tener que estar confirmando una por una:

```
mvn release:prepare -DautoVersionSubmodules=true
```
