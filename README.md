# Pepita (parte 2)

Este ejercicio extiende la versión inicial de pepita para que les estudiantes agreguen
sus primeras líneas en wollok luego de la explicación del docente

## Ejercicio 1: Pepona

Agregar a Pepona: Es otra ave que puede comer el alpiste y la manzana y sigue las siguientes reglas:

- La energía inicial de Pepona es 30.
- Sabe decir su energía. 
- Cuando come, solo puede aprovechar la mitad de la energía que aporta el alimento
- Cuando vuela gasta 20 fijos más 2 joules por km, 

Ejemplos:
- si tiene 30 de energía y come alpiste su nueva energía es 30 + 20/2 = 40 
- si tiene 30 de energía y vuela 3 km su nueva energía es: 30 - 20 - 2*3 = 4


## Ejercicio 2: Roque
Agregar a Roque, que es una persona.

### Ave de roque
Tiene un ave, a veces es Pepona, a veces es Pepita, por lo tanto tiene que entender un mensaje para que se le indique cual es su ave. Inicialmente es Pepita.

### Alimentar

 Entiende el mensaje *alimentar*, que recibe un alimento por parámetro. Al recibir este mensaje Roque alimenta a su ave. 

Ejemplos:
- Si tiene a Pepona con energía de 30, y recibe el mensaje alimentar(alpiste) pepon queda con 40 de energía
- Si tiene a Pepita con energía de 100 y recibe el mensaje alimentar(alpiste) pepita queda con 120 de energía.

### Cenas

Entiende el mensaje *cenas* sin parámetros, el cual devuelve la cantidad de veces que Roque dio de alimentar a su ave desde que es la suya (pensar como hacer para recordar este dato y que pasa al cambiar de ave).


## Ejercicio 3: Excepciones al volar
Las aves cada una tiene sus virtudes y defectos, por lo que a veces no pueden hacer lo que se les pide.
 Pepita y Pepona al querer volar deben tener suficiente energia, si no se amotinan y no te vuela nada, lanzando una excepción.
  
Se pide 
* Implementar las validacionesa y consultas correspondientes realizando las modificaciones a los objetos ya resueltos para garantizar que un ave no puede volar bajo dada condiciones. 

Ejemplos: 
 Suponiendo que Pepita tiene energia 100 y Pepona 30.
 
 * Tanto Pepita como Pepona pueden volar 4 kms.
 * Pepona no puede volar 6 kms.
 * Ninguna puede volar 100 kms.

## Ejercicio BONUS: Excepciones al comer
 Pepona es delicada con su alimentación, por lo que le gusta solo comer variado. Si se le da de comer lo mismo que comió la última vez se niega. Por defecto comió manzana la última vez.

Se pide 
* Implementar las validacionesa y consultas correspondientes realizando las modificaciones en Pepona, para garantizar que no puede comer la misma comida que comió la última vez.

Ejemplos: 
 Suponiendo que Pepona tiene 30 de energia y comió manzana la última vez.
 
 * Puede comer alpiste, quedando su energia en 40. Pero ai luego intenta comer alpiste nuevamente no puede, quedando em 40 su energia.
 * Si luego come manzana lo hace sin problema, pero luego no puede comer manzana otra vez pero si alpiste.
 
## Ejercicio BONUS: Milena la entrenadora

Milena es una entrenadora de aves que puede entrenar a varias a la vez. Cuando Milena recibe el mensaje movilizar(distancia), hace que todas sus aves se muevan esa distancia.

Se pide 
* implementar a milena, 
* realizar las modificaciones a los objetos ya resueltos para garantizar que un ave no puede volar una distancia mayor a la de su energia. 
* Tener en cuenta que milena no puede movilizar sus aves si alguna de ellas no puede recorrer esa distancia.

Ejemplos: 
 Suponiendo que milena tiene a pepita y a pepon, con sus respectivas energias iniciales (100 y 30).
 
 * tanto pepita como pepon pueden volar 4 kms. Por lo tanto milena puede movilizarlas.
 * pepita puede volar 6 kms, pero pepon no. Por lo tanto milena no puede movilizarlas. (Si se intenta movilizarlas ambas deben quedar con su energia inicial)
 * ni pepita ni pepon pueden volar 100 km.
 
 
 
 
 











