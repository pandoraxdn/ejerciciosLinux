### Ejercicios con `sed`

1. **Reemplazo simple**: Crea un archivo llamado `texto.txt` con el contenido:
   ```
   Hola mundo
   Bienvenido al curso
   ```
   Usa `sed` para reemplazar "mundo" por "universo".

2. **Eliminar líneas**: Dado un archivo `datos.txt` con el siguiente contenido:
   ```
   Línea 1
   Línea 2
   Línea 3
   ```
   Elimina la segunda línea usando `sed`.

3. **Insertar líneas**: Crea un archivo `notas.txt` con:
   ```
   Nota 1
   Nota 2
   ```
   Usa `sed` para insertar "Importante" antes de la segunda línea.

4. **Cambiar el formato**: Dado un archivo `emails.txt` con:
   ```
   user1@example.com
   user2@example.com
   ```
   Usa `sed` para cambiar el dominio de todos los correos a `newdomain.com`.

5. **Eliminar comentarios**: Crea un archivo `config.txt` con:
   ```
   # Este es un comentario
   clave=valor
   # Otro comentario
   ```
   Usa `sed` para eliminar las líneas que comienzan con `#`.

### Ejercicios con `awk`

6. **Contar palabras**: Dado un archivo `texto.txt` con varias líneas de texto, usa `awk` para contar el número total de palabras.

7. **Filtrar columnas**: Crea un archivo `estudiantes.txt` con:
   ```
   Juan 23
   Ana 20
   Pedro 22
   ```
   Usa `awk` para mostrar solo los nombres.

8. **Calcular promedios**: Dado un archivo `calificaciones.txt`:
   ```
   Matemáticas 90
   Física 80
   Química 85
   ```
   Usa `awk` para calcular el promedio de las calificaciones.

9. **Buscar coincidencias**: Crea un archivo `datos.txt` con:
   ```
   perro
   gato
   pez
   ```
   Usa `awk` para encontrar líneas que contengan la letra "e".

10. **Agrupar datos**: Dado un archivo `ventas.txt` con:
    ```
    ProductoA 10
    ProductoB 15
    ProductoA 20
    ```
    Usa `awk` para sumar las ventas por producto.

### Ejercicios combinando `sed`, `awk` y `cut`

11. **Filtrar y procesar**: Crea un archivo `informacion.txt` con:
    ```
    1,Juan,23
    2,Ana,20
    ```
    Usa `cut` para extraer solo los nombres y `awk` para imprimir cada nombre en mayúsculas.

12. **Reformatear datos**: Dado un archivo `registro.txt`:
    ```
    Juan;23
    Ana;20
    ```
    Usa `cut` para separar los nombres de las edades y `sed` para reemplazar `;` por `:`.

13. **Sumar columnas**: Crea un archivo `numeros.txt`:
    ```
    1 2
    3 4
    5 6
    ```
    Usa `awk` para sumar la primera columna y `cut` para extraer los números.

14. **Buscar y reemplazar**: Dado un archivo `frutas.txt`:
    ```
    manzana
    naranja
    plátano
    ```
    Usa `sed` para reemplazar "naranja" por "limón" y `awk` para contar las líneas.

15. **Contar caracteres**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar el número total de caracteres.

### Ejercicios con `cut`

16. **Extraer campos**: Crea un archivo `data.txt` con:
    ```
    nombre1;apellido1;edad1
    nombre2;apellido2;edad2
    ```
    Usa `cut` para extraer solo los apellidos.

17. **Filtrar texto**: Dado un archivo `cursos.txt`:
    ```
    Curso1;10
    Curso2;15
    ```
    Usa `cut` para extraer solo los nombres de los cursos.

18. **Contar líneas**: Crea un archivo `info.txt` con varias líneas. Usa `cut` junto con `wc` para contar el número de líneas.

19. **Filtrar por longitud**: Dado un archivo `nombres.txt` con:
    ```
    Juan
    Ana
    Pedro
    ```
    Usa `cut` para mostrar nombres que tengan más de 3 letras.

20. **Concatenar campos**: Crea un archivo `empleados.txt`:
    ```
    1;Juan;desarrollador
    2;Ana;diseñadora
    ```
    Usa `cut` para extraer solo los nombres y concatena con su respectiva posición.

### Ejercicios avanzados

21. **Reemplazar patrones complejos**: Crea un archivo `texto_complejo.txt`:
    ```
    $USER is logged in
    $USER has new messages
    ```
    Usa `sed` para reemplazar `$USER` por el nombre real de un usuario.

22. **Formatear salida**: Dado un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida en el formato "Nombre: Juan, Saldo: 1000".

23. **Eliminar duplicados**: Crea un archivo `lista.txt`:
    ```
    manzana
    plátano
    manzana
    ```
    Usa `sort` y `uniq` para eliminar duplicados y luego `awk` para contar los elementos únicos.

24. **Filtrar líneas con condición**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto3 50
    ```
    Usa `awk` para mostrar solo los productos con ventas superiores a 100.

25. **Agrupar y contar**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    B
    ```
    Usa `awk` para contar cuántas veces aparece cada producto.

26. **Modificar varios campos**: Dado un archivo `usuarios.txt`:
    ```
    Juan 23
    Ana 20
    ```
    Usa `awk` para sumar 5 años a cada edad y mostrar la salida.

27. **Reemplazo condicional**: Crea un archivo `notas.txt` con:
    ```
    1 5
    2 8
    3 3
    ```
    Usa `sed` para reemplazar notas menores a 5 por "Repetir".

28. **Contar y filtrar con `grep`**: Dado un archivo `textos.txt` con varias líneas, usa `grep` para contar cuántas líneas contienen la palabra "error".

29. **Modificar la estructura de datos**: Crea un archivo `equipos.txt`:
    ```
    EquipoA 5
    EquipoB 10
    EquipoC 8
    ```
    Usa `awk` para modificar el formato a "EquipoA tiene 5 jugadores".

30. **Extraer y contar**: Dado un archivo `datos.txt` con el siguiente contenido:
    ```
    1|Juan|20
    2|Ana|25
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

### Más ejercicios

31. **Reemplazo con patrón**: Crea un archivo `mensajes.txt`:
    ```
    Hola, [nombre]
    Adiós, [nombre]
    ```
    Usa `sed` para reemplazar `[nombre]` por un nombre específico.

32. **Sumar por categoría**: Dado un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos por categoría.

33. **Formato de salida personalizado**: Crea un archivo `citas.txt`:
    ```
    "El único modo de hacer un gran trabajo es amar lo que haces."
    "La vida es lo que pasa mientras estás ocupado haciendo otros planes."
    ```
    Usa `awk` para formatear cada línea como "Cita: [texto de la cita]".

34. **Buscar patrones y reemplazar**: Dado un archivo `items.txt`:
    ```
    item1
    item2
    item3
    ```
    Usa `sed` para reemplazar "item" por "producto".

35. **Contar coincidencias**: Crea un archivo `registro.txt` con:
    ```
    Error en línea 1
    Todo correcto en línea 2
    Error en línea 3
    ```
    Usa `grep` para contar cuántas líneas contienen "Error".

### Ejercicios prácticos

36. **Generar un informe**: Dado un archivo `ventas.txt`:
    ```
    A 100
    B 150
    A 200
    ```
    Usa `awk` para generar un informe

 con la suma de las ventas por producto.

37. **Modificar el contenido de un archivo**: Crea un archivo `frases.txt`:
    ```
    La vida es bella.
    La vida es corta.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

38. **Agrupar y contar**: Dado un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    B
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

39. **Filtrar datos por longitud**: Crea un archivo `nombres.txt`:
    ```
    Juan
    Ana
    Pedro
    ```
    Usa `awk` para mostrar solo los nombres que tienen más de 3 letras.

40. **Contar caracteres por línea**: Dado un archivo `texto.txt` con varias líneas, usa `awk` para contar cuántos caracteres hay en cada línea.

### Ejercicios avanzados adicionales

41. **Contar ocurrencias**: Crea un archivo `palabras.txt`:
    ```
    hola
    mundo
    hola
    ```
    Usa `awk` para contar cuántas veces aparece cada palabra.

42. **Modificar formato de salida**: Dado un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

43. **Reemplazo condicional**: Crea un archivo `notas.txt`:
    ```
    1 5
    2 8
    3 3
    ```
    Usa `awk` para reemplazar notas menores a 5 por "Repetir".

44. **Contar líneas y palabras**: Dado un archivo `texto.txt` con varias líneas, usa `wc` para contar tanto las líneas como las palabras.

45. **Buscar y formatear**: Crea un archivo `frases.txt`:
    ```
    La vida es bella.
    La vida es corta.
    ```
    Usa `sed` para cambiar "vida" por "existencia" y `awk` para contar las frases resultantes.

### Ejercicios combinados

46. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

47. **Sumar y mostrar**: Crea un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

48. **Formatear y contar**: Dado un archivo `usuarios.txt` con:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

49. **Agrupar datos**: Crea un archivo `ventas.txt`:
    ```
    A 100
    B 150
    A 200
    ```
    Usa `awk` para generar un informe con la suma de las ventas por producto.

50. **Buscar y contar**: Dado un archivo `registros.txt` con varias líneas, usa `grep` para contar cuántas líneas contienen "Error".

### Ejercicios de práctica

51. **Reemplazar patrones en varias líneas**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

52. **Contar caracteres totales**: Dado un archivo `texto.txt` con varias líneas, usa `awk` para contar el número total de caracteres en el archivo.

53. **Filtrar y mostrar**: Crea un archivo `productos.txt` con:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

54. **Eliminar líneas duplicadas**: Dado un archivo `lista.txt`:
    ```
    item1
    item2
    item1
    ```
    Usa `sort` y `uniq` para eliminar duplicados.

55. **Contar ocurrencias de palabras**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar cuántas veces aparece una palabra específica.

### Ejercicios de análisis de datos

56. **Agrupar y contar**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto1 200
    ```
    Usa `awk` para sumar las ventas por producto.

57. **Reemplazar texto específico**: Crea un archivo `notas.txt`:
    ```
    Esto es una nota importante.
    Esto es solo un recordatorio.
    ```
    Usa `sed` para reemplazar "importante" por "crítica".

58. **Extraer y contar**: Dado un archivo `informacion.txt` con:
    ```
    nombre1;edad1
    nombre2;edad2
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

59. **Buscar y reemplazar en múltiples líneas**: Crea un archivo `frases.txt`:
    ```
    La vida es hermosa.
    La vida es efímera.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

60. **Filtrar líneas con un patrón**: Dado un archivo `textos.txt`, usa `grep` para mostrar solo las líneas que contienen la palabra "error".

### Ejercicios de administración de datos

61. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

62. **Contar y sumar**: Crea un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

63. **Extraer campos específicos**: Dado un archivo `data.txt`:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer solo los nombres.

64. **Modificar el formato de salida**: Crea un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

65. **Contar líneas y palabras**: Dado un archivo `texto.txt`, usa `wc` para contar tanto las líneas como las palabras.

### Ejercicios de manipulación de texto

66. **Buscar patrones y formatear**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

67. **Contar caracteres por línea**: Dado un archivo `texto.txt`, usa `awk` para contar cuántos caracteres hay en cada línea.

68. **Filtrar y mostrar resultados**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

69. **Eliminar duplicados**: Dado un archivo `lista.txt`:
    ```
    item1
    item2
    item1
    ```
    Usa `sort` y `uniq` para eliminar duplicados.

70. **Contar ocurrencias de palabras específicas**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar cuántas veces aparece una palabra específica.

### Ejercicios de análisis y salida de datos

71. **Agrupar y contar**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto1 200
    ```
    Usa `awk` para sumar las ventas por producto.

72. **Reemplazar texto específico**: Crea un archivo `notas.txt`:
    ```
    Esto es una nota importante.
    Esto es solo un recordatorio.
    ```
    Usa `sed` para reemplazar "importante" por "crítica".

73. **Extraer y contar**: Dado un archivo `informacion.txt` con:
    ```
    nombre1;edad1
    nombre2;edad2
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

74. **Buscar y reemplazar en múltiples líneas**: Crea un archivo `frases.txt`:
    ```
    La vida es hermosa.
    La vida es efímera.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

75. **Filtrar líneas con un patrón**: Dado un archivo `textos.txt`, usa `grep` para mostrar solo las líneas que contienen la palabra "error".

### Ejercicios de manipulación y transformación

76. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

77. **Contar y sumar**: Crea un archivo `

gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

78. **Extraer campos específicos**: Dado un archivo `data.txt`:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer solo los nombres.

79. **Modificar el formato de salida**: Crea un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

80. **Contar líneas y palabras**: Dado un archivo `texto.txt`, usa `wc` para contar tanto las líneas como las palabras.

### Ejercicios finales

81. **Buscar patrones y formatear**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

82. **Contar caracteres por línea**: Dado un archivo `texto.txt`, usa `awk` para contar cuántos caracteres hay en cada línea.

83. **Filtrar y mostrar resultados**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

84. **Eliminar duplicados**: Dado un archivo `lista.txt`:
    ```
    item1
    item2
    item1
    ```
    Usa `sort` y `uniq` para eliminar duplicados.

85. **Contar ocurrencias de palabras específicas**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar cuántas veces aparece una palabra específica.

### Más ejercicios para completar

86. **Agrupar y contar**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto1 200
    ```
    Usa `awk` para sumar las ventas por producto.

87. **Reemplazar texto específico**: Crea un archivo `notas.txt`:
    ```
    Esto es una nota importante.
    Esto es solo un recordatorio.
    ```
    Usa `sed` para reemplazar "importante" por "crítica".

88. **Extraer y contar**: Dado un archivo `informacion.txt` con:
    ```
    nombre1;edad1
    nombre2;edad2
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

89. **Buscar y reemplazar en múltiples líneas**: Crea un archivo `frases.txt`:
    ```
    La vida es hermosa.
    La vida es efímera.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

90. **Filtrar líneas con un patrón**: Dado un archivo `textos.txt`, usa `grep` para mostrar solo las líneas que contienen la palabra "error".

### Ejercicios de repaso y práctica

91. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

92. **Contar y sumar**: Crea un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

93. **Extraer campos específicos**: Dado un archivo `data.txt`:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer solo los nombres.

94. **Modificar el formato de salida**: Crea un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

95. **Contar líneas y palabras**: Dado un archivo `texto.txt`, usa `wc` para contar tanto las líneas como las palabras.

### Ejercicios finales para el dominio

96. **Buscar patrones y formatear**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

97. **Contar caracteres por línea**: Dado un archivo `texto.txt`, usa `awk` para contar cuántos caracteres hay en cada línea.

98. **Filtrar y mostrar resultados**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

99. **Eliminar duplicados**: Dado un archivo `lista.txt`:
    ```
    item1
    item2
    item1
    ```
    Usa `sort` y `uniq` para eliminar duplicados.

100. **Contar ocurrencias de palabras específicas**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar cuántas veces aparece una palabra específica.

### Ejercicios de aplicación práctica

101. **Agrupar y contar**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto1 200
    ```
    Usa `awk` para sumar las ventas por producto.

102. **Reemplazar texto específico**: Crea un archivo `notas.txt`:
    ```
    Esto es una nota importante.
    Esto es solo un recordatorio.
    ```
    Usa `sed` para reemplazar "importante" por "crítica".

103. **Extraer y contar**: Dado un archivo `informacion.txt` con:
    ```
    nombre1;edad1
    nombre2;edad2
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

104. **Buscar y reemplazar en múltiples líneas**: Crea un archivo `frases.txt`:
    ```
    La vida es hermosa.
    La vida es efímera.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

105. **Filtrar líneas con un patrón**: Dado un archivo `textos.txt`, usa `grep` para mostrar solo las líneas que contienen la palabra "error".

### Ejercicios de dominio avanzado

106. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

107. **Contar y sumar**: Crea un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

108. **Extraer campos específicos**: Dado un archivo `data.txt`:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer solo los nombres.

109. **Modificar el formato de salida**: Crea un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

110. **Contar líneas y palabras**: Dado un archivo `texto.txt`, usa `wc` para contar tanto las líneas como las palabras.

### Ejercicios de análisis de datos avanzados

111. **Buscar patrones y formatear**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

112. **Contar caracteres por línea**: Dado un archivo `texto.txt`, usa `awk` para contar cuántos caracteres hay en cada línea.

113. **Filtrar y mostrar resultados**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.

114. **Eliminar duplicados**: Dado un archivo `lista.txt`:
    ```
    item1
    item2
    item1
    ```
    Usa `sort` y `uniq` para eliminar duplicados.

115. **Contar ocurrencias de palabras específicas**: Crea un archivo `texto.txt` con varias líneas de texto. Usa `awk` para contar cuántas veces aparece una palabra específica.

### Ejercicios de práctica y aplicación

116. **Agrupar y contar**: Dado un archivo `ventas.txt`:
    ```
    producto1 100
    producto2 150
    producto1 200
    ```
    Usa `awk` para sumar las ventas por producto.

117. **Reemplazar texto específico**: Crea un archivo `notas.txt`:
    ```
    Esto es una nota importante.
    Esto es solo un recordatorio.
    ```
    Usa `sed` para reemplazar "importante" por "crítica".

118. **Extraer y contar**: Dado un archivo `informacion.txt` con:
    ```


    nombre1;edad1
    nombre2;edad2
    ```
    Usa `cut` para extraer los nombres y `wc -l` para contar cuántos nombres hay.

119. **Buscar y reemplazar en múltiples líneas**: Crea un archivo `frases.txt`:
    ```
    La vida es hermosa.
    La vida es efímera.
    ```
    Usa `sed` para cambiar "vida" por "existencia".

120. **Filtrar líneas con un patrón**: Dado un archivo `textos.txt`, usa `grep` para mostrar solo las líneas que contienen la palabra "error".

### Ejercicios finales de dominio

121. **Eliminar líneas vacías**: Dado un archivo `documento.txt` con varias líneas, algunas vacías, usa `sed` para eliminar las líneas vacías.

122. **Contar y sumar**: Crea un archivo `gastos.txt`:
    ```
    comida 10
    transporte 5
    comida 15
    ```
    Usa `awk` para sumar los gastos y mostrar el total.

123. **Extraer campos específicos**: Dado un archivo `data.txt`:
    ```
    1;Juan;20
    2;Ana;25
    ```
    Usa `cut` para extraer solo los nombres.

124. **Modificar el formato de salida**: Crea un archivo `clientes.txt`:
    ```
    1;Juan;1000
    2;Ana;1500
    ```
    Usa `awk` para mostrar la salida como "Cliente 1: Juan, Saldo: 1000".

125. **Contar líneas y palabras**: Dado un archivo `texto.txt`, usa `wc` para contar tanto las líneas como las palabras.

### Ejercicios de aplicación práctica avanzada

126. **Buscar patrones y formatear**: Crea un archivo `mensajes.txt`:
    ```
    Error en el sistema.
    Todo funcionando bien.
    ```
    Usa `sed` para reemplazar "Error" por "Advertencia".

127. **Contar caracteres por línea**: Dado un archivo `texto.txt`, usa `awk` para contar cuántos caracteres hay en cada línea.

128. **Filtrar y mostrar resultados**: Crea un archivo `productos.txt`:
    ```
    A
    B
    A
    C
    ```
    Usa `sort` y `uniq` para contar la cantidad de cada producto.
