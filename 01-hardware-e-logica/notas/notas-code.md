# Code, Charles Petzold

## Primeiro Capítulo - Best Friends
O primeiro capítulo fala sobre a história de dois melhores amigos que moram um na frente do outro. Eles sempre queriam continuar conversando mesmo depois da hora de dormir, como seu quartos tinham janelas viradas, tentavam se comunicar com gestos e movimentação do corpo, mas ficava muito difícil para entender o que o outro queria falar.
Como era hora de dormir e nenhum deles tinha celular, precisavam arrumar um jeito de entender o que o outro colega queria dizer. Depois de um tempo tentaram se comunicar usando uma lanterna, eles desenhavam no ar o formato das letras, mas logo perceberam que era muito díficil entender também, não sabiam dizer quando uma letra começava e a outra acabava e se perdiam na metade do caminho.
Tentaram outra solução, dessa vez arrumaram um tipo de código para conseguir identificar as letras que estavam tentando escrever, para cada letra do alfabeto tinha um número certo de piscadas que a lanterna precisava dar, começava assim: A era 1 piscada, B era 2 piscadas, C era 3 piscadas.... Z era 26, dessa vez ficava fácil identificar qual letra o outro estava tentando escrever, mas mesmo assim dava muito trabalho para se comunicar, dependendo da frase era preciso piscar muitas vezes a lanterna, isso dificultava o entendimento da frase completa.
No final das contas eles descobriram outra solução, que facilitaria muito a escrita das frases, e a identificação das letras, o código Morse. Ele pontos e traços para identificar as letras, então se você quisesse escrever Z, não precisava dar 26 piscadas com a lanterna, era só dar duas piscadas lentas e duas rápidas e depois uma pequena palsa para escrever a próxima letra.

## Segundo Capítulo - Codes and Combination
Dentro do Código Morse podemos ter infinitas combinações de pontos e traços para formar diversos caracteres, usando somente um símbolo no código morse conseguimos representar apenas 2 letras:
- . = E
- - = T

Se adicionarmos mais um símbolo, conseguimos representar mais 4 letras além das duas que fizemos
- .. = I
- .- = A
- -. = N
- -- = M

Se adicionarmos mais um, conseguimos representar mais 8 além das outras letras, repare que toda vez que adicionamos mais um símbolo para representar um letra, o número de possíbilidades dobra comparado ao quantidade de símbolos anterior, isso porque o código Morse é **binário**, ou seja, cada "casa" do código Morse representa uma potência de dois.

2¹ + 2² + 2³...
Com uma casa temos duas possibilidades
Com duas casas temos quatro possibilidades
Com três temos oito
Com quatro temos dezesseis...

## Terceiro Capítulo - Braille and Binary Codes
O código Morse não é a única forma de tranformar linguagem escrita em códigos interpretáveis, existe também o Braille, que foi criado por um estudande Frânces cego, e basicamente usa 6 "espaços" para interpretar algum significado, ao contrário de Morse, dependendo do contexto, um símbolo em Braille pode dar outro significado para um carácter, podemos usar um símbolo só para escrever uma palavra inteira, ou usar um símbolo para Letras Maiúsculas, basicamente usa sequências e padrões para mudar o significado.


## Quarto Capítulo - Anatomy of a Flashlight
Circuítos Elétricos não são nada mais do que um Círculo, quando esse círculo é rompido, o circuíto é desligado.
Toda a matéria do nosso planeta é feito de átomos, e eles são positivos (prótons) e negativos (neutrons e elétrons), a eletricidade nada mais é que os életrons viajando de um átomo para outro.
Isso acontece em uma bateria, ela tem dois polos, o negativo (onde sobram elétrons) e o positivo (onde faltam elétrons) ela age como uma bomba, explodindo os elétrons de um polo para o outro.
Existem 3 grandezas em circuítos elétricos:
- Voltagem (Volts, V): É a força ou potência que os elétrons passam pelo circuito, uma analogia é a pressão que uma água passa por um cano;
- Corrente(Amperagem, I): É a quantidade de elétrons que passa por segundo pelo circuíto, uma analogia é a quantidade de água que passa por segundo em um encamento;
- Resistência (Ohm, R): É a dificuldade que os elétrons tem para passar no circuíto, uma analogia é a o tamanho do cano que a água passa;

**A lei de Ohm**
$$I = \frac{E}{R}$$

Por fim, o papel de um interruptor é controlar a carga elétrica do circuíto, quando o interruptor está desligado, ele deixa o fluxo seguir normalmente, quando ele liga, ele desliga todo o circuíto. Não existe meio termo, ou o circuíto está ligado, ou desligado.

## Quinto Capítulo - Communicating Around Corners
Pressupomos que não conseguimos mais usar a luz da lanterna para nos comunicar através de uma janela, agora vamos precisar usar um circuito elétrico, onde colocamos um lâmpada e um interruptor em cada casa, assim, se eu ligar o interruptor na minha casa a lâmpada da outra casa vai ligar, e vice-versa. Repare que para esse circuíto, precisariamos de 4 fios, mas para economizarmos, poderíamos usar somente um fio **Comum**, para ligarmos e usarmos ele para compartilhar a condução elétrica entre duas lâmpadas e um interruptor, assim conseguíriamos reduzir de 4 para 3 fios.
Pensando em podermos econimizar mais fios ainda, podemos usar a terra **(Ground)**, porque ela é um grande condutor, mas nesse caso, não esteríamos mais utilizando somente baterias de 1.5v e sim um potencial maior, mas assim como a terra é um bom condutor de elétrons, também é um "mar de elétrons" então isso aumentaria muito a **Resistência**, então não conseguiríamos utilizar toda a extensão da terra para podermos ligarmos o circuíto, porque quanto mais longo é o circuíto, mas a lâmpada perderia força e chegaria ao ponto de apaga-la.

## Sexto Capítulo - Logic with Switches
A álgebra booleana é um tipo de matemática diferente da álgebra convencional, os operadores + e x na verdade são usados para outras operações dentro dela. O + significa União, e o x significa Interseção, invés de usarmos números na álgebra booleana, usamos **classes**.
Por exemplo, temos dois tipos de classes de gatos, Machos (M) e Fêmeas (F), também podemos ter classes das cores de gatos, como Branco (B), Preto (P), Laranja (L) agora vamos para um exemplo de operação booleana:
M x B
Isso é um gato macho branco.
Supondo que uma pessoa vá em um petshop e peça um gato que não pode ser Macho, e nem ter as cores Branco e nem Preto, então se eu chegasse com um gato Fêmea e Laranja essa pessoa ficaria satisfeita:
!M x !B x !P = F x L

A mesma coisa acontece para classes binárias, 0 e 1, ou seja:
0 x 0 = 0
0 x 1 = 0
1 x 0 = 0
1 x 1 = 1

0 + 0 = 0
0 + 1 = 1
1 + 0 = 1
1 + 1 = 1

Isso basicamente se encaixa em circuítos elétricos que vimos nos últimos capítulos, dependendo da lógica aplicada um circuíto pode estar ligado ou desligado.

## Sétimo Capítulo - Telegraphs and Relays
O telégrafo foi um dispositivo inventado para se comunicar com agilidade e através de longas distâncias, basicamente funcionava como um interruptor de um lado, onde uma pessoa apertava um botão e ligava o circuíto elétrico, do outro lado do circuíto tinha uma pequena barra de ferro amarrada em um fio que quando era acionada fazia um barulho, desse modo as pessoas conseguiam se comunicar por código Morse. O circuíto usava o Ground para poder economizar nos fios, utilizando a terra como condutor, mas como se sabe a distância fica limitada, por isso que para alcançar grandes distâncias, precisava-se de alguém que repetia os sinais para passar adiante, pessoas faziam isso, ficavam escutando os sinais, anotavam a mensagem e passavam para frente até chegar no destinatário.
Mas isso mudou quando perceberam que poderiam usar a própria barra de ferro para repetir o sinal, assim eles conectavam um pequeno pedaço de madeira a barra e assim que ela se movimentava e fazia os "clicks" o pedaço de madeira apertava sozinho o próximo telégrado da linha, assim se criou os **Relays** ou **Repetidores**.

## Oitavo Capítulo - Relays and Gates
Dentro da lógica booleanda existem **gates** ou **portas lógicas** que são usadas para manipular classes, dentro dos gates tem dois tipos de informações, os **inputs** que são os dados que são enviados para o operador, ou seja, se estivéssemos falando de circuítos elétricos, o dado poderia ser a presença ou a ausência da corrente elétrica no circuíto, assim, quando essa corrente chegar (ou não) no gate, é feito uma operação aritmética, temos o operador **AND** que nada mais é a interseção que falamos no capítulo anterior, junto deles temos mais outros gates básicos:
1. AND
2. OR
3. NOT
4. NOR
5. NAND

Segundo a **Lei de'Morgan**, nós podemos fazer qualquer tipo de porta lógica, somente utilizando o NAND, essa lei serve para simplificar operações muito complexas.

## Nono Capítulo - Our Ten Digits
Os números são um linguagem universal, todo o mundo usa os mesmos caracteres para representar eles. Antigamente, existiam os números gregos, eles usavam caracteres para representar uma quantidade específica, por exemplo I é 1, V é 5, X é 10, L é 50, etc... Mas esses tipos de algorismos dificultavam muito as operações matemáticas, por conta da sua complexidade e sintaxe, depois de algum tempo foi apresentado ao mundo os algorismos Hindu-arábicos, eles usam uma base **decimal** e é a mesma base que usamos hoje em dia, ou seja tem dez caracteres diferentes (0,1,2,3,4,5,6,7,8,9) e a posição dos números influencia no seu peso.
Quanto mais um número está a esquerda, mais ele vale, veja um exemplo:
478

Esse número é o Quatrocentos e Setenta e Oito, essa é a forma convencional de escreve-lo, mas também podemos usar:
4 x 100
7 x 10
8 x 1

Ou até mesmo usamor potências para escreve-lo:
4 x 10² + 7 x 10¹ + 8 x 10⁰

Basicamente esse é o sistema numérico com base 10 que usamos no dia a dia.
