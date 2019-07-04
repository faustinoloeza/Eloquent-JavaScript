{{meta {load_files: ["code/intro.js"]}}}

# Introducción

{{quote {author: "Ellen Ullman", title: "Close to the Machine: Technophilia and its Discontents", chapter: true}

Creemos que estamos creando el sistema para nuestros propios fines. Creemos que lo estamos haciendo a nuestra propia imagen ... Pero la computadora no es como nosotros. Es una proyección de una parte muy delgada de nosotros mismos: la parte dedicada a la lógica, el orden, la regla y la claridad.

quote}}

{{figure {url: "img/chapter_picture_00.jpg", alt: "Picture of a screwdriver and a circuit board", chapter: "framed"}}}

Este es un libro sobre la instrucción de computadoras. Las computadoras son tan comunes como los destornilladores en la actualidad, pero son un poco más complejas, y hacer que hagan lo que usted quiere que hagan no siempre es fácil.


Si la tarea que tiene para su computadora es una tarea común y bien entendida, como mostrarle su correo electrónico o actuar como una calculadora, puede abrir la *aplicación* correspondiente  y ponerse a trabajar. Pero para tareas únicas o abiertas, probablemente no haya ninguna aplicación.


Ahí es donde puede entrar la programación. Programar es el acto de construir un programa con un conjunto de instrucciones precisas que le dicen a una computadora qué hacer. Debido a que las computadoras son bestias tontas y pedantes, la programación es fundamentalmente tediosa y frustrante.

{{index [programming, "joy of"], speed}}

Afortunadamente, si puedes superar ese hecho, y tal vez incluso disfrutar del rigor de pensar en términos que las máquinas tontas pueden manejar, la programación puede ser gratificante. Te permite hacer cosas en segundos que te llevarían una eternidad a mano. Es una forma de hacer que su computadora haga cosas que antes no podía hacer. Y proporciona un maravilloso ejercicio de pensamiento abstracto.

La mayoría de la programación se realiza con lenguajes de programación. Un lenguaje de programación es un lenguaje construido artificialmente utilizado para instruir a las computadoras. Es interesante que la forma más efectiva que hemos encontrado para comunicarnos con una computadora se preste mucho de la manera en que nos comunicamos entre nosotros. Al igual que los lenguajes humanos, los lenguajes informáticos permiten que las palabras y frases se combinen de nuevas maneras, lo que hace posible expresar conceptos siempre nuevos.

{{index [JavaScript, "availability of"], "casual computing"}}

En un punto, las interfaces basadas en el lenguaje, como las ventanas de BASIC y DOS de los años 1980 y 1990, fueron el método principal de interacción con las computadoras. Han sido reemplazados en gran parte por interfaces visuales, que son más fáciles de aprender pero ofrecen menos libertad. Los lenguajes informáticos siguen ahí, si sabes dónde buscar. Uno de estos lenguajes, JavaScript, está incorporado en cada navegador web moderno y, por lo tanto, está disponible en casi todos los dispositivos.

{{indexsee "web browser", browser}}

Este libro intentará familiarizarte lo suficiente con este lenguaje para hacer cosas útiles y sorprendentes con él.

## En la programación

{{index [programming, "difficulty of"]}}

Además de explicar JavaScript, presentaré los principios básicos de la programación. Resulta que la programación es difícil. Las reglas fundamentales son simples y claras, pero los programas construidos sobre estas reglas tienden a ser lo suficientemente complejos como para introducir sus propias reglas y complejidad. En cierto modo, estás construyendo tu propio laberinto y podrías perderte en él.

{{index learning}}

Habrá momentos en que la lectura de este libro se siente terriblemente frustrante. Si eres nuevo en la programación, habrá un montón de material nuevo para digerir. Gran parte de este material se combinará en formas que requieran que usted haga conexiones adicionales.

Depende de usted hacer el esfuerzo necesario. Cuando tenga dificultades para seguir el libro, no saque ninguna conclusión sobre sus propias capacidades. Estás bien, solo necesitas mantenerte en ello. Tome un descanso, vuelva a leer algún material y asegúrese de leer y comprender los programas y ejercicios de ejemplo. Aprender es un trabajo duro, pero todo lo que aprendes es tuyo y facilitará el aprendizaje posterior.

{{quote {author: "Ursula K. Le Guin", title: "The Left Hand of Darkness"}

{{index "Le Guin, Ursula K."}}

Cuando la acción no es rentable, reúne información; Cuando la información crece sin rentabilidad, el sueño.

quote}}

{{index [program, "nature of"], data}}

Un programa es muchas cosas. Es un fragmento de texto escrito por un programador, es la fuerza de dirección que hace que la computadora haga lo que hace, es información en la memoria de la computadora, pero controla las acciones realizadas en esta misma memoria. Las analogías que intentan comparar programas con objetos con los que estamos familiarizados tienden a quedarse cortos. Una que encaja superficialmente es la de una máquina: muchas partes separadas tienden a estar involucradas y, para hacer que todo funcione, debemos considerar las formas en que estas partes se interconectan y contribuyen al funcionamiento del conjunto.

Una computadora es una máquina física que actúa como un host para estas máquinas inmateriales. Las computadoras mismas pueden hacer cosas estúpidamente simples. La razón por la que son tan útiles es que hacen estas cosas a una velocidad increíblemente alta. Un programa puede combinar ingeniosamente una cantidad enorme de estas acciones simples para hacer cosas muy complicadas.

{{index [programming, "joy of"]}}

Un programa es un edificio de pensamiento. Es gratis construirlo, no pesa y crece fácilmente bajo nuestras manos.

Pero sin cuidado, el tamaño y la complejidad de un programa crecerán fuera de control, confundiendo incluso a la persona que lo creó. Mantener los programas bajo control es el principal problema de la programación. Cuando un programa funciona, es hermoso. El arte de la programación es la habilidad de controlar la complejidad. El gran programa es tenue, simplificado en su complejidad.

{{index "programming style", "best practices"}}

Algunos programadores creen que esta complejidad se gestiona mejor utilizando solo un pequeño conjunto de técnicas bien entendidas en sus programas. Han compuesto reglas estrictas ("mejores prácticas") que prescriben los formularios que los programas deben tener y se mantienen cuidadosamente dentro de su pequeña zona segura.

{{index experiment}}

Esto no solo es aburrido, es ineficaz. Los nuevos problemas a menudo requieren nuevas soluciones. El campo de la programación es joven y todavía se está desarrollando rápidamente, y es lo suficientemente variado para tener espacio para enfoques totalmente diferentes. Hay muchos errores terribles que cometer en el diseño del programa, y debe seguir adelante y cometerlos para que los entienda. Un sentido de cómo se ve un buen programa se desarrolla en la práctica, no se aprende de una lista de reglas.

## Why language matters

{{index "programming language", "machine code", "binary data"}}

In the beginning, at the birth of computing, there were no programming
languages. Programs looked something like this:

```{lang: null}
00110001 00000000 00000000
00110001 00000001 00000001
00110011 00000001 00000010
01010001 00001011 00000010
00100010 00000010 00001000
01000011 00000001 00000000
01000001 00000001 00000001
00010000 00000010 00000000
01100010 00000000 00000000
```

{{index [programming, "history of"], "punch card", complexity}}

That is a program to add the numbers from 1 to 10 together and print
out the result: `1 + 2 + ... + 10 = 55`. It could run on a simple,
hypothetical machine. To program early computers, it was necessary to
set large arrays of switches in the right position or punch holes in
strips of cardboard and feed them to the computer. You can probably
imagine how tedious and error-prone this procedure was. Even writing
simple programs required much cleverness and discipline. Complex ones
were nearly inconceivable.

{{index bit, "wizard (mighty)"}}

Of course, manually entering these arcane patterns of bits (the ones
and zeros) did give the programmer a profound sense of being a mighty
wizard. And that has to be worth something in terms of job
satisfaction.

{{index memory, instruction}}

Each line of the previous program contains a single instruction. It
could be written in English like this:

 1. Store the number 0 in memory location 0.
 2. Store the number 1 in memory location 1.
 3. Store the value of memory location 1 in memory location 2.
 4. Subtract the number 11 from the value in memory location 2.
 5. If the value in memory location 2 is the number 0,
    continue with instruction 9.
 6. Add the value of memory location 1 to memory location 0.
 7. Add the number 1 to the value of memory location 1.
 8. Continue with instruction 3.
 9. Output the value of memory location 0.

{{index readability, naming, binding}}

Although that is already more readable than the soup of bits, it is
still rather obscure. Using names instead of numbers for the
instructions and memory locations helps.

```{lang: "text/plain"}
 Set “total” to 0.
 Set “count” to 1.
[loop]
 Set “compare” to “count”.
 Subtract 11 from “compare”.
 If “compare” is zero, continue at [end].
 Add “count” to “total”.
 Add 1 to “count”.
 Continue at [loop].
[end]
 Output “total”.
```

{{index loop, jump, "summing example"}}

Can you see how the program works at this point? The first two lines
give two memory locations their starting values: `total` will be used
to build up the result of the computation, and `count` will keep track
of the number that we are currently looking at. The lines using
`compare` are probably the weirdest ones. The program wants to see
whether `count` is equal to 11 to decide whether it can stop
running. Because our hypothetical machine is rather primitive, it can
only test whether a number is zero and make a decision based
on that. So it uses the memory location labeled `compare` to compute
the value of `count - 11` and makes a decision based on that value.
The next two lines add the value of `count` to the result and
increment `count` by 1 every time the program has decided that `count`
is not 11 yet.

Here is the same program in JavaScript:

```
let total = 0, count = 1;
while (count <= 10) {
  total += count;
  count += 1;
}
console.log(total);
// → 55
```

{{index "while loop", loop, [braces, block]}}

This version gives us a few more improvements. Most important, there
is no need to specify the way we want the program to jump back and
forth anymore. The `while` construct takes care of that. It continues
executing the block (wrapped in braces) below it as long as the
condition it was given holds. That condition is `count <= 10`, which
means “_count_ is less than or equal to 10”. We no longer have to
create a temporary value and compare that to zero, which was just an
uninteresting detail. Part of the power of programming languages is
that they can take care of uninteresting details for us.

{{index "console.log"}}

At the end of the program, after the `while` construct has finished,
the `console.log` operation is used to write out the result.

{{index "sum function", "range function", abstraction, function}}

Finally, here is what the program could look like if we happened to
have the convenient operations `range` and `sum` available, which
respectively create a ((collection)) of numbers within a range and
compute the sum of a collection of numbers:

```{startCode: true}
console.log(sum(range(1, 10)));
// → 55
```

{{index readability}}

The moral of this story is that the same program can be expressed in
both long and short, unreadable and readable ways. The first version of the
program was extremely obscure, whereas this last one is almost
English: `log` the `sum` of the `range` of numbers from 1 to 10. (We
will see in [later chapters](data) how to define operations like `sum`
and `range`.)

{{index ["programming language", "power of"], composability}}

A good programming language helps the programmer by allowing them to
talk about the actions that the computer has to perform on a higher
level. It helps omit details, provides convenient building blocks
(such as `while` and `console.log`), allows you to define your own
building blocks (such as `sum` and `range`), and makes those blocks
easy to compose.

## What is JavaScript?

{{index history, Netscape, browser, "web application", JavaScript, [JavaScript, "history of"], "World Wide Web"}}

{{indexsee WWW, "World Wide Web"}}

{{indexsee Web, "World Wide Web"}}

JavaScript was introduced in 1995 as a way to add programs to web
pages in the Netscape Navigator browser. The language has since been
adopted by all other major graphical web browsers. It has made modern
web applications possible—applications with which you can interact
directly without doing a page reload for every action. JavaScript is also
used in more traditional websites to provide various forms of
interactivity and cleverness.

{{index Java, naming}}

It is important to note that JavaScript has almost nothing to do with
the programming language named Java. The similar name was inspired by
marketing considerations rather than good judgment. When JavaScript
was being introduced, the Java language was being heavily marketed and
was gaining popularity. Someone thought it was a good idea to try to
ride along on this success. Now we are stuck with the name.

{{index ECMAScript, compatibility}}

After its adoption outside of Netscape, a ((standard)) document was
written to describe the way the JavaScript language should work so
that the various pieces of software that claimed to support JavaScript
were actually talking about the same language. This is called the
ECMAScript standard, after the Ecma International organization that
did the standardization. In practice, the terms ECMAScript and
JavaScript can be used interchangeably—they are two names for the same
language.

{{index [JavaScript, "weaknesses of"], debugging}}

There are those who will say _terrible_ things about JavaScript. Many
of these things are true. When I was required to write something in
JavaScript for the first time, I quickly came to despise it. It would
accept almost anything I typed but interpret it in a way that was
completely different from what I meant. This had a lot to do with the
fact that I did not have a clue what I was doing, of course, but there
is a real issue here: JavaScript is ridiculously liberal in what it
allows. The idea behind this design was that it would make programming
in JavaScript easier for beginners. In actuality, it mostly makes
finding problems in your programs harder because the system will not
point them out to you.

{{index [JavaScript, "flexibility of"], flexibility}}

This flexibility also has its advantages, though. It leaves space for
a lot of techniques that are impossible in more rigid languages, and
as you will see (for example in [Chapter ?](modules)), it can be used
to overcome some of JavaScript's shortcomings. After ((learning)) the
language properly and working with it for a while, I have learned to
actually _like_ JavaScript.

{{index future, [JavaScript, "versions of"], ECMAScript, "ECMAScript 6"}}

There have been several versions of JavaScript. ECMAScript version 3
was the widely supported version in the time of JavaScript's ascent to
dominance, roughly between 2000 and 2010. During this time, work was
underway on an ambitious version 4, which planned a number of radical
improvements and extensions to the language. Changing a living, widely
used language in such a radical way turned out to be politically
difficult, and work on the version 4 was abandoned in 2008, leading to
a much less ambitious version 5, which made only some uncontroversial
improvements, coming out in 2009. Then in 2015 version 6 came out, a
major update that included some of the ideas planned for version 4.
Since then we've had new, small updates every year.

The fact that the language is evolving means that browsers have to
constantly keep up, and if you're using an older browser, it may not
support every feature. The language designers are careful to not make
any changes that could break existing programs, so new browsers can
still run old programs. In this book, I'm using the 2017 version of
JavaScript.

{{index [JavaScript, "uses of"]}}

Web browsers are not the only platforms on which JavaScript is used.
Some databases, such as MongoDB and CouchDB, use JavaScript as their
scripting and query language. Several platforms for desktop and server
programming, most notably the ((Node.js)) project (the subject of
[Chapter ?](node)), provide an environment for programming JavaScript
outside of the browser.

## Code, and what to do with it

{{index "reading code", "writing code"}}

_Code_ is the text that makes up programs. Most chapters in this book
contain quite a lot of code. I believe reading code and writing ((code))
are indispensable parts of ((learning)) to program. Try to not just
glance over the examples—read them attentively and understand them.
This may be slow and confusing at first, but I promise that you'll
quickly get the hang of it. The same goes for the ((exercises)). Don't
assume you understand them until you've actually written a working
solution.

{{index interpretation}}

I recommend you try your solutions to exercises in an actual
JavaScript interpreter. That way, you'll get immediate feedback on
whether what you are doing is working, and, I hope, you'll be tempted
to ((experiment)) and go beyond the exercises.

{{if interactive

When reading this book in your browser, you can edit (and run) all
example programs by clicking them.

if}}

{{if book

{{index download, sandbox, "running code"}}

The easiest way to run the example code in the book, and to experiment
with it, is to look it up in the online version of the book at
[_https://eloquentjavascript.net_](https://eloquentjavascript.net/). There,
you can click any code example to edit and run it and to see the
output it produces. To work on the exercises, go to
[_https://eloquentjavascript.net/code_](https://eloquentjavascript.net/code),
which provides starting code for each coding exercise and allows you
to look at the solutions.

if}}

{{index "developer tools", "JavaScript console"}}

If you want to run the programs defined in this book outside of the
book's website, some care will be required. Many examples stand on their
own and should work in any JavaScript environment. But code in later
chapters is often written for a specific environment (the browser or
Node.js) and can run only there. In addition, many chapters define
bigger programs, and the pieces of code that appear in them depend on
each other or on external files. The
[sandbox](https://eloquentjavascript.net/code) on the website provides
links to Zip files containing all the scripts and data files
necessary to run the code for a given chapter.

## Overview of this book

This book contains roughly three parts. The first 12 chapters discuss
the JavaScript language. The next seven chapters are about web
((browsers)) and the way JavaScript is used to program them. Finally,
two chapters are devoted to ((Node.js)), another environment to
program JavaScript in.

Throughout the book, there are five _project chapters_, which describe
larger example programs to give you a taste of actual programming. In
order of appearance, we will work through building a [delivery
robot](robot), a [programming language](language), a [platform
game](game), a [pixel paint program](paint), and a [dynamic
website](skillsharing).

The language part of the book starts with four chapters that introduce
the basic structure of the JavaScript language. They introduce
[control structures](program_structure) (such as the `while` word you
saw in this introduction), [functions](functions) (writing your own
building blocks), and [data structures](data). After these, you will
be able to write basic programs. Next, Chapters [?](higher_order) and
[?](object) introduce techniques to use functions and objects to write
more _abstract_ code and keep complexity under control.

After a [first project chapter](robot), the language part of the book
continues with chapters on [error handling and bug fixing](error),
[regular expressions](regexp) (an important tool for working with
text), [modularity](modules) (another defense against complexity), and
[asynchronous programming](async) (dealing with events that take
time). The [second project chapter](language) concludes the first part
of the book.

The second part, Chapters [?](browser) to [?](paint), describes the
tools that browser JavaScript has access to. You'll learn to display
things on the screen (Chapters [?](dom) and [?](canvas)), respond to
user input ([Chapter ?](event)), and communicate over the network
([Chapter ?](http)). There are again two project chapters in this
part.

After that, [Chapter ?](node) describes Node.js, and [Chapter
?](skillsharing) builds a small website using that tool.

{{if commercial

Finally, [Chapter ?](fast) describes some of the considerations that
come up when optimizing JavaScript programs for speed.

if}}

## Typographic conventions

{{index "factorial function"}}

In this book, text written in a `monospaced` font will represent
elements of programs—sometimes they are self-sufficient fragments, and
sometimes they just refer to part of a nearby program. Programs (of
which you have already seen a few) are written as follows:

```
function factorial(n) {
  if (n == 0) {
    return 1;
  } else {
    return factorial(n - 1) * n;
  }
}
```

{{index "console.log"}}

Sometimes, to show the output that a program produces, the
expected output is written after it, with two slashes and an arrow in
front.

```
console.log(factorial(8));
// → 40320
```

Good luck!
