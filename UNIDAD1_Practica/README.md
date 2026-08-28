# UNIDAD 1 - Práctica de Linux

En esta práctica se utilizaron diferentes comandos de Linux para trabajar con directorios, archivos, historial de comandos y alias.

## 1. Creación de la estructura de directorios

Se creó la carpeta `proyectos` con los subdirectorios `web` y `movil` utilizando el comando `mkdir`. También se creó el archivo `index.html` dentro de la carpeta `web` mediante el comando `touch`.

![Creación de directorios](Screenshot%202026-08-28%20092639.png)

## 2. Creación del archivo notas.txt

Se creó el archivo `notas.txt` dentro del directorio `proyectos/movil` utilizando el comando `touch`. Posteriormente, se editó con `nano` y se verificó su contenido mediante `cat`.

![Creación de notas.txt](Screenshot%202026-08-28%20093127.png)

## 3. Creación del alias ir_notas

Se creó el alias `ir_notas` para acceder directamente al directorio `proyectos/movil` desde otra ubicación. Se comprobó su funcionamiento con `pwd` y `ls`, verificando que el directorio contiene el archivo `notas.txt`.

![Alias ir_notas](Screenshot%202026-08-28%20093205.png)

## 4. Consulta y filtrado del historial de comandos

Se utilizó `history 5` para consultar los últimos cinco comandos ejecutados. Posteriormente, se combinó `history` con `grep` para filtrar y mostrar únicamente los comandos que contienen la palabra `touch`.

![Historial y grep](Screenshot%202026-08-28%20093252.png)

## 5. Eliminación del historial de comandos

Se utilizó el comando `history -c` para limpiar el historial de comandos de la sesión. Posteriormente, se ejecutó `history` para comprobar que los registros anteriores habían sido eliminados.

![Eliminación del historial](Screenshot%202026-08-28%20093317.png)

## 6. Repetición del último comando con !!

Se utilizó `!!` para ejecutar nuevamente el último comando ingresado en la terminal. En este caso, se repitió el comando `pwd`, mostrando nuevamente la ruta del directorio actual.

![Uso de doble exclamación](Screenshot%202026-08-28%20093341.png)

## 7. Preservación del historial de comandos

Se utilizó `history -a` para guardar los comandos recientes de la sesión en el archivo `.bash_history`. Posteriormente, se verificó la existencia del archivo y se visualizaron sus últimos registros mediante `tail`.

![Preservación del historial](Screenshot%202026-08-28%20093412.png)

## 8. Creación del alias respaldo

Se creó el alias `respaldo` para generar automáticamente un directorio con el mismo nombre. Después de ejecutar el alias, se utilizó `ls` para comprobar que la carpeta `respaldo` fue creada correctamente.

![Alias respaldo](Screenshot%202026-08-28%20093442.png)

## 9. Creación del archivo log.txt

Se ingresó al directorio `respaldo` y se creó el archivo `log.txt` utilizando `touch`. Posteriormente, se editó con `nano` para agregar la palabra `OK` y se verificó su contenido mediante `cat`.

![Creación de log.txt](Screenshot%202026-08-28%20093512.png)

## 10. Creación del alias error

Se creó el alias `error` para agregar la palabra `Error` al archivo `log.txt` mediante el operador de redirección `>>`, conservando el contenido existente. Después se ejecutó el alias y se verificó el resultado con `cat`.

![Alias error](Screenshot%202026-08-28%20093539.png)

## 11. Creación del alias wiper

Se creó el alias `wiper` para eliminar el directorio `respaldo` junto con su contenido. Se utilizó `ls` antes y después de ejecutar el alias para comprobar que la carpeta fue eliminada correctamente.

![Alias wiper](Screenshot%202026-08-28%20093616.png)
