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

## Factorial (Combinatoria)

Entendemos a un factorial como la multiplicacion de todos los enteros positivos, hasta el 1, que preceden a un n, de forma que se puede definir que: $n! \Leftrightarrow n\in \mathbb{Z}^+, n!= n\left(n-1\right)\cdot \left(n-2\right)\cdot ...\cdot 1$

Los factoriales son muy importantes en combinatoria, pues facilitan contar.

Por ejemplo, imaginemos que quiero acomodar a 10 personas en una fila, si no me importa el orden, es decir que $AB=BA$ entonces, cuantas formas distintas hay de conseguirlo?

En primer lugar tenemos diez posibles lugares para colocarlos, para el primer lugar tendremos a 10 candidatos para elegir, al avanzar al segundo ligar solo contaremos con 9 candidatos, pues a uno ya lo posicionamos en el lugar anterior, para el tercero se contara con 7, pues ya habremos colocado dos anteriormente, y asi sucesivamente hasta llegar al ultimo lugar, donde unicamente contamos con un candidato, visto de forma grafica seria:

$$
\begin{matrix}
10 candidatos & 9 cantidatos & 8 candidatos & 7 candidatos & 6 candidatos & 5 candidatos & 4 candidatos & 3 candidatos & 2 candidatos & 1 cantidato\\
\vdots & \vdots & \vdots & \vdots & \vdots & \vdots & \vdots & \vdots & : & .\\
\vdots & \vdots & \vdots & \vdots & \vdots & : & . & \\
\vdots & \vdots & : & . & \\
. \\
\end{matrix}
$$

Visto de esta manera es sencillo ver como sacar los posibles formas de acomodarlos, simplemente bastaria con multiplicar la cantidad de cantidatos posibles que hay por lugar, obteniendo que para este caso $10\cdot 9\cdot 8\cdot 7\cdot 6\cdot 5\cdot 4\cdot 3\cdot 2\cdot 1$ son las formas posibles de formarlos, lo cual tambien se puede reescribir como 10! (10 factorial)

## Problema (Combinatoria)

Imagina que deseas sentar a 10 personas, pero solo cuentas con 6 sillas, cuantas formas posibles hay de sentarlos.

Pues este problema es algo diferente al anterior, pues aunque aun contamos con las 10 personas, ahora solo existen 6 lugares donde pueden sentarse, asi que, como podemos resolver este problema?. Pues simple, asumamos que no hay 6, sino 10 lugares, de esta manera podremos operar como anteriormente lo hicimos, posteriormente le "restamos" las posibilidades hipoteticas y tendremos el resultado real. Usando la logica anterior, se tiene 10 lugares y 10 personas por sentar, facil. 10!, muy bien, ya vamos a la mitad del camino, ahora solo falta quitar los 4 lugares que nosotros aplicamos, razonemos; si hay 10 personas para el primer lugar tendremos 10 canidatos para sentar, para el segundo 9, para el tercero 8... y asi hasta que lleguemos al sexto lugar, que es el ultimo asiento real, en este punto solo contamos con 5 personas candidatas a ser sentados, asi que elegimos a una bien, ahora empiezan los lugares imaginarios, para el septima teoricamente hay 4 personas candidatas, para el octavo 3, para el noveno 2 y para el decimo solamten 1.


$\quad \quad LUGARES \quad REALES  \quad \quad \quad \quad \quad \quad \quad  \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad LUGARES \quad IMAGINARIOS$

$$
\begin{matrix}
10 candidatos & 9 cantidatos & 8 candidatos & 7 candidatos & 6 candidatos & 5 candidatos & | & 4 candidatos & 3 candidatos & 2 candidatos & 1 cantidato\\
\vdots & \vdots & \vdots & \vdots & \vdots & \vdots & | & \vdots & \vdots & : & .\\
\vdots & \vdots & \vdots & \vdots & \vdots & : & | & . & \\
\vdots & \vdots & : & . & \\
. \\
\end{matrix}
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

## Suma de Gauss (Teoria de Numeros)

Supongamos que te pidieran hacer una suma ingentemente grande que tal una suma de $n$ terminos, similar a esto $1+2+3+4+5+6+7+8+9+...+n$ ¿que harias? seguro que piensas que algo asi es imposible, pues ¿como voy a sumar algo que ni siquiera se donde termina? Pues la realidad es que si es posible, y fue precisamente este problema el que llevo a un joven Gauss a desarrollar esta curiosa suma ahora lleva su nombre.

Imaginemos que ahora en lugar de pedirte que sumes hasta $n$ , te pidiera que lo hicieras del 1 al 10, si eres agil los obtendras relativamente facil, pero que tal si fuera del 1 al 100 o del 1 al 1000? ya no parece tan sencillo verdad? pero que tal si te dijera que hay una forma relativamente facil de obtener todos estos casos, sin que te tomara mas de 5 minutos.

El truco consiste en agarrar la suma y duplicarla colocando este clon justo abajo de nuestra original, solamente que invertida, tal que debajo del primer numero que el ultimo, del segundo el penultimo, y asi... si hacemos la suma verticalmente nos daremos cuenta que es la misma cifra en todos los lugares, por lo que solo debemos sumaldo, al ser el mismo numero pormos multiplicarlo, el resultado de esa multiplicacion lo dividiremos entre dos, pues hicimos la suma deseada dos veces y nos quedaria asi de manera grafica:

$$\begin{matrix}
1 &+& 2 &+& 3 &+& 4 &+& 5 &+& 6 &+& 7 &+& 8 &+& 9 &+& 10 \\
10 &+& 9 &+& 8 &+& 7 &+& 6 &+& 5 &+& 4 &+& 3 &+& 2 &+& 1 \\
11 &+& 11 &+& 11 &+& 11 &+& 11 &+& 11 &+& 11 &+& 11 &+& 11 &+& 11 
\end{matrix}$$

Entonces podemos deducir que 
$$\frac{n\left(n+1\right)}{2}=\frac{n^2+n}{2} \quad n\in \mathbb{Z}^+$$


## Problema (Teoria de numeros)

Resuelve los casos para $n$ tal que $\frac{1+3+5+...+\left(2n-1\right)}{2+4+6+...+2n}=\frac{2006}{2007}$

Si somos observadores nos daremos cuenta que los elementos de la izquierda son sucesiones, pero no cualquier sucesion, sino unas verdaderamente unicas si miramos los terminos de arriba nos daremos cuenta que son la suma de los impares y como sabemos esto es igual al numeor siguiente, al cuadrado, tal que $1+3+5+...+(2n-1)=n²$ . Para el termino de abajo se requiere algo mas de ingenio, pues si nos damos cuenta son la suma de todos los pares hasta $n$ , pero si lo dividimos entre dos es decir factorizar sacando el elemento comun, el dos, obtenemos que $2+4+6+...+2n=2(1+2+3+...+n)$ este termino que esta dentro del parentesis es una suma del 1 hasta $n$ terminos, asi que es una sucesion de suma de Gauss, por lo que podemos decir que la sucesion es equivalente a la siguiente ecuacion $\left(1+2+4+...+n\right)=\frac{n\left(n+1\right)}{2}$ a este resultado lo podemos simplificar sin perder su generalizacion, de modo que $\frac{n\left(n+1\right)}{\:2}=\frac{n^2+n}{2}$ con esto ya podemos reemplazarlo en la sucesion anterior, tal que $2\left(1+2+4+...+n\right)=2\left(\frac{n^2+n}{2}\right)$ si nos concentramos en este resultado podremos notar que la division y multiplicacion se contrarestan $\therefore 2\left(\frac{n^2+n}{2}\right)=n^2+n$ , bien ya que lo tenemos solo falta reemplazar estas equivalencias por sus terminos originales, de modo que $\\frac{1+3+5+...+\left(2n-1\right)}{2+4+6+...+2n}=\frac{n^2}{n^2+n}$ sustituimos $\Longrightarrow \frac{n^2}{n^2+n}=\frac{2006}{2007}$ para este punto solo hara falta algo de algebra , de modo que multiplicamos el denominador de ambos lados por el numeroador del otro tal que 
$$\left(2007\right)\frac{n^2}{n^2+n}=\left(2007\right)\frac{2006}{2007}\Longrightarrow \frac{2007n^2}{n^2+n}=2006,\:\left(n^2+n\right)\frac{2007n^2}{n^2+n}=\left(n^2+n\right)\left(2006\right)\Longrightarrow 2007n^2=2006n^2+2006n,\left(2007n^2\right)-\left(2006n^2\right)=\left(2006n^2+2006n\right)-\left(2006n^2\right)\Longrightarrow n^2=2006n,\frac{n^2}{n}=\frac{2006}{n}\Longrightarrow n=2006$$ 
Finalmente con esto se concluye que los casos donde $\exists n\in \mathbb{Z}^+$ tal que $\frac{1+3+5+...+\left(2n-1\right)}{2+4+6+...+2n}=\frac{2006}{2007} \quad n=2006$

## Factorizacion (Algebra)

Imagina que te dan $ax²+bx+c=0$ y te pidieran despejar $x$ hay dos maneras de hacerlo, con la formula general o factorizando. Al factorizar hablamos de esto $\left(x1,+\alpha \right)\left(x1,+B\right)=0$ , permiteme explicarte, si tu lo desarrollas llegas a que $\left(x1,+\alpha \right)\left(x2,+B\right)=x^2+Bx+\alpha \:x+\alpha \:B$ , si simplificamos a $Bx+\alpha \:\:x=\left(B+\alpha \:\:\right)x$ tal que $x^2+Bx+\alpha \:x+\alpha \:B=x^2+\left(B+\alpha \:\right)x+\alpha \:B$ pero fijate que esta nueva forma se parece mucho a la expresion original, y eso es porque son lo mismo, siempre y cuando se cumpla una condicion que atenderemos mas adelante. Si no me crees evalua $\left(B+a\right)x$ es un termino que depende de la $x$ siendo la multiplicacion de una variable y un termino independiente, al igual que $bx$ por lo que $\left(B+\alpha \right)x=bx$ y dentro de esto tambien podemos deducir que $\frac{\left(B+\alpha \right)x}{x}=\frac{bx}{x}\therefore B+\alpha =b$ lo cual por si solo ya es una gran deduccion. Pero sigamos, si somos observadores, el producto de $\alpha \:B$ es un termino independiente a la $x$ al igual que $c$ por lo que no es dificil de deducir que $\alpha \:B=c$. Pero ahora ¿que hay del $ax²$ y $x²$ ? ¿acaso tambien son iguales? Pues aqui entra la condicion de antes, pues para que $ax^2+bx+c=x^2+\left(B+\alpha \:\right)x+\alpha \:B,a=1$ por lo que si queremos generalizar la expresion tendiramos que decir algo similar a esto $\frac{ax^2+bx+c}{a}=x^2+\left(B+\alpha \:\right)x+\alpha \:B$ . Pero para fines practicos forzaremos a que $a=1$ haciendo lo de dividir toda la expresion entre $a$ para que ahora si $x^2+bx+c=x^2+\left(B+\alpha \right)x+\alpha B=0$ tal que $\left(x1+\alpha \right)\left(x2+B\right)=0$. Con esto podemos deducir que para que esa ultima condicion se cumpla $x1=-\alpha ,x2=-B$ tal que $\left(-\alpha +\alpha \right)\left(-B+B\right)=\left(\alpha -\alpha \right)\left(B-B\right)=0$. Esto nos da una conclusion muy importante pues para encontrar las soluciondes de $x$ basta con que encontremos a $\alpha$ y $B$ tal que sumados den $bx$ pues $bx=(B+\alpha)x,y$ multiplicados den $c$ pues $c=\alpha B$ tal que $(x1+\alpha)(x2+B)=0$ pues se concluye que $\frac{ax^2+bx+c}{a}=x^2+\left(B+\alpha \right)x+\alpha B=\left(x1+\alpha \right)\left(x2+B\right)=0$ tal que $x1=-\alpha$ y $x2=-B$

## Metodo de Po-Shen Loh (Algebra)

El mayor problema con la factorizacion es que, a priori, solo funciona cuando $x,x2\in \mathbb{Z}$ pues en si el metodo consiste en encontrar un $a$ y $B$ simplemente adivinando tal que $(B+a)=b,aB=c$ pero evidentemente ponerse a adivinar $a$ y $B$ cuando estos sean racionales, irracionales o complejos es simplemente imposible, o eso mismo penso Po-Shen Loh, antes de desarrollar este metodo.

El truco esta en que $ax²+bx+c=x²+(B+a)x+aB=0$ , si $a,B\in \mathbb{R},a\ne B$ para que se cumpla la forma $\left(x1+a\right)\left(x2+B\right)=0,\left(B+a\right)=b$ y $aB=c$ intuitivamente probariamos con la multiplicacion pues hay menos $a$ y $B$ que multiplicados dan $c$ de los que hay tal que sumados de $b$. El truco empieza aqui, pues comenzamos que cumplen, usaremos la mas simple que es $B=\frac{b}{2},a=\frac{b}{2}$ tal que $\frac{b}{2}+\frac{b}{2}=b$ pero esto va en contra de $a\ne B$ ademas salvo en los casos especificos $\left(\frac{b}{2}\right)\left(\frac{b}{2}\right)\ne c$ asi que ¿como solucionamos esto? simple asumimos que $B=\frac{b}{2}+u,a=\frac{b}{2}-u$ tal que $\left(\frac{b}{2}+u\right)+\left(\frac{b}{2}-u\right)=b$ pues las $u$ se cancelan y obtendremos la expresion $\frac{b}{2}+\frac{b}{2}=b$ . La razon de esta forma de ver a $a$ y $B$ es que independientemente de su valor real, estas cifras siempre daran $b$ de modo que si $a$ es muy grande $B$ sera muy pequeña y viceversa y al promediar $a$ y $B$ hacemos que esta proporcionalidad sea directa reflejandose en el termino u.
Ahora bien, para despejar $u$ tendremos que atender a $c=aB$ reemplazando tenemos que $c=\left(\frac{b}{2}-u\right)\left(\frac{b}{2}+u\right)$ al ser una diferencia de cuadrados $c=\left(\frac{b}{2}\right)^2-u^2$ si resolvemos el parentesis $\left(\frac{b}{2}\right)^2=\left(\frac{b}{2}\right)\left(\frac{b}{2}\right)=\frac{6^2}{4}\therefore c=\frac{b^2}{4}-u^2$ ahora a la $u²$ la pasamos a la izquierda sumando y a $c$ a la derecha restando tal que $u^2=\frac{b^2}{4}-c$ simplificando $u=\sqrt[\pm ]{\frac{b^2}{4}-c}\therefore a=\frac{b}{2}-\sqrt{\frac{b^2}{4}-c}$ , $B=\frac{b}{2}+\sqrt{\frac{b^2}{2}-c}$ $\Rightarrow$ $b=\left(\frac{b}{2}+\sqrt{\frac{b^2}{4}-c}\right)+\left(\frac{b}{2}-\sqrt{\frac{b^2}{4}-c}\right)$ , $c=\left(\frac{b}{2}-\sqrt{\frac{b^2}{4}-c}\right)\left(\frac{b}{2}+\sqrt{\frac{b^2}{4}-c}\right)$

## Problema (Algebra)


