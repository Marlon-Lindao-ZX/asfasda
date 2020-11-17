# TALLER UNIDAD 2 Y 3

Ud va a empezar a desarrollar una aplicación para el manejo de un album de fotos.  Para empezar realice lo siguiente:

Parte1:
1. Crear la clase Fotografia de acuerdo al diagrama de clases mostrado en la figura.
2. Crear dos constructores para la clase Fotografia.  
    - El primer constructor recibirá como parámetros el nombre y ubicacion.  El valor por defecto para el tamaño será 200
    - El segundo constructor recibirá como parámetros nombre, ubicacion, tamano y asignará los valores a su atributo correspondiente.
3. Escribir el método toString para mostrar toda la información de la foto
4. Escribir el get para cada atributo.

Parte2: Completar la clase Main.java de acuerdo al diagrama.  Esta clase sería como el album de fotos
1. Escribir el constructor sin parámetros que crea el arraylist fotos;
2. Escribir el método consultarFoto(String nombre) que consulta el arraylist fotos para retornar el objeto Fotografia cuyo nombre coincide exactamente con el nombre recibido en el parámetro.
3. Escribir el método consultarFoto(int tam) que consulta el arraylist fotos para retornar un arraylist de objetos Fotografia cuyo tamaño es menor o igual al tamaño recibido en el parámetro.
4. En el método main crear 3 objetos de la clase Fotografia con la información de la tabla siguiente. Almacenar los 3 objetos en el arraylist fotos

| Nombre  | Ubicacion   | Tamaño   | 
|---|---|---|
| Carnet  | C://Pictures  |  200 |
| PaseoFeriado  |   C://Pictures | 400  |
| Cumpleaños  |  C://Pictures  | 900  |

5. Realizar el proceso de consulta de fotos
- Consulta1: Solicitar el ingreso del nombre de la foto.  Deberá utilizar el método consultarFoto apropiado para mostrar información de la foto si es que existe o el mensaje “No hay foto con ese nombre” en caso contrario.
- Consulta2: Solicitar un tamaño a consultar.  Deberá utilizar el método consultarFoto apropiado para mostrar información de las fotos con tamaño menor o igual al ingresado o el mensaje “No hay fotos con ese tamaño” si no se encontraron fotos.

_Ejemplo de salida exitoso_
```
Consulta 1
Ingrese nombre de foto a consultar:Carnet   
Foto encontrada:
Fotografia: nombre= Carnet, ubicacion= C://Pictures, tamano= 200
Consulta 2
Ingrese tamano a consultar:500
Fotos encontradas:
Fotografia: nombre= Carnet, ubicacion= C://Pictures, tamano= 200
Fotografia: nombre= PaseoFeriado, ubicacion= C://Pictures, tamano= 400
```
_Ejemplo de salida sin resultados_
```
Consulta 1
Ingrese nombre de foto a consultar:Viaje
No hay foto con ese nombre
Consulta 2
Ingrese tamano a consultar:100
No hay fotos con ese tamano
```

```
