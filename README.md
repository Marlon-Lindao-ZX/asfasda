# TALLER UNIDAD 2

Se desea realizar una aplicación para el manejo de garages. Para empezar va a modelar el manejo de los garages y los carros que puede acoger.

Desarrolle en Java las siguientes clases:


### Clase Carro:
Atributos privados:
- matrícula.  Identificador del carro.  Tipo  de dato String
- clave. Clave para desbloquear el carro. Tipo de dato int

Constructor
- Constructor con los parámetros para los dos atributos

Métodos
- getters para todos sus atributos

### Clase Garage:

Atributos privados:

- El nombre. Nombre del garage. Tipo  de dato String
- La capacidad. La cantidad de carros máxima que puede albergar. Tipo de dato int
- Puestos libres. La cantidad de puestos que están disponibles en el garage.  Tipo de dato int

Constructores:
- Constructor con parámetro para el nombre.  Este constructor asigna además el valor de 20 a la capacidad y los puestos libres. 
- Constructor con parámetros nombre y capacidad.  Este constructor asigna los valores a los atributos respectivos y al atributo puestos libres el valor de capacidad.

Métodos
- getters para todos sus atributos
- parquearCarro. Ubica un carro en el garage. Este método tiene como parámetro un objeto de tipo Carro. Este método debe verificar si el garage tiene un puesto para el carro que se va a parquear. Si hay puesto libre modifica el atributo de los puestos libres disminuyendo su valor en 1, imprime el mensaje "Parqueando carro <MATRICULA>".(Ver ejemplo de salida) y retorna  **true**, caso contrario retorna  **false**

**NOTA: Ubique las clases Carro y Garage en el paquete modelo**

### Clase Main:
Desarrollar en el método main lo siguiente
- Cree dos objetos de tipo Garage.  Un objeto con el constructor que recibe el nombre y otro objeto con el constructor que recibe dos atributos. Asigne los valores que ud. desee a los atributos del garage.
- Simule el proceso de parquear carros en el garage(Seleccione el objeto de tipo Garage que prefiera)
  - Genere un número aleatorio entre 1 y la capacidad del garage + 5 para indicar cuántos carros va a parquear.
  * Use el número aleatorio para realizar iteraciones para la creación de objetos tipo Carro.  
  * En cada iteración:
    - Pida al usuario la matricula y la clave del carro y cree el objeto.  
    - Llame al método parquearCarro del garage elegido usando el objeto de tipo Carro creado.  Si el carro no se pudo parquear en el garage imprima el mensaje "Garage sin lugares libres" y termine la iteración.
  * Presente la información del garage 

_Nota: Asuma que el usuario va a ingresar los datos en el formato esperado.  No olvide incluir comentarios_

_Ejemplo de ejecución en la que no se pueden parquear todos los carros_
```
Cantidad de carros a parquear:7
Ingrese matricula del carro:GNW-1234
Ingrese clave del carro:1234
Parqueando carro GNW-1234
Ingrese matricula del carro:GNW-2345
Ingrese clave del carro:2341
Parqueando carro GNW-2345
Ingrese matricula del carro:GNW-1256
Ingrese clave del carro:6435
Parqueando carro GNW-1256
Ingrese matricula del carro:GNW-5453
Ingrese clave del carro:6333 
Garage sin lugares libres

Información del garage utilizado
Nombre: Malecon Colon
Capacidad: 3
Disponibles: 0

```
_Ejemplo de ejecución que completa las iteraciones_

```
Cantidad de carros a parquear:8
Ingrese matricula del carro:GNW-3245
Ingrese clave del carro:3245  
Parqueando carro GNW-3245
Ingrese matricula del carro:GNW-3433
Ingrese clave del carro:4322      
Parqueando carro GNW-3433
Ingrese matricula del carro:GNX-3432
Ingrese clave del carro:3221
Parqueando carro GNX-3432
Ingrese matricula del carro:GNS-3243
Ingrese clave del carro:3215
Parqueando carro GNS-3243
Ingrese matricula del carro:GMU-4323
Ingrese clave del carro:5325
Parqueando carro GMU-4323
Ingrese matricula del carro:PEW-3432
Ingrese clave del carro:4323
Parqueando carro PEW-3432
Ingrese matricula del carro:GEW-3243
Ingrese clave del carro:3433
Parqueando carro GEW-3243
Ingrese matricula del carro:GTU-3243
Ingrese clave del carro:4333
Parqueando carro GTU-3243
Información del garage utilizado
Nombre: Malecon Colon
Capacidad: 10
Disponibles: 2
```
