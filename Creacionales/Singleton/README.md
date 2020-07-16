# Abstract Factory :waning_gibbous_moon:

## 1. Introducción.

Utilizaremos el patrón Singleton cuando por alguna razón necesitemos que exista sólo una instancia (un objeto) de una determinada Clase. Muchas veces deseamos esto y mas alla de desearlo lo veremos obligatorio hacerlo, como por ejemplo alguna conexión a una base de datos. Cabe mencionar y es curioso, que a Singleton tambien se le conoce como un antipatrón, es decir que en vez de aportar soluciones buenas o positivas a nuestro software, este trae problemas, un mal uso de Singleton nos podria hacer caer en estas trampas.

![intIMg](img\singleton.png)

## 1. Nombre del patrón.

Singleton.

## 2. Clasificación del patrón.

Creacional

## 3. Intención.

Singleton proporciona que se lleve a cabo solo una instanciación de una clase, es decir, solo existe un objeto de esta clase en el programa, 
mientras proporciona un punto de acceso global a esta instancia. Como en la imagén que observamos arriba.

## 4. También conocido como.

Singleton

## 5. Motivación.
Usamos Singleton cuando una clase en el programa debe tener solo una unica instancia disponible para todos los clientes; por ejemplo, un solo objeto en una base de datos el cual es compartido para diferentes partes del programa.

## 6. Aplicabilidad.

Otros usos comunes de este patrón es cuando necesitamos control estricto sobre variables globales.

Los criterios para aplicar este patrón son:

- Solo debe existir una única instancia de una clase y debe existir un acceso a esta.

- Cuando esta única instancia debe ser extendida por subclases y los clientes deben ser capaces de extender esta instancia sin la modificación de sus códigos.

## 7. Estructura.
El siguiente diagrama representa Singleton:

![umlSingleton](img\uml.png)

## 8. Participantes.

- Singleton: La clase Singleton declara el metodo estatico **getInstance()** el cual retorna o devuelve la misma instancia de esta propia clase.
    
    El constructor debe ser escondido del cliente. Llamando al metodo **getInstance()** debe ser la unica manera de obtener el objeto de la clase Singleton

- Client: El cual necesita obtener el objeto de Singleton.


## 9. Colaboraciones.

Como se menciono en el apartado de **Participantes** , Singleton se encarga de crear su propia instancia, y en cuanto al cliente, el cliente obtiene el objeto de Singleton, solo por medio del metodo **getInstance()**, no lo podra hacer mediante un "new" por ejemplo, ya que el constructor de Singleton es privado, entonces no devolvera el objeto como suele ser si este (el constructor) es publico. El cliente solo obtendra una unica instancia, no sera posible crear otro, ya que Singleton no se lo permitira, a menos que se modifique el metodo que realiza esta acción y defina un numero de instancias a crear.

## 10. Consecuencias.

:white_check_mark:
-  Estas seguro que una clase tiene una sola instancia.
- Ganas un punto de acceso global a esa instancia.

- El objeto Singleton es inicializado solo cuando es requerido por primera vez. 



## 11. Implementación.

## 12. Código de ejemplo.

## 13. Usos conocidos.

## 14. Patrones Relacionados.