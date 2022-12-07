# Manifesto
Autores: Julio Porfirio, Pedro Guzman, Elias Garza

Transcripcion: Diego Alejandro Moreno

## Simbologia Matematica
Potencia $a^x=a\cdot a\cdot a\cdot a\cdot a...$ un "a" que se multiplica a si mismo "x" veces

Tetración $^xa=a^{a^{a^{...}}}$ un "a" elevado a si mismo "x" veces

Pi $\pi =\frac{diametro}{perimetro}=3,141592...$ un número que determina la relación perimetro-diametro

Euler $e=2,71828...$ un número derivado del logaritmo natural

Conjunto { } una serie de elementos con caracteristicas en común

Pertenencia $\in$  $\notin$  $\in$ refleja que algo pertenece a un conjunto

Tal que... tq I :  usado para hacer cumplir algo sobre una oración

Naturales $\mathbb N=\{1,2,3,4,5,6,7,8,...,\infty\}$  los numeros usados cotidianamente

Enteros $\mathbb Z=-\infty,...,-4,-3,-2,-1,0,1,2,3,...,\infty$

Racionales $\mathbb Q=\frac{b}{a}:a\in \mathbb{Z},\:a\ne 0,\:b\in \mathbb{Z}$ los numeros que se pueden escribir como fracción.

Reales $\mathbb R,   \mathbb N \subsetneq \mathbb Z \subsetneq \mathbb Q \subsetneq \mathbb R$ todos los numeros existentes en la realidad

Complejos $\mathbb C=a+b+i:a,b\in \\mathbb{R}$ son numeros reales compuestos por uno imaginario

Imaginarios $i=\sqrt{1}\quad tq\ \quad i\notin \mathbb{R}$ es la solucion de la ecuacion $x^2+1=0$

Inclusion $\subseteq \quad \subsetneq \quad \nsubseteq$ refleja que un conjunto esta o no contenido en otro

Mayor que $> \quad \geq$ refleja que un termino es mayor en escala que otro

Menor que $< \quad \leq$ relfeja que un termino es menor en escala que otro

Interseccion $A\cap B$ dicta la zona o elementos en comun de dos conjuntos

Union $A\cup B$ dicta la totalidad de dos conjuntos unidos

Existencia $\exists \quad \nexists$ se usa para decir que algo existe o no

Implicacion $\Rightarrow$ denota que un resultado implica otro resultado o conclusion

Si y solo si $\Leftrightarrow$ se usa para denotar que algo se cumple solo si otra es cierta

Primos $\mathbb P=\frac{n}{m}=a\left|n\notin \mathbb{Z}^+\right|m,a=n\quad o\quad 1$ numeros solo divisibles entre si mismos y por uno

Factorial $\binom{n}{k}=\frac{n!}{\left(n-k\right)!k!}$ usado en combinatoria, se lee como "n sobre k"

Por lo tanto $\therefore$ se usa para dictaminar una conclusion o resultado

Para todo $\forall$ se usa apra enunciar un resultado para todo elemento dicho

Divisibilidad $A|B$ refleja que un numero es divisor de otro expuesto

Contradiccion $\Rightarrow \Leftarrow$ refleja algo falso o que se contradice a si mismo

## Factoria (Combinatoria)

Entendemos a un factorial como la multiplicacion de todos los enteros positivos, hasta el 1, que preceden a un n, de forma que se puede definir que: $n! \Leftrightarrow n\in \mathbb{Z}^+, n!= n\left(n-1\right)\cdot \left(n-2\right)\cdot ...\cdot 1$

Los factoriales son muy importantes en combinatoria, pues facilitan contar.

Por ejemplo, imaginemos que quiero acomodar a 10 personas en una fila, si no me importa el orden, es decir que $AB=BA$ entonces, cuantas formas distintas hay de conseguirlo?

En primer lugar tenemos diez posibles lugares para colocarlos, para el primer lugar tendremos a 10 candidatos para elegir, al avanzar al segundo ligar solo contaremos con 9 candidatos, pues a uno ya lo posicionamos en el lugar anterior, para el tercero se contara con 7, pues ya habremos colocado dos anteriormente, y asi sucesivamente hasta llegar al ultimo lugar, donde unicamente contamos con un candidato, visto de forma grafica seria:

$$
\begin{pmatrix}
10 candidatos & 9 cantidatos & 8 candidatos & 7 candidatos & 6 candidatos & 5 candidatos & 4 candidatos & 3 candidatos & 2 candidatos & 1 cantidato\\
\vdots & \vdots & \vdots & \vdots & \vdots & \vdots & \vdots & \vdots & : & .\\
\vdots & \vdots & \vdots & \vdots & \vdots & : & . & \\
\vdots & \vdots & : & . & \\
. \\
\end{pmatrix}
$$

Visto de esta manera es sencillo ver como sacar los posibles formas de acomodarlos, simplemente bastaria con multiplicar la cantidad de cantidatos posibles que hay por lugar, obteniendo que para este caso $10\cdot 9\cdot 8\cdot 7\cdot 6\cdot 5\cdot 4\cdot 3\cdot 2\cdot 1$ son las formas posibles de formarlos, lo cual tambien se puede reescribir como 10! (10 factorial)

## Problema (Combinatoria)

Imagina que deseas sentar a 10 personas, pero solo cuentas con 6 sillas, cuantas formas posibles hay de sentarlos.

Pues este problema es algo diferente al anterior, pues aunque aun contamos con las 10 personas, ahora solo existen 6 lugares donde pueden sentarse, asi que, como podemos resolver este problema?. Pues simple, asumamos que no hay 6, sino 10 lugares, de esta manera podremos operar como anteriormente lo hicimos, posteriormente le "restamos" las posibilidades hipoteticas y tendremos el resultado real. Usando la logica anterior, se tiene 10 lugares y 10 personas por sentar, facil. 10!, muy bien, ya vamos a la mitad del camino, ahora solo falta quitar los 4 lugares que nosotros aplicamos, razonemos; si hay 10 personas para el primer lugar tendremos 10 canidatos para sentar, para el segundo 9, para el tercero 8... y asi hasta que lleguemos al sexto lugar, que es el ultimo asiento real, en este punto solo contamos con 5 personas candidatas a ser sentados, asi que elegimos a una bien, ahora empiezan los lugares imaginarios, para el septima teoricamente hay 4 personas candidatas, para el octavo 3, para el noveno 2 y para el decimo solamten 1.


$\quad \quad LUGARES \quad REALES  \quad \quad \quad \quad \quad \quad \quad  \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad LUGARES \quad IMAGINARIOS$

$$
\begin{pmatrix}
10 candidatos & 9 cantidatos & 8 candidatos & 7 candidatos & 6 candidatos & 5 candidatos & | & 4 candidatos & 3 candidatos & 2 candidatos & 1 cantidato\\
\vdots & \vdots & \vdots & \vdots & \vdots & \vdots & | & \vdots & \vdots & : & .\\
\vdots & \vdots & \vdots & \vdots & \vdots & : & | & . & \\
\vdots & \vdots & : & . & \\
. \\
\end{pmatrix}
$$

Bien, 10! es el total de lugares, a este hay que "restarle" los lugares hipoteticos, que si nos damos cuenta es $4!=4\cdot 3\cdot 2\cdot 1$ y obtendremos los lugares reales, y como se esta multiplicando, la "resta" queda $\frac{10!}{\:4!}=\frac{10\cdot 9\cdot 8\cdot 7\cdot 6\cdot 5\cdot 4\cdot 3\cdot 2\cdot 1}{4\cdot 3\cdot 2\cdot 1}=10\cdot 9\cdot 8\cdot 7\cdot 6\cdot 5$

## Pares e Impares (Teoria de numeros)

Supongamos que te pidieran formar un numero par con cualquier otro numero, que haces?. Pues pensemos, que hace a un numero par ser par? Pues facil, que se pueda dividir entre dos, pues si esto es lo que caracteriza a un par, como podemos forzar a cualquier numero a ser par?
Pues es muy obvio no? si el truco esta en que sea divisible entre dos, solo agarraremos cualquier numero y lo multiplicaremos por dos, tal que si $\exists n\in \mathbb{Z}^+$ y queremos volver a "n", par, solo lo multiplicamos como ya dijimos antes; 2n, tal que asi podemos formar a cualquier numero par habido y par por haber en los reales, por lo que si nosotros quisieramos expresar a la sucesion infinita de pares seria algo muy parecido a esto $2n=2\left(1,2,3,4,5,6,7,...,n\right)$ , por lo tanto $2n=2,4,6,8,...,2n$

Y ¿como formamos a un impar? pues es muy sencillo tambien, si nos damos cuenta que los impares son el numero inmediato a un par, tal que si $a$ es impar y $b$ par y los dos son numeros consecutivos, entonces $a-b=1 \Leftrightarrow a>b$ , con esto podemos deducir que un impar es igual a un par mas uno, por lo que ¿como expresamos esto? tomemos a nuestro buen $n$, bien $n$ puede ser par o impar pues $n\in \mathbb{Z}^+$ , entonces ¿como nos aseguramos de que sea par? pues como ya vimos 2n y ahora si queremos tener un impar pues como estos son el consecutivo de un par y discrepan por un pues resuelto $2n\pm 1$, esta expresion engloba a todos los impares.

Ahora fijate en la siguiente sucesion: $1,4,9,16,25,36,49,64,81,100$ exacto son los resultados de los cuadrados del 1 al 10: pues $1^2=1,2^2=4,3^2=9,...,10^2=100$, ahora fijate que pasa si resto $4-1=3$ y si $9-4=5$ y ahora que tal si hacemos estos con todos lossmeros cuadrados inmediatos, de mayor a menor, pues se da que obtenemos: $1,2,3,5,7,9,11,...,2n+1$ por lo que $2n+1$ esta contemplado por $n^2$, asi que intuimos que $n^2\in 2n+1\Rightarrow \:n^2=1+3+6+7+\left(2n-1\right)$



