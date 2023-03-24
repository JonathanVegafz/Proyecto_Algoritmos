**Ecuación 1.**

a = valor desde [2,0] , decrece mientras más iteraciones ocurran

r = vector random desde [0,1]

A,C = valores aleatorios que se utilizan para controlar el movimiento de las ballenas y actualizar su posición en el espacio de búsqueda.







**Ecuación 2.**

Esta ecuación representa a la ballena encerrando a su presa (estrategia 1)

D = distancia de la ballena a la presa

X(t+1) = actualiza la posición 




**Ecuación 3.**

La ecuación representa a la ballena avanzando en espiral alrededor de su presa. (estrategia 2)

l = numero random desde [-1,1]

b = constante para definir la forma en espiral

D = distancia de la ballena a la presa











**Ecuación 4.**

p = numero random desde [0,1]

esta ecuacion representa el 50% de probabilidad de que una ballena eliga entre encerrar a su presa (ecuacion 2) o girar en espiral al rededor de su presa(ecuacion 3)

























|<p>Inicializar la población de ballenas Xi (i = 1, 2, ..., n) Calcular la aptitud de cada agente de búsqueda X\*=el mejor agente de búsqueda</p><p></p><p>mientras (t < número máximo de iteraciones)</p><p>`  `para cada agente de búsqueda Actualice a, A, C, l y p</p><p>`    `si 1 (p<0.5)</p><p>`      `si 2 (|A| < 1)</p><p>`        `Actualizar la posición del agente de búsqueda actual por la ecuación. (2.1) </p><p>`      `sino si 2 (|A| >= 1)</p><p>`        `Seleccione un agente de búsqueda aleatorio ( )</p><p>`        `Actualizar la posición del agente de búsqueda actual por la ecuación. (2.8)</p><p>`      `fin si 2 </p><p>`    `sino si 1(p >= 0.5)</p><p>`      `Actualizar la posición del agente de búsqueda actual por la ecuación. (2.8)</p><p>`    `fin si 1</p><p>fin para</p><p></p><p>Comprobar si algún agente de búsqueda va más allá del espacio de búsqueda y modificarlo Calcular la aptitud de cada agente de búsqueda</p><p></p><p>Actualice X\* si hay una solución mejor</p><p></p><p>t=t+1</p><p>fin Mientras</p><p>retornar X\*</p><p></p>|
| :- |

