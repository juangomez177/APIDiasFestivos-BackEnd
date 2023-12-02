# API - SpringBoot Días Festivos
### Por Juan José Gomez Mejia

Aplicación básica, basada en solicitudes http para calcular y consultar días festivos.
### Obtiene todos los festivos de la Base de Datos.
```
http://localhost:8080/festivos/get
```

### Verifica si es festivo para una fecha específica, (En tiempo de Ejecución).
```
http://localhost:8080/festivos/verificar/{año}/{mes}/{dia}
```

### Verifica si es festivo para una fecha específica, de la Base de Datos.
```
http://localhost:8080/festivos/verificarbd/{año}/{mes}/{dia}
```

### Obtiene todos los festivos de un año específico, sin guardar.
```
http://localhost:8080/festivos/obtener/{año}
```

### Guarda todos los festivos de un año específico, en la Base de datos.
```
http://localhost:8080/festivos/guardar/{año}
```
Se garantiza que los Festivos Base (Los que no tienen año, ya que se basan para el cálculo de los festivos de cada año), nunca serán modificados. Por lo tanto, se creará la columna "año" automáticamente en la Base de Datos para poder guardar los festivos correspondientes a cada año, y se valida el no guardar festivos que son iguales.