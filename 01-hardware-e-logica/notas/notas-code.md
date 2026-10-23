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

## Décimo Capítulo - Alternatives 10s
Além da base decimal que usamos no nosso dia a dia, elas usam 10 caracteres diferentes (0,1,2,3,4,5,6,7,8,9) depois que esses caracteres acabam, nós passamos para a próxima casa (10), estamos mais familiarizados com esse sistema, mas também temos outras alternativas, como a base 8, com 8 caracteres diferentes (0,1,2,3,4,5,6,7), repare que na base octal não temos o número 8, assim como não temos um caracter para representar o dez na base decimal, então na base 8, o 10 na verdade não significa dez, e sim 1 e 0, e o valor dele na verdade é 8. Então para escrevermos um número em base octal que realmente vale dez é 12, e no caso caso o número '12' não é doze, e sim 1 e 2.
Assim como temos a base octal, temos também a base dois, que são representadas apenas por dois caracteres (0,1) então 10 na base dois na verdade não vale "dez" e sim 2, cada casa da base 2 é representada como uma potência de dois, ou seja o número é 1011, e ele poderia ser escrito assim:
1 x 2³ + 0 x 2² + 1 x 2¹ + 1 x 2⁰

Algum matemático percebeu que chamar os números da base dois de "dígito binário" era muito simples para a importânciaque eles tem, então ele decidiu chama-lo de bit
Assim a base dois é usada para representar qualquer número, com essa simplicidade podemos usarmos em circuítos elétricos, representadando o ligado e desligado (1 e 0), e com ela também podemos fazer operações booleanas, e isso é tudo que precisamos para montar um computador.

## Décimo primeiro Capítulo - Bit by Bit by Bit
A mágica da base dois, é a sua simplicidade, ela é a base numérica mais simples que podemos usar para representar algo, no caso também existe a base um, mas só teríamos um caracter e não conseguiríamos fazer muita coisa com isso.
Com a base dois nós conseguimos representar diferentes coisas dependendo do contexto, por exemplo:
Uma pessoa pode responder uma pesquisa de um cinema, que serve para responder se ela gostou ou não do filme, e as respostas são 0 para não gostou e 1 para gostou. Aí está, temos uma forma de interpretar esses dois caracteres.
Podemos ir mais adiante ainda, vamos supor que estamos entre 2 amigos (Pedro e João), agora temos uma combinação:
- 00 Ninguém gostou do filme
- 01 Apenas o Pedro gostou do filme
- 10 Apenas o João gostou do filme
- 11 Ambos gostaram do filme

Mas podemos ir mais adiante, códigos de barras, por exemplo, usam o mesmo raciocínio, mas ao invés de termos os 1's e 0's escritos, temos linhas e espaços, onde cada linha representa 1 e cada espaço representa 0, quando o leitor passa no código de barras ele interpreta aquela sequência e retorna o código de barras.
Resumindo, conseguimos representar qualquer tipo de coisa com a base 2, tudo depende do contexto.

## Décimo segundo Capítulo - Bytes and Hexadecimal
Historicamente, os dados se moviam dentro do computador por quantidade variáveis, poderiam ser 6, 7, ou até mesmo 9 bits, mas essa pequena quantidade de bits se movendo dentro do computador tinha um problema, eles não eram uma potência de dois, por mais que a tabela de caracteres da época cabia dentro de um conjunto com 7 bits, a escolha for faze-la com 8, por vário motivos, economia de hardware, padronização, etc... E ainda 8 bits conseguem representar de 0 a 255 caracteres, isso abrange muito mais do que somente letras,mas também outros tipos de informações.
Esse conjunto de 8 bits se chamam **bytes**, e eles foram muito importantes para a Arquitetura da computação.
Metade desse conjunto, ou seja, 4 bits são chamados de **nibble**
E um conjunto com 2 bytes, ou seja, 16 bits são chamados de **Word**
Outra base muito importante para a computação é a **Hexadecimal**, nela temos ao todo 16 caracteres para representar as quantidades (0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F), se convertemos os caracteres finais da base hexadecimal para a base decimal seria assim: A = 10, B = 11, C = 12, D = 13...  e assim por diante. No HTML temos como mudar a cor de alguma coisa usando o RGB (Red, Green, Blue) porque combinando essas cores, nós conseguimos fazer praticamente qualquer cor que conseguimos enxergar a olho nu.
Funciona dessa forma, nós temos uma sequência de 6 números onde os dois primeiros dígitos ditam a quantidade de vermelho, os dois segundos de Verde e os últimos de Azul, a quantidade mais baixa é 0 e a mais alta é F, dessa forma nós conseguimos 256 tons de cada cor, aqui são alguns exemplos:
- #FFFFFF = Branco
- #000000 = Preto
- #FF0000 = Vermelho
- #00FF00 = Verde
- #0000## = Azul

## Décimo terceiro Capítulo - From ASCII to Unicode
Grande parte das informações que você no seu computador hoje em dia estão em formato de texto, isso porque o computador usa os bits e interpretam ele como letras. Para que isso seja possível, foram criados "protocolos", o primeiro criado tinha 32 variações, isso só conseguia abranger alguns caracteres básicos, sem diferença de letra maiúscula e letra minúscula, isso é um problema, porque existem muitas outras variações de caracteres, principalmente em linguas estrangeiras, depois dela vieram mais alguns outros protocolos, mas o mais importante deles foi o *American Standard Code for Information Interchange* que usava 7 bits e contava com 128 variações de caracteres. Mas mesmo assim, esse tipo de protocolo ainda só cobria a língua inglesa, e só tinha caracteres específicos da América, como o símbolo de dólar, por exemplo.
Após a criação do ASCII, foi criado um protocolo que usava 8 bits, e dobrava as variações comparado a tabela ASCII, esse é o UTF, com 256 variações, dessa vez ele conseguia abranger bem mais línguas, e os primeiros caracteres dele foram herdados da tabela ASCII, ele é usado em grande parte da internet, existem outras tabelas com ainda mais variações, mas começam se tornar muito mais pesadas, para escrever arquivos, então o padrão da internet hoje em dia é o **UTF-8**.

## Décimo quarto Capítulo - Adding with Logic Gates
A adição na base dois é a operação matemática mais básica, e ela funciona exatamente da mesma forma que a base decimal:

0 + 0 = 0
0 + 1 = 1
1 + 0 = 1
1 + 1 = 10

Na última conta o resultado deu dois dígitos, isso porque o número da esquerda é a "sobra" da soma, ele é conhecido como **carry**, nós conseguimos montar essas adições usando portas lógicas. Usando gates como AND, OR, NAND e XOR, podemos montar um bit-adder, que pode ser usado para montar um Half-adder e depois um Full-Adder, e toda essa operação nasce de uma porta lógica.

## Décimo quinto Capítulo - Is This for Real?
Os computadores no começo de sua história, usavam relés para fazer cálculos, mas isso era um problema, por causa de custo, tamanho, manutenção, etc... Eram computadores gigantescos comparados ao que temos hoje.
O termo "Computador", antigamente, era um cargo de pessoas que trabalhavam fazendo cálculos complexos.
Depois dos computadores de relés, eles evoluíram para Válvulas, que eram muito mais rápidas que relés mecânicos, aqui também foi quando os computadores começaram a usar números binários para fazer cálculos. Mas mesmo assim, as válvulas davam muito problema de manutenção e esquentavam demais, e logo eles evoluíram para transistores (feitos de Sílicio ou Germânio), que são muito menores e são muito mais difíceis de queimar. Foi daí que surgiu o nome "Vale do sílicio"" na California.

## Décimo sexto Capítulo - But What About Substraction?
Os computadores não sabem fazer literalmente uma subtração, isso porque a arquitetura dos computadores foram feitas para usar apenas 0 e 1, e isso inclui símbolos também. O que os computadores fazem na verdade é somar números negativos, e números negativos não são representados simplesmente por um bit no final do byte, por exemplo, 10000001 é -1 e 10000001 é +1, na verdade eles fizeram outra coisa para representar números negativos.
Os computadores usam números positivos para representar números negativos, isso funciona assim, ao invés de termos uma sequência de 0 a 999 de números positivos, nós usamos os números a partir do 500 para representar números positivos.
Isso é um exemplo normal de sequência numérica:
-500, -499,... -2, -1, 0, 1, 2 ...499, 500
Aqui temos infinitos números positivos e infinitos números negativos, e usamos o símbolo de "-" para representar números abaixo de 0. Para resolver a falta do símbolo negativo, pegamos uma sequência de números positivos, dentro de um contexto e dividimos eles para representar números positivos e negativos:
500, 501,... 998, 999, 0 , 1, 2 ... 498 499

Aqui na verdade o 500 está representando o -500, o 501 é o -499, e assim por diante até chegarmos no 999, que é o último número da nossa sequência que representa o valor -1.
Dentro de um byte, nós usamos o último bit do lado esquerdo para representar um número negativo, se for 1, ele é um número negativo, assim nós conseguimos representar os números -126 até 125 usando base 2, então para fazer uma subtração na verdade é a soma de dois números positivos, e o carry (resto) é descartado.
Não temos como saber se um número binário é negativo só de olhar para ele, precisamos do contexto que ele está inserido.
