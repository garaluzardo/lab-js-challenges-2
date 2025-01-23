1. Challenge 1:
  - Answer: b) "xyz" and "xyz"
  - Explanation:
    Comenzamos con una variable let foo que ha sido declarada fuera de la función y pertenece al global scope. Como se ha usado una variable let, podrá ser modificada.
    
    A continuación vemos que la función bar() no declara una nueva variable, sino que actualiza el valor de la ya declarada fuera de la función, la reasigna. Por tanto se modificará el valor cambiando "abc" por "xyz" en la variable global y por eso ambos console.log(foo) reflejarán el mismo resultado ("xyz").


2. Challenge 2:
  - Answer: c) 10 and 1
  - Explanation:
    Comenzamos con una variable let a = 1, variable global ya que está declarada fuera de la función.

    Lo siguiente que vemos es una función que tiene como argumento el valor de la variable global (1).
    En este punto, al pasar el valor de la variable global como argumento de la función, ese parámetro pasaría a ser una variable local y podríamos modificarlo sin afectar a la variable externa o global. Como consecuencia cada console.log dará un valor distinto, reflejando en este caso el de la variable local primero (10) y el de la global después (1).


3. Challenge 3:
  - Answer: c) "Hi there!"
  - Explanation:
    Aunque el valor no está definido o declarado en la función inicialmente, debido al hoisting, la declaración de la función se moverá/procesará al inicio del scope antes de la ejecución del código.


4. Challenge 4:
  - Answer: c) { num: 90 }
  - Explanation:
    Al imprimir la consola se mostrará { num: 90 } porque al declarar const b = a no se está creando un nuevo objeto, sino copiando la referencia del valor de "a" y asignándolo a "b", por tanto ambas variables parten del mismo punto o misma ruta en la memoria. Entonces cuando se modifica la propiedad de "b", al referenciar el mismo objeto que "a", se modifica el valor de ambas.


5. Bonus - Challenge 5:
  - Answer:
  - Explanation:
