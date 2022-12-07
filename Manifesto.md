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

## Problema (Teoria de numeros)

¿Por que tres numeros sucesivos cualquiera, si se multiplica el menor por el mayor te da un numero menor al cuadrado del numero de en medio?

Empecemos definiendo el problema, decimos que $\exists a,b,c\in \mathbb{Z}$ pues al ser numeros consecutivos se intuye que son enteros solamente, ahora si son consecutivos quiere decir que la diferencia entre ellos es de $1\therefore a+1=b\:y\:b+1=c$ ahora atendamos al problemas, se nos plantea la siguiente cuestion ¿Por que $a\cdot c=b^2-1$?

Para empezar, generalicemos el problema, definamos a $a$4 como $n$ siendo que $n\in \mathbb{Z}$, pues dicho caso $b$ sera $n+1$ y $c$ sera $n+2$ bien este problema se establece que $a\cdot c=b^2-1$ atendamos cada bloque de la ecuacion por separado $a\cdot c=n\left(n+2\right)$ bien si simplificamos esto nos da $n^2+2n=ac$ ahora bien para $b^2$ se escribiria $\left(n+2\right)^2=\left(n+1\right)\left(n+1\right)$ lo que en resumidas cuentas es $n^2+n+n+1=n^2+2n+1$.
Volviendo al cuestionamiento inicial ¿$ac=b^2-1$? comprobemos, reemplazamos $ac$ por $n^2+2n$ y $a\:b^2$ por $n^2+2n´1$ quedando que $\left(n^2+2n\right)=\left(n^2+2n+1\right)-1$ y si resolvemos veremos que en efecto se cumple el enunciado.

$\therefore$ concluimos el problema diciendo que $\forall \:a,b,c\in \mathbb{Z}\:tq\:a+1=b,\:b+1=c$ se cumple que $a\cdot c=b^2-1$

## Productos Notables (Algebra)
Sean $x,y,z\in \mathbb{R}$ podemos obtener las siguientes igualdades

$x^2+2xy+y^2=¿?$ para esto tenemos que descomponer la expresion a su maxima forma es decir, $x^2+xy+xy+y^2$, una vez aqui dividiremos la expresion en dos bloques: $x^2+xy$ y $xy+y^2$, muy bien ya que tenemos esto factoricemos la expresion parte por parte: para $x^2+xy$ notamos que $x$ compone a ambos elemetos por lo que es su factor comun, si lo sacamos obtenemos que $x^2+xy=x\left(x+y\right)$. La misma logica aplica para $xy+y^2$, ya que la $y$ es su factor comun, lo sacamos en la factorizacion quedando que $xy+y^2=y\left(x+y\right)$. Su unimos todo nos queda que la expresion $x^2+xy+xy+y^2=x\left(x+y\right)+y\left(x+y\right)$, en $x\left(x+y\right)$ y $y\left(x+y\right)$ vemos un factor comun, el $\left(x+y\right)$, asi que lo sacamos y obtenemos $\left(x+y\right)\left(x+y\right)$, como sabemos que $a\cdot a=a^2$ podemos decir que $\left(x+y\right)\left(x+y\right)=\left(x+y\right)^2\:y\:\therefore x^2+2xy+x^2=\left(x+y\right)^2$

$x²-y²=¿?$ para este tendremos que aplicar una curiosa propiedad, pues para completar la ecuacion sin alterar el resultado habra que agregar un 0, sí un 0, pero el truco no esta en agregarlo, sino en como lo hacemos, pues bien el 0 se puede agregar como tal, tambien lo podemos representar como $a-a=0$, o como nos interesa mas a nosotros $xy-xy$, de este modo podemos completar la expresion sin alterar el resultado tal que $x²-y²=x²+xy+xy-y²$, esto empieza a tomar forma, ahora nuevamente dividimos la expresion el bloques para factorizarlos: en este caso $x²-xy$ vemos que $x$ es el factor comun, si factorizamos en esta caso $x²-xy$ vemos que "$x$" es el factor comun, si factorizamos tenemos que $x²-xy=x(x-y)$. Para el bloque $y$ se usaran $xy-y²$ el cual se puede factorizar como $y(x-y)$ al unir todo de nuevo obtenemos $x(x-y)+y(x-y)=x²+xy-xy-y²$, ahora bien si miramos su factor comun es (x-y), si lo sacamos obtenemos la expresion que dice $x(x-y)+y(x-y)=(x+y)(x-y)$ que $\therefore x²-y²=(x+y)(x-y)$ una diferencia de cuadrados.

$x²+y²+z²+2(xy+xy+yz)=¿?$ empecemos resolviendo el parentesis, es decir que $2(xy+xz+yz)=2xy+2xz+2yz$, como sabemos que $a+a-2a$, podemos reescribir la expresion como $2xy + 2xz +2yz = xy + xy + xZ + x2 +yz + yz$, asi que ahora solo queda remplazar y obtendremos que $x²+y²+z²+xy+xy+xz+xz+yz+yz$, a simple vista pudiera parecer quer solo empeoramos las cosas, pero la realidad es que estamos muy cercas de resolverlo, ahora vamos a volver a dividir la expresión por bloques de factores comunes sin repetir ningún termino tal que para $x$ tenemos el bloque compuesto por $x²+xy +xz$, sacamos al factor común, que seria $x$ y obtendremos que $x²+xy+xz=x(x+y+z)$. 
Para el bloque de las $y$ se envlobaran los terminos $y²+xy+yz$ el cual se puede factorizar a partir de sacar el elemento comun, $y$, $\therefore y²+xy+yz=y(y+x+z)$. Para el bloque $z$ aplica la misma logica $z²+yz+xz=z(z+y+x)$ . Uniendo todos los bloques se obtiene que $x(x+y+z)+y(y+x+z)+z(z+y+x)$ esto ya va tomando mas forma, para el siguiente paso hay que revisar una propiedad muy curiosa de la suma y la clave para nuestro siguiente truco, pues resulta que $a+b=b+a$ y si eres observador veras dentro de los parentesis solo se realizaran sumas y no solo eso, sino que se estan sumando los mismo terminos $x,y,z$ $\therefore$ podemos decir que $(x+y+z)=(y+x+z)=(z+y+x)$ asi que entendiendo esto podemos elegir una de las expresiones y sustituir al resto por esa misma de modo que alfinal la ecuacion nos queda algo similar a esta forma $x\left(x+y+z\right)+y\left(y+x+z\right)+z\left(z+y+x\right)=x\left(x+y+z\right)+y\left(x+y+z\right)+z\left(x+y+z\right)$ y si tenemos un termino multiplicandose por si mismo se dice que $\left(x+y+z\right)\left(x+y+z\right)=\left(x+y+z\right)^2$ $\therefore$ podemos concluir que para todo $x,y,z$ que cumpla su pertenencia a los reales, cumple que $x^2+y^2+z^2+2\left(xy+xz+yz\right)=\left(x+y+z\right)^2$




