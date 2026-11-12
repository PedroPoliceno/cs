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

## Décimo sétimo Capítulo - Feedback and Flip-Flops
Nós vimos que conseguimos fazer contas matemáticas usando circuítos elétricos e gates, mas também podemos armazenar bits, e para isso existe o flip-flop, que é usado para armazenar um estado. Isso é importante porque se quisermos, por exemplo, contar até 10, precisamos saber qual foi o último número que falamos, ele funciona basicamente como um looping, que fica rodando o mesmo sinal, e só muda quando mandamos outro sinal. Vimos também o **clock** que serve para ordernar todos os cálculos que o circuíto faz, ele funciona com um sinal oscilando entre ligado e desligado, na vida real ele é um pequeno pedaço de Quartzo dentro do processador, e ele é medido de Heartz (Hz), isso é usado para medir as frequências por segundo que um processador consegue trabalhar.

## Décimo oitavo Capítulo - Let's Build a Clock!
Aqui basicamente aprendemos como montar um relógio, começamos definindo um relógio binário, que mostra somente números da base dois, mas para isso usamos O BCD(*Binary-coded-decimal*) que funciona mostrando números decimais com 4 dígitos binários, ou seja, vamos de 0000 a 1001 (ou de 0 a 9) e cada caracter se torna um número separado, por exemplo, se quisessémos escrever o seguinte horário:
12:30:24

0001 0010 : 0011 0000 : 0010 0100

Assim seria o "horário" em binário.
Esse tipo de utilização de números binários não é muito usado na arquitetura de computadores, porque eles dificultam muito as operações aritméticas, então usamos somente para horários.
Fora o modelo binário de horas, podemos também transforma-lo em legível para humanos, usando diversos gates e flip-flops.

## Décimo nono Capítulo - An Assemblage of Memory
Na computação precisamos armazenar dados permanentemente, assim como acordamos todos os dias e lembramos o que fizemos no dia anterior, e lembramos quem somos e o que precisamos fazer.
Já vimos anteriormente que um *flip-flop* é usado para armazenar um bit, que funciona basicamente como um loop, se combinarmos vários flips-flops, podemos conseguir armazenar um byte.
Quando misturamos vários flip-flops e usamos bits para "mapear" onde fica cada informação, conseguimos construir uma **RAM**(Random Access Memory).
Basicamente, temos 3 tipos de dados que são usados em uma RAM, o primeiro é o *address*, que serve como mapeamento de onde uma informação está armazenada, *Data In* são dados que passam pela RAM, *Data Out* são os dados que estavam na RAM, e o *Write Signal* que dita o que vai acontecer com os bits, se estiver ativo os dados são escritos na RAM, e se tiver desativado é somente leitura.

## Vigésimo Capítulo - Automating Arithmetic
Aqui aprendemos como automatizar operações aritméticas com portas lógicas, primeiro de tudo, precisamos organizar as informações por blocos na memória, temos duas opções principais:
- Big-Endian: Armazena primeiro os dados maiores, as casas que valem mais.
- Little-Endian: Armazena primeiro os dados que valem menos, como casas depois da vírgulo nos números decimais.

Escolhemos o *Little-Endian* por facilitar as operações, como o caso dos Carrys são calculados mais facilmente.
Para conseguirmos declarar qual operação devemos fazer (soma ou subtração) podemos usar sequência de bits para declarar isso, por exemplo 0100 para soma e 1000 para subtração (somente um exemplo).
Dessa forma conseguimos executar as operações quando queremos e salvar os resultados na RAM.
Aqui temos a separação de **hardware** e **software**:
- **hardware**: É a parte física ou simulada que é difícil de alterar (circuítos elétricos, portas lógicas, flips-flops...)
- **software**: É a parte mais fácil, são os códigos e números armazenadas na memória, é a parte fácil de alterar, podemos apaga-los e reescreve-los.

## Vigésimo primeiro Capítulo - The Arithmetic Logic Unit
A *ALU*(Arithmetic Logic Unit) serve para executar operações aritméticas com base com sinais que o CPU envia para ela, usa os números fornecidos e executa a operação e devolve o resultado.

## Vigésimo segundo Capítulo - Registers and Busses
Nesse capítulo vemos mais alguns comandos que o CPU é capaz de interpretar para manipular dados, e tivemos uma pequena menção sobre o Assembly, e vimos como ele usa os registradores para manipular esses dados.

## Vigésimo terceiro Capítulo - CPU Control Signals
Aqui vemos como a CPU usa sinais para controlar os seus dados, e como ela interpreta comandos alocados na memória para poder manipular esses dados. Vimos como o *PC*(Program Counter) funciona, e como ele ajuda a CPU a buscar informações ou comandos alocados na memória.

## Vigésimo quarto Capítulo - Loops, Jumps and Calls
Os algoritmos de computadores usam loops para poderem operar, por exemplo, se tivéssemos uma memória com 10 espaços vazios e a CPU só usasse os dados e comandos desses 10 espaços, uma hora o programa terminaria e não faria mais nada, para isso foram introduzidos os comandos *JMP* que são usados para pular para um espaço de memória. Então poderíamos usar essa mesma memória de 10 espaços e colocar um JMP no final para que quando o algoritmo terminasse poderia voltar ao ínicio e começar novamente ou introduzir novos dados.
Além do comando JMP, temos os comandos CALL e RET que são usados como funções, nesse caso, funciona como as linguagens normais, onde escrevemos um bloco de código que pode ser reutilizado ao longo do nosso algoritmo, e para sair marcar o fim dessas "funções" são usados o RET.

## Vigésimo quinto Capítulo - Peripherals
A CPU é sem dúvida o componente mais importante do computador, mas para conseguirmos aproveitar ao máximo o seu desempenho, também precisamos de outros componentes, assim como a RAM, para isso existem os periféricos.
A RAM é uma memória volátil, ou seja, depende de energia para funcionar, assim que o computador é desligado, toda a memória some, e conseguimos resolver isso com um *Mass Storage Device*, que funciona salvando dados permanentemente(a menos que eles sejam apagados ou substituídos) sem depender de energia.
Outro periférico que nos ajuda no dia a dia são as telas e monitores, que funcionam com pixel (mini quadradinhos na tela), um monitor pode ter uma resolução de 1920x1080 pixels, ou seja, a sua tela tem 1920 pixels horizontalmente e 1080 verticalmente, e conseguimos manipular as cores desses pixeis para desenhar qualquer coisa na nossa tela usando o sistema RGB.
Em paralelo as telas e monitores, o que nos ajuda a escrever e selecionar coisas na tela são os mouses e teclado, quando nós apertamos uma tecla no teclado ele envia um código que o CPU interpreta e desenha o caracter na tela, acontece a mesma coisa com o mouse que passa códigos quando é usado e é trabalho do Sistema Operacional desenhar o cursor e fazer cálculos de coordenada para que nós possamos usa-lo. Esse tipo de periférico pode ser chamados de *I/O*(Input / Output Devices).

## Vigésimo sexto Capítulo - The Operating System
Os Sistemas Operacionais servem para ajudar o usuário a conseguir manipular os dados no seu hardware, vimos que existe o *file system* que se trata de um sistema que cria arquivos para guardar informações, os computadores de hoje em dia tem uma ROM que contém um pequeno script para "puxar" todo o resto do sistema operacional chamado bootstrap loader, ele serve para iniciar todo o sistema, esse processo é atualmente chamado de 'booting'.
O computador é organizado por hierarquia, o nível mais baixo que conversa diretamente com o hardware se chama *BIOS*(Basic Input/Output System).
Temos alguns exemplos muito importantes para a história dos Sistemas Operacionais, o MS-DOS, um dos primeiros OS da Microsoft, Macintosh, O sistema operacional mais importante para Apple que disponibilizava uma interface gráfica, o UNIX que nasceu para ser um OS que funcionava em qualquer computador.

## Vigésimo sétimo Capítulo - Coding
Conseguimos criar algoritmos com a liguagem *Assembly*, como vimos nos capítulos anteriores, podemos utilizar declarações para manipular dados e criar uma sequência de passos para atingir um objetivo. Mas a Linguagem Assembly é muito díficil de usar e pouco útil hoje em dia (salvo as execeções), ela funciona com um montador, que interpreta a o script que escrevemos e "traduz" ela para linguagem de máquina.
Mas hoje em dia temos muitas outras linguagens de programação usada para a Engenharia de Software, elas foram criadas com o objetivo de facilitar o desenvolvimento e fazer com que um algoritmo possa ser usado em vários computadores, alguns exemplos de linguagens que foram desenvolvidas para isso são FORTRAN, COBOL e ALGOL, mas elas não usadas mais hoje em dia. Essas são linguagens de *alto nível*, o Assembly é considerado de *baixo nível* porque conversa diretamente com o hardware.
Para cada linguagem de programação nós precisamos ter uma ferramenta de "intermediação" que seja capaz de traduzir os scripts para linguagem de máquina, essas ferramentas podem ser o compilador, ou interpretador, elas funcionam de formas diferentes, o interpretador é um pouco mais fácil para desenvolver, mas também pode ser um pouco mais lento que o compilador.
Alguns exemplos de linguagens de programação que são muito usadas hoje em dia são Python, JavaScript, C#, etc... Existem diversos tipos diferentes de linguagens, procedurais, orienteada a objetos, funcionais, e aí por diante...

## Vigésimo oitavo Capítulo - The World Brain
Nesse último capítulo vemos um pouco de como a Internet funciona, ela é um ambiente descentralizado, que está em vários computadores ao redor do mundo.
Foi falado como que a transferência de dados por pacotes funciona *TCP/IP*, e como os nossos computadores tem endereços para saber para onde devem ir os dados que requisitamos.
Hoje a maior base de conhecimento do mundo é a Internet, onde grande parte de todas as informações estão localizadas.

# Releitura do livro (Cap: 8, 12, 14, 16, 17, 18, 19, 20, 21, 22, 23 e 24)
## Capítulo 8 - Relays and Gate
Resumindo, os computadores são uma junção de Álgebra Booleana e Eletricidade, os componentes que fazem essa junção são as "portas" ou "gates". O livro nos apresenta um exemplo de uma pessoa escolhendo um gato, e essas são as exigências dela:
"Eu quero um gato macho, castrado, preto ou bronzeado, ou uma gata fêmea, qualquer cor exceto branco, ou eu quero qualquer gato contanto que seja preto."

A expressão booleana para esses critérios fica assim:
(M × N × (W + T)) + (F × N × (1 − W)) + B

Onde x representa o AND e o + representa o OR.
Usando a "communicative law" e a "distributive law" a expressão fica simplificada assim:
(N × ((M × (W + T)) + (F × (1 − W)))) + B

Para essa expressão poderíamos montar um painel para escolher o nosso gatinho, onde cada variável pode virar um interruptor ligado a um circuíto elétrico, e conforme você acionasse ou desligasse eles, iria ligar uma lâmpada caso os critérios do gatinho fossem atendidos.
Falando em terminologia de computadores, os interruptores seriam os "input devices" e a lâmpada seria o "output device".

Nesse capítulos vemos como os Relés são ligados em cascatas para construirmos portas lógicas, cada relé é conectado em outro e assim conseguimos combinar os sinais elétricos.
- AND é usado para uma opereção booleana, onde todos os inputs precisam ser verdadeiros para resultar em um output verdadeiro, se qualquer um dos inputs for falso, o output será falso também. O AND básico tem somente duas entradas para inputs, mas se combinarmos mais de um AND, conseguimos fazer um 3-input-AND, ou até mais do que apenas três.
- OR é outro gate usado para operações booleanda, mas ele age de forma um pouco diferente, se apenas um dos inputs for verdadeiro, o output também vai ser.
- NOT é o único dessa lista que contém somente um input, e a razão disso é porque ele inverte a entrada, ou seja, se o input for verdadeiro, ele irá retornar o falso, e vice-versa.
- NOR ou (NOT OR) é basicamente o inverso dos outputs do NOR comum, ou seja toda vez que um OR resultaria em falso o NOR resulta em verdadeiro, a mesma coisa ao contrário.
- NAND ou (NOT AND) segue a mesma lógica que que o NOR, mas age com o inverso do AND, toda vez que o AND resultaria em verdadeiro, ele resulta em falso.
- Buffer é conhecido por não fazer muita coisa de diferente, ele apenas replica o input no output, ele é usado para duplicar um sinal fraco, ou usado para conseguir "atrasar" um pouco o sinal, isso funciona porque os relés demoram uma pequena fração de segundo para operar.

Nós podemos usar o NAND e o NOR para fazer qualquer outro gate. Por exemplo, se ligarmos o mesmo input nas duas entradas do NAND conseguirmos construir um NOT, se pegarmos esse NOT e conectarmos no final do output do NAND construimos um AND, se invertemos os dois inputs do AND, ele tem o mesmo resultado que um NOR, o mesmo funciona se invertemos os inputs do OR, temos o mesmo resultado que o NAND. Isso que acabei de explicar é a representação do **Lei de Morgan**:

- (NOT A) AND (NOT B) = NOT(A OR B)
- (NOT A) OR (NOT B) = NOT(A AND B)

A Lei de Morgan é uma ferramente importante para simplificar operações booleanas, e também circuítos elétricos, muito usados por engenheiros elétricos.

## Capítulo 12 - Bytes and Hexadecimal
Para conveniência em mover e manipular dados, os sistemas de computadores agrupam bits, esses "grupos" de bits são chamadas **word**. Os tamanhos das words dependem da capacidade do processador, a diferença de word para bytes é que os bytes são um número fixo de bits (8) enquanto as words dependem da arquitetura do processador (16 bits, 32 bits, 64 bits), se um processador consegue mover e tratar 64 bits de uma vez a "word" desse processador são 64 bits.
Os bits são convertidos em outra base, como o exemplo a seguir, para facilitar a leitura e interpretação de humanos, porque números binários são muito longos e confusos, e converte-los para uma base maior, ajuda na hora de desenvolvimento.
Antigamente, os computadores eram majoritariamente feitos com múltiplos de 6 bits (12, 24, etc...), isso acontece porque era possível representar esses números com *base octal*(0, 1, 2, 3, 4, 5, 6, 7) que correspondem a um valor de 3 bits:
000 0
001 1
010 2
011 3
100 4
101 5
110 6
111 7

Mas a indústria da computação tomou um rumo um pouco diferente, o problema dos processadores com múltiplos de 6 bits é que não são potências de dois. Aí entrou a palavra "byte", no começo o byte era somente o número em um determinado caminho de dados, mas mais para frente por causa do desenvolvimento de computadores empresariais chamados *System/360*, a byte foi definido como um conjunto de 8 bits. A escolha de 8 bits aconteceram por uma série de comodidades, uma delas é porque os caracteres que conseguimos representar com 8 bits são 256, e é a quantidade necessária para representar os caracteres da tabela ASCII por exemplo, e se caso houvesse alguma outra língua que não fosse possível representar com apenas 256 caracteres, como o caso do japones, chines, etc... 2 bytes funcionam muito bem.
Como a base octal não se encaixa para conseguirmos representar uma sequência de 8 bits (isso acontece porque 8 não é divisível por 3), precisamos de outra base para conseguirmos fazer isso, aí entra a **base hexadecimal (16)**.

A base hexadecimal é representada por 16 caracteres (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F). Eles conseguem representar um *nibble* (4 bits, meio byte, etc...):
| Binary | Hexadecimal | Decimal |
| :--- | :---: | :---: |
| 0000 | 0 | 0 |
| 0001 | 1 | 1 |
| 0010 | 2 | 2 |
| 0011 | 3 | 3 |
| 0100 | 4 | 4 |
| 0101 | 5 | 5 |
| 0110 | 6 | 6 |
| 0111 | 7 | 7 |
| 1000 | 8 | 8 |
| 1001 | 9 | 9 |
| 1010 | A | 10 |
| 1011 | B | 11 |
| 1100 | C | 12 |
| 1101 | D | 13 |
| 1110 | E | 14 |
| 1111 | F | 15 |

Ou seja, conseguimos representar 1 bytes com 2 caracter hexadecimais:
| Binary | Hexadecimal | Decimal |
| :--- | :---: | :---: |
| 00000000 | 00h | 0 |
| 00010000 | 10h | 16 |
| 00011000 | 18h | 24 |
| 00100000 | 20h | 32 |
| 01000000 | 40h | 64 |
| 01100100 | 64h | 100 |
| 10000000 | 80h | 128 |
| 11000000 | C0h | 192 |
| 11001000 | C8h | 200 |
| 11100000 | E0h | 224 |
| 11110000 | F0h | 240 |
| 11111111 | FFh | 255 |

A base 16 funciona como todas as outras, onde cada número representa uma potencia de 16, e o caracter mais a esquerda é o que vale mais.

## Capítulo 14 - Adding with Logic Gates
Nesse capítulo vamos aprender como construir um sistema de adição, porque adição é a operação aritmética mais básica da computação, e com ela conseguimos construir todas as outras.
Mas para o caso de construir um computador do zero, nós não vamos construir uma calculadora normal, da base 10, ao contrário disso, vamos montar um sisterma quer faz a adição *números binários*.
A adição para números binários funciona exatamente igual a de números decimais, você começa do número menos significativo para o mais, e sempre que aparece uma "sobra" ou um **carry**, nós passamos para a próxima casa.

Para somar dois bits com Portas Lógicas nós precisamos primeiro analisar o resultado que queremos, um soma de dois bits, pode resultar em um número maior que um bit:

| A | B | Sum | Carry |
| :--- | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

Ou seja, o carry é a "sobra" da adição de dois bits. Mas repara bem em uma coisa, se analizarmos somente a coluna do Carry e as colunas do A e B, o resultado da tabela é idêntico a se nós usassemos o AND gate, então logo já conseguimos resolver o problema do Carry, agora precisamos do Sum (ou o resultado da soma).
Dentro da computação, nós temos um gate chamado **XOR**, ou Exclusive OR, e ele é montado exatemente assim:
(A NAND B) AND (A OR B)
O resultado dessa operação é o que chamamos de XOR, e é exatamente o que precisamos para montar o resultado da nossa soma, porque a truth table dele é exatamente igual a da coluna Sum. Ou seja:
A AND B = carry
A XOR B = sum

Essa "simplificação" se chama **encapsulação**, é quando nós abstraímos os detalhes de como exatamente o sistema ou circuíto funciona para deixarmos a visualização e entendimento mais "simples". Quando nós representamos o HalfAdder (que é o que acabamos de montar), com apenas um quadrado com dois inputs (A e B) e dois outputs (Carry Out e Sum Out), sem mostrarmos as portas lógicas, isso se chama *black box* ou caixa preta, é uma forma de abstração.
Agora já temos uma forma de fazer uma conta simples de dois bits, mas com isso não conseguimos fazer muita coisa, por exemplo se quisessemos fazer essa conta:
 1111
+1111
11110

Veja que conseguimos usar o HalfAddder para a primeira coluna, mas a partir da segunda, precisamos colocar o carry que sobrou da primeira na equação, para isso vamos precisar fazer um Adder com 3 bits:

Considere os operandos A,B e C (de carry).
HalfAdder(a=a, b=b, carry=carry1, sum=sum1)
HalfAdder(a=sum1, b=c, carry=carry2, sum=sum)
Or(a=carry1, b=carry2, out=carry)

Isso se chama **FullAdder**, e ele serve para somar 3 bits, agora sim conseguimos executar a operação que citei acima.
Com o FullAdder em mão tudo o que precisamos fazer é conectar o carry out de um FullAdder no próximo e assim conseguimos fazer um efeito cascata para criarmos um 8-bit adder, para somarmos 1 byte, e o resultado dele vai ser um sum e um carry.
FullAdder(a=a[1], b=b[1], c=c0, sum=out[1], carry=c1);
	FullAdder(a=a[2], b=b[2], c=carryin, sum=out[2], carry=c2);
	FullAdder(a=a[3], b=b[3], c=c2, sum=out[3], carry=c3);
	FullAdder(a=a[4], b=b[4], c=c3, sum=out[4], carry=c4);
	FullAdder(a=a[5], b=b[5], c=c4, sum=out[5], carry=c5);
	FullAdder(a=a[6], b=b[6], c=c5, sum=out[6], carry=c6);
	FullAdder(a=a[7], b=b[7], c=c6, sum=out[7], carry=carryout);

Uma vez que construímos o 8-bit adder, podemos combina-los para criar um 16-bit adder, usando um 8Adder para calcular os bits menos significantes, e outro para os bits mais significantes, e depois ligamos o carry out de um ligado no carry out de outro.

## Capítulo 16 - But What About Substraction
Agora que temos o poder do Adder nas mãos, como que podemos fazer a operação de **Subtração**, ela ainda é uma operação básica que complementa a adição, mas tem um mecanismo um pouco diferente.
Na subtração, ao invés de sobrar, ou o "carry", temos a sobra, ou o "borrow", e para não precisarmos manipular um monte de portas lógicas e circuítos elétricos para chegarmos nesse mecânismo, podemos simplifica-lo para funcionar no que já temos.
Vamos supor que queremos subtrair dois números decimais, como vimos no ensino fundamental, a subtração é a mesma coisa que a adição com números negativos:
-176 + 253 = ?

Nessa conta, nós ainda vamos ter as chamadas "sobras" então como podemos contornar isso? Simples, podemos adicionar um 1000 no começo e subtrair 1000 no final da conta:
1000 - 176 + 253 - 1000

Mas repare que ainda vamos ter que emprestar 1  na primeira conta (1000-176), como sabemos o 1000 pode ser representado com 999 + 1, então podemos adicionar 999 e depois somar 1 no final da conta, quando usamos o 999 nunca vamos precisar emprestar da próxima casa decimal:
999 - 176 + 253 - 1000
823 + 253 - 1000
1076 + 1 - 1000
1077 - 1000
**77**

Repare que não precisamos "emprestar um" em nenhum momento da conta. Isso se chama **complemento 9**, e serve para simplificarmos as contas.
O complemento 9 de 823 é 176, e vice e versa. E não importa a conta, *o complemento nunca precisa emprestar*.
Mas e se tentassemos subtrair um número maior do que outro, para fazermos essa conta usando o complemento 9, é só lembrar que o número é maior, logo o resultado vai ser negativo:
999 - 253 + 176 - 1000
746 + 175 - 999
922 - 999
**-77**
Isso não é tão direto quanto a operação anterior, mas ainda funciona bem. Podemos usar essa mesma estratégia para números binários:
- 10110000 + 11111101

Podemos adicionar 11111111 no primeiro, depois adicionar 0000001, e no final da equação subtrair 100000000:
11111111 - 10110000 + 11111101 + 00000001 - 100000000
01001111 + 11111101 + 0000001 - 100000000

Quando utilizamos a técnica de complemento em base decimais usando o 999... o nome é complemento 9, mas quando usamos na base binária, adicionando 111... na conta, o nome é complemento 1.
Repare que o complemento 1 de 10110000 é 01001111 e o complemnto 1 de 01001111 é 10110000, repare que os digítos são só invertidos, essa é a razão do complemento 1 ser comumente referido como *inverse*.
Continuando...
101001100 + 00000001 - 100000000
101001101 - 100000000
**01001101**

Essa foi a mesma conta que fizemos mais cedo com a base decimal (253-176=77), mas voltamos ao problema que citamos a cima, quando tentamos subtrair um número maior e o resultado tende a ser negativo.
11111111 – 11111101 + 10110000 – 11111111
10110010 – 11111111
11111111 – 10110010 = 01001101
255 – 178 = 77

E aqui temos um problema, porque o resultado da conta foi 77, quando na verdade deveria ter sido -77, mas não vamos tratar esse problema agora. Por enquanto vamos nos concentrar em transformar o nosso 8-bit adder em um sistema de subtração também, que calcula números positivos.
Para isso vamos adicionar mais um bit de input usado para indicar se vamos subtrair ou fazer adição dos números indicados, e agora vamos tratar o que antes era o Carry Out, como **overflow**, o overflow vai aparecer quando o resultado for um número de 9 bits, isso pode acontecer tanto na adição quanto na subtração.
A principal implementação da nossa máquina de subtrair e adicionar, é o calculador de complemento 1, para isso podemos usar o gate XOR, com um dos inputs como o sinal de subtração ou adição e outro como o bit que queremos inverter (ou não).
Assim, supunhamos que temos dois números com 8 bits, um deles nós conectamos no inversor para calcular o complemento 1 e o mesmo sinal que usamos para definir se vamos subtrair ou adicionar, usamos como Carry In do Adder, porque precisamos adicionar 1 no número antes de terminamos a conta e somarmos 100000000.

No final do cálculo do 8-bit adder, pegamos o Carry Out e o sinal de Subtraction e colocamos os dois em um gate XOR, e o output dele vai servir como Overflow. Isso significa que se o "Substraction" estiver desligado, e o Overflow for 1 quer dizer que o resultado foi maior que 255, se o Substraction estiver ligado e o overflow for 1 quer dizer que o resultado é menor que o número "A"(o número que não foi invertido).
Nós ainda não chegamos no resultado esperado, que é conseguir subtrair de forma que o resultado seja representado certo, para fazermos isso, precisamos de um jeito de representar os números negativos nessa equação, como vimos antes, temos o complemento 1 onde adicionamos 11111111 no começo da conta, depois adicionamos 00000001, e no final subtraímos 100000000, mas nele temos alguns problemas, como por exemplo, suponhamos que temos o número 0000 (que representa 0) e queremos fazer um conta de subtração, então existira um "zero negativo" (1111).
Nesse caso, precisamos de uma solução que resolva esse problema, para isso eu apresento o complemento 2. Vou explicar primeiro como funciona o complemento 10 para ficar mais fácil o entendimento:
Suponhamos que temos uma sequência de 0 a 999 números, nesse caso poderíamos representar (obviamente), do 0 ao 999, mas e se não precisassemos representar tudo isso, e se quisessemos representar só metade desses números positivos e deixamos a outra metade para representar números negativos. Em algorismos normais os números negativos funcionam assim:
-999, -998,... -2, -1, 0, 1, 2,... 998, 999
Repare que o 0 é o centro e temos infinitos números negativos para a esquerda e infinitos números positivos para a direita, mas no nosso caso não temos infinitos números, temos apenas 1000(0 a 999), nesse caso poderíamos usar até o 499 para representar números positivos, e a partir daí usarmos o restante para números negativos:
500, 501,... 998, 999, 0, 1, 2,... 498, 499
-500, -499,... -2 -1, 0, 1, 2,... 498, 499

A diferença entre o complemento 1 e o complemento 2 é que no primeiro nós só invertemos os bits, no segundo nós somamos 1 bit na conta.
Agora fazendo um paralelo para os números binários, podemos pegar um número de 8 bit (byte) e fazermos a mesma coisa, mas no caso podemos só inverter os bits, como fazemos no complemento 1: 10110011 vira 01001100, e vice versa, e adicionamos 00000001 no final:
10000000 = -128
10000001 = -127
10000010 = -126
...
11111101 = -3
11111110 = -2
11111111 = -1
00000000 = 0
00000001 = 1
00000010 = 2
...
01111100 = 124
01111101 = 125
01111110 = 126
01111111 = 127

Assim podemos usar somente a soma e ignorar o carry para obtermos o resultado correto da subtração:
  10000001
+ 01111100
  11111101

Aqui subtraímos o número -127 por 124 e o resultado foi -3.
Mas o problema aparece quando tentamos somar dois números negativos, ou quando o resultado da soma (ou subtração) é maior que 127:
  01111101
+ 01111101
  11111010

Aqui o resultado de 125 - 125 foi -6, isso acontece quando tentamos somar -125:
  10000011
+ 10000011
 100000110

Se ignorarmos o bit mais a esquerda (já que essa é uma operação de 8 bits), o resultado é 6, e obviamente está errado. Em geral o complemento 2 apresenta erros quando 2 números iguais são somados.
Nós podemos adicionar alguns gates para detectar o overflow da operação, em mente que o bit que mais vale em um número representa se o número é positivo (0) ou negativo(1), tanto dos números que vão ser usados no cálculo, tanto no resultado do cálculo.
Nós pegamos o bit mais valioso do número A e do número B, e invertemos o bit mais valioso do sum desses números e conectamos eles em um gate AND e em um gate NOR. O papel do AND é detectar o overflow para números negativos, se o bit mais valioso do A e do B forem 1, o que indica um número negativo e o bit mais significativo do resultado for 0, o que indica um número positivo, algo está errado.
O NOR detecta o overflow de números positivos, se ambos os bits mais valiosos do A e B forem 0 e o resultado der um bit 1, que indica número negativo, algo também está errado.
Os números binários por si só, são *unsigned* porque são somente positivos, quando usamos o complemento a 2, esses números binários se tornam *signed*, porque podemos representar números negativos com ele também, para um sequência de 8 bits conseguimos representar dos números -127 ao 128. O conceito matemático disso são números inteiros, ou **integers**, ou seja, que podem ser negativos e positivos.
Hoje em dia, um número de 8 bits é extramamente pouco para trabalharmos, por isso usamos números com 16, 32, e até 64 bits, todos eles conseguem ser representados com *unsigned* e *signed*, e a sequência exponencialmente usando potências de 2.

## Capítulo 17 - Feedback and Flip-Flops
Todo mundo sabe que conseguimos usar a eletricidade para mover as coisas, como ventiladores, motores, ferramentas, etc... Na computação isso não é diferente.
Nós conseguimos construir um loop usando uma porta lógica que oscila o sinal, basta conectarmos um input em um gate NOT e usar o output como input novamente, assim criamos um loop que oscila entre 0 e 1, desligado e ligado, falso e verdadeiro, etc... Essas conexão pode se chamar de *oscillator*.
Conseguimos criar um diagrama de uma linha representando o output desse oscilador, seria algo como uma linha quadrada que sobe e desce de forma simétrica, onde a linha horizontal representa o tempo e a linha vertical representa o estado de 0 e 1. Olhando para essa linha vemos um espécie de tic-tac regular, e por isso que alguns chamam esse oscilador de **clock**, porque contando o números de oscilações conseguimos dizer o tempo (mais ou menos).
Como que sabemos o quão rápido um clock é? Primeira precisamos saber algumas medidas que são usadas, a primeira dela é o *cycle* que é o tempo que um clock está na posição padrão, oscila e volta para a posição padrão novamente, o tempo que esse ciclo demora para acontecer se chama *period*, suponhamos que o período do nosso clock seja 0,02 segundos. Depois disso temos a frequência, ela é calculada *1 / period*, no caso do nosso clock, seria 50 ciclos por segundo.
"Ciclos por segundo" é um termo auto-explicativo que não é usado muito hoje em dia, em homenagem ao Heinrich Rudolph Hertz, que foi a primeira pessoa que transmitiu e recebeu ondas de rádio, a palavra *hertz* é usada para medir a quantidade de ciclos de segundo, nesse caso diríamos que o nosso clock tem a capacidade de *50 hertz* ou *50 Hz*. Nesse caso nós apenas adivinhamos qual era a velocidade desse clock, mas o objetivo ao final desse capítulo é construir algo que consiga mensurar a velocidade do oscilador.
Para começar podemos montar um circuíto com um par de gates NOR, O primeiro deles usa um input, e o output dele serve para o outro gate NOR, no 2° gate NOR já temos um input vindo do primeiro, e o segundo input é o normal, depois o output do segundo NOR vai fazer a volta e virar o segundo input do primeiro NOR e esse mesmo vai ser ligado em uma lâmpada, então ficaria mais ou menos assim:
Nor(a=out, b=a, out=b);
Nor(a=b, b=c, out=out);
Para esse circuíto funcionar, precisamos sair do princípio que podemos fechar o input A ou o C, mas nunca os dois juntos.
Supondo que os dois inputs (a e c) estejam abertos, o output do primeiro NOR vai ser 1 e o output do segundo NOR vai ser 0, o que resulta em 0.
Agora se fechamos o input a, o primeiro NOR vai resultar em 0, o que significa que o segundo NOR vai ser 1, e o resultado é 1.
Agora a mágica ocorre quando os dois inputs (a e c) são aberto novamente, o circuíto continua ligado, isso acontece porque o primeiro NOR continuou recebendo carga do output do primeiro, o que resultou no output do primeiro NOR igual a 0 e do segundo igual a 1. Nós podemos abrir e fechar o primeiro input que o circuíto vai continuar ligado, só conseguimos um resultado diferente quando fechamos o input c, porque o output do segundo NOR vai ser 0, o que resulta no desligamento de todo o circuíto, e agora podemos desligar o input c, que vai continuar tudo desligado.
O mais estranho é que dependendo quando abrimos os dois inputs (ambos 0), o output do circuíto pode variar de 0 e 1, ele tem dois estados estáveis quando os inputs são ligados. Esse circuíto é chamado de **flips-flops**, eles "retém informação". Esses circuítos podem ser comparados a uma "gangorra" por que só de olhar para ela nós conseguimos deduzir qual lado foi empurrado para baixo por último, esse circuíto é uma ferramenta muito importante para que possamos adicionar um tipo de memória ao nosso computador, isso é muito importante para diversas coisas, pense como é contar sem saber o último número que falamos.
Existem diversos tipos de flip-flop, o que acabamos de ver se chama R-S (Reset-Set), os dois NOR gates podem ser desenhados mais simétricamente, imagine dois NOR's um com cada input, um desses inputs são chamados Reset e o outro Set, os outputs de cada NOR são conectados no input do outro, o NOR que está com o Reset tem o output chamado Q, e o outro é o Q/, ou Q bar, que no caso é o oposto do Q.
Tabela de Verdade (SR Latch)

Inputs: S, R | Outputs: Q, Q̅

S = 1 e R = 0 | Q = 1 e Q̅ = 0
S = 0 e R = 1 | Q = 0 e Q̅ = 1
S = 0 e R = 0 | Q = Q e Q̅ = Q̅
S = 1 e R = 1 | Disallowed (Proibido)

Essa é a truth table do Flip-Flop, note que quando ambos inputs são 0 os outputs são Q e Qbar, isso acontece porque o circuíto se lembra do estado deles antes dos dois inputs ficarem abertos.
Melhor do que apenas lembrar de um bit qualquer, é lembrar de um bit que **queremos** lembrar, para implementar isso, precisamos de mais um input, o nome dele vai ser "Hold That Bit", que basicamente é um sinal para quando queremos guardar um bit, vamos supor que temos esse input e mais outro que se chama "Data", quando o input Hold That Bit está apagado, o bit "Data" não tem nenhum efeito sobre o circuíto, agora quando ele é 1, o circuíto reflete o Data:
Inputs: Data, Hold That Bit | Output: Q

Data = 0 e Hold That Bit = 1 | Q = 0
Data = 1 e Hold That Bit = 1 | Q = 1
Data = 0 e Hold That Bit = 0 | Q = Q
Data = 1 e Hold That Bit = 0 | Q = Q

Para implementar o Hold That Bit no R-S que já fizemos anteriormente, precisamos inserir mais dois gates AND, o primeiro AND vai ter como o input o reset e o sinal do Hold That Bit, o segundo AND, também tem o Hold That Bit como input, mas tem também o Set. Quando fazemos isso, se o Hold That Bit for 0, não importa se o Set ou o Reset tiverem valores diferentes, não vamos ter efeito nenhum no circuíto, apenas quando o Hold é 1 que o R-S volta a funcionar normalmente como vimos antes, o comportamento é exatamente o mesmo. Mas nós queremos somente 2 inputs, não três.
Se paramos para pensar, não faz sentido ambos os inputs (Set e Reset) serem 0, porque isso não tem efeito nenhum sobre o circuíto, a mesma coisa acontece quando ambos são 1, então o que mais faz sentido é um ser o inverso do outro, quando o Set está ligado, o Reset desliga, e vice e versa, então podemos unir os dois inputs somente em um chamado "Data" e ligar ele em um NOT, para servir como Reset, assim os sinais sempre vão ser diferentes. A segunda mudança que vamos fazer é dar um nome diferente para o Hold That Bit, vamos começar chama-lo de Clock, o que pode soar um pouco estranho, mas vamos ver daqui a pouco como isso vai funcionar, mas por enquanto ele só significa quando o bit é salvo.
Então funciona exatamente da mesma maneira, quando o clock está ativo, o circuíto vai lembrar do valor do Data, o nome dele é "level-triggered D-type flip-flop", o D é de Data. Esse é a truth table dele:
Tabela de Verdade (D Flip-Flop / Latch com Clock)

Inputs: D, Clk | Outputs: Q, Q̅

D = 0 e Clk = 1 | Q = 0 e Q̅ = 1
D = 1 e Clk = 1 | Q = 1 e Q̅ = 0
D = X e Clk = 0 | Q = Q e Q̅ = Q̅

Esse circuíto também é conhecido como "Level-triggered D-type latch", isso porque o ele segura um bit de informação para quando quisermos usar.
Esse é uma memória de um bit, e conseguimos montar ela para salver 1 byte de uma vez, ou seja, 8 bits, ou seja vão ter 8 datas inputs , um clock e 8 Qs de output, quando o clock é um, o byte inteiro vai para os "Qs", os Q̅ são ignorados aqui.
Nós podemos usar esse circuíto com outros e montar algo mais complexo, como por exemplo, montar um "adder acumulador", nós podemos usar um 8 bit adder e conectar o output dele no 8 bit latcher, e usar o output do 8 bit latcher como input do adder, e colocamos um sinal no clock para quando queremos somar que podemos chamar de "Add". Então por padrão a primeira saída do latcher é 0, o que significa que o adder vai somar o input com nada, o que não vai mudar nada no output, então quando ele chegar no latcher, o Add estiver ativado, ele vai ser armazenado e vai voltar como input do adder novamente, somando com o próximo valor de input, e novamente o ciclo se repete.
Para algumas aplicações, o Level-triggered D-type latch serve, mas para um adder acumulador nós não queremos que o data passe direto sempre quando o Clock for um, nós queremos que o latch salve o data toda vez que o clock muda de 0 para 1, ou de 1 para 0, essa transição é chamada "edge".
Para isso temos o positive edge-triggered flip-flop latches, a diferença dele para o que vemos acima é que ele não salva os dados quando o clock é um, ele salva quando o clock migra de 0 para 1. Parece algo meio difícil de montar, mas há um macete, o positive edge-triggered flip-flop latches, é feito com dois Level-triggered D-type latch conectados de uma forma específica.
Para conectarmos os dois latchs, primeiro invertemos o sinal do Clock e conectamos no primeiro flip-flop, e depois conectamos os dois outputs do primeiro no segundo latch, junto com o sinal original do clock, repare que o primeiro latch vai funcionar como um level-triggered D-type flip-flop, os bits vão ficar armazenados sempre no primeiro latch, já que o sinal do clock chega invertido.

Tabela de Verdade (D Flip-Flop Sensível à Borda de Subida)

Inputs: D, Clk | Outputs: Q, Q̅

D = 0 e Clk = ↑ | Q = 0 e Q̅ = 1
D = 1 e Clk = ↑ | Q = 1 e Q̅ = 0
D = X e Clk = 0 | Q = Q e Q̅ = Q̅

Essa é a truth table do nosso novo latch, repare que há setas apontadas para cima, isso quer dizer quando o clock muda de 0 para 1.
Agora podemos conectar o nosso edge-triggered latch no nosso 8 bit adder para fazermos a acumulação adder, mas ainda temos um problema, o Carry Out ou "sobra" do adder é simplesmente ignorado aqui.
Agora vamos explorar outro tipo de edge type latch, primeiro precisamos conectar o oscilador que falamos no começo do capítulo no input de clock, e depois usamos o Q̅ como próprio input no Data do Latch, o truth table desse flip-flop:
Tabela de Verdade (D Flip-Flop)

Inputs: D, Clk | Outputs: Q, Q̅

D = 1 e Clk = 0 | Q = 0 e Q̅ = 1
D = 1 e Clk = ↑ | Q = 1 e Q̅ = 0
D = 0 e Clk = 1 | Q = 1 e Q̅ = 0
D = 0 e Clk = 0 | Q = 1 e Q̅ = 0
D = 0 e Clk = ↑ | Q = 0 e Q̅ = 1
D = 1 e Clk = 1 | Q = 0 e Q̅ = 1

Repare que quando o clock muda de 0 para 1, o Q e o Q̅ mudam de posição, por exemplo, o Q é 0, quando o clock muda para 1 ele muda para 1 também, mas quando o clock muda para 0 não acontece nada, somente quando o clock para um, o Q muda para 0, isso também ocorre para o Q̅ (só que ao inverso, é lógico).
Nós já sabemos que usamos a medida *Hertz* para medir frequências, mas se um clock oscila 20 vezes por segundo, esse flip-flop tem a metade dessa frequência, ou seja 10 Hz. Isso pode ser chamado de **divisor de frequência**.
Nós obviamente, conseguimos dividir um divisor e dividir outro divisor, e assim vai...
Sinal Clk: Ciclos alternando entre 0 e 1 continuamente a cada pulso.

Sinal Q1: Mantém-se em 0 nos dois primeiros instantes e depois alterna o estado a cada dois ciclos (0, 0, 1, 1, 0, 0, 1, 1).

Sinal Q2: Mantém-se em 0 por quatro ciclos e depois vai para 1 por mais quatro ciclos (0, 0, 0, 0, 1, 1, 1, 1).

Sinal Q3: Mantém-se em 0 por oito ciclos e depois vai para 1 nos oito ciclos seguintes

Se nós escrevessemos os números resultados de cada divisor de frequência, e depois colocasse eles na vertical o nosso resultado seria esse:
**Binary**

0000
0001
0010
0011
0100
0101
0110
0111
1000
1001
1010
1011
1100
1101
1110
1111

Veja o padrão? É uma sequência de 0 a 15 em binário. A cada transação positiva do clock (de 0 para 1), o output fala para *incrementar*, nós podemos pegar esse circuíto e colocar dentro de uma caixa, podemos chamar ele de 8-bit ripple counter. Nós conseguimos usar os 8 bits que saem desse circuíto para contar a frequência do clock. Nós poderiamos "zerar" os outputs, e colocar para contar quando o circuíto chegasse em 255 em binário em zerasse novamente, nós checaríamos em quanto tempo demorou, vamos supor que fosse 10 segundos, nós pegamos 256 e dividiriamos por 10, o que resultaria em 25,6 hz.
O único problema com o ripple counter, é que nem sempre ele pode começar com o 0, para isso, nós adicionamos um sinal "Clear" que serve para zerar totalmente o contador. Nós conectamos ele em um NOR depois do AND que seria o "Reset". E se colocamos um sinal de Reset, também precisamos considerar um sinal de "Preset", enquanto o Clear muda o Q para 0, o Preset muda para 1.
**Entradas (Inputs):** Pre, Clr, D, Clk

**Saídas (Outputs):** Q, Q̅

Pre = 1, Clr = 0, D = X, Clk = X → Q = 1, Q̅ = 0

Pre = 0, Clr = 1, D = X, Clk = X → Q = 0, Q̅ = 1

Pre = 0, Clr = 0, D = 0, Clk = ↑ → Q = 0, Q̅ = 1

Pre = 0, Clr = 0, D = 1, Clk = ↑ → Q = 1, Q̅ = 0

Pre = 0, Clr = 0, D = X, Clk = 0 → Q = Q, Q̅ = Q̅

Esses são os primeiros passos para construir uma **memória** do computador.

## Capítulo 19 - Let's Build a Clock
Nesse capítulo vamos construit um relógio, mas não um relógio de parede que mostra as horas por um ponteiro, e sim um relógio que mostra os números em binário!
Vamos pegar um exemplo: 12:30:47
Se quisessemos desenhar esse número em binário ficaria da seguinte forma: 1100 : 11110 : 101111
Mas conseguimos deixar algo mais simples, já que assim que terminassemos de converter os números binários, os segundos já mudariam: 0001 0010 : 0011 0000 : 0100 0111
Agora nós temos 4 digítos binários para representar cada número decimal do horário, já que os números só vão até 9, fica muito mais fácil converte-los. O nome disso é *binary-coded decimal*, ou BCD.
O BCD é pouco utilizado dentro da arquitetura de computadores, pelo fato que ele dificulta muito operações aritméticas, como adição e subtração, mas para mostrar horários representando números decimais ele funciona bem.
Para fazer isso, nós precisamos definir a sequência de dígitos que vamos precisar mostrar:
- O primeiro dígito de segundos vai de 0 a 10
- O segundo dígito de segundos vai de 0 a 5
- O primeiro dígito do minuto vai de 0 a 9
- O segundo dígito de minuto vai de 0 a 5
- O primeiro dígito das horas vai de 0 a 9
- O segundo dígito das horas vai de 0 a 1

Quando chega no último dígito da sequência, ele volta a 0. Começando com os primeiros dígitos, podemos usar um edge-triggered flip flop em linha. Nós usamos um Clock que tem 1 Hz de frequência, ou seja, muda de valor a cada 1 segundo, mas pensando nisso, esses flip-flops vão de 0000 a 1111, isso são 16 segundos até zerar, e isso não é o que queremos, nós queremos que quando chegue em 1001 (9) ele ativa o Clear em todos os flip-flops, para isso conectamos um AND no Q do segundo e no último flip-flop, e conectamos o output dele ao sinal de Clear e todos os flip-flops, assim antes do circuíto mostrar o 1011, ele limparia todos os dados de dentro dele, retornando a 0.
Agora que nós temos o sinais dos primeiros dígitos, que vão de 0 a 9, nós precismos que toda vez que ele chegue até 9 e retorne para 0, mande um sinal para que o segundo dígito possa subir. Para que possamos resolver esse problema, podemos conectar um gate NAND no primeiro e no útimo flip-flops para mandarmos um sinal para o próximo circuíto, o output do NAND sempre vai ser 1, e quando o contador chegar até 1001, ele oscila de 0 a volta para 1.
O próximo circuíto, que vai receber o sinal do NAND, ele vai servir para contar de 000 a 110 (6), vamos usar o mesmo fundamento do que os flip-flops passados, vamos conectar um AND no último e no bit do meio, e um NAND no último (mais valioso) e no primeiro bit (menos valioso), O AND vai servir como sinal para mandar um Clear para todos os flip-flops e o NAND vai servir como output para o próximo circuíto.

Nós repetimos o primeiro circuíto, só que agora com o input vindo do circuíto de 1 minuto. E fazemos a mesma coisa com o segundo dígito dos minutos, são exatamente os mesmo circuítos dos segundos, mas com outputs diferentes.
Os relógios convencionais contam as horas de 00 a 23, mas para esse caso, nós vamos construir um relógio com o padrão americano, que é o padrão 12 horas, mas para fazermos nós enfrentamos um pequeno problema, as horas não começam em 0 e sim em 12, depois vai para 1, mas vamos ignorar isso por enquanto, vamos partir do pressuposto que as horas vão de 00 a 11.
Para fazer isso, temos dois pequenos problemas, o primeiro é que nos minutos e nos segundos, os dígitos maiores e menores são limpos independetemente do outro, quando o dígito menos chega a 1010, e quando o maior chega a 110, nas horas, o dígito também funciona quando chega a 1010 e é limpo, mas precisamos considerar quando o dígito maior é 1 e o segundo dígito é 0010, isso é a transição de 11 horas para 00, isso significa que devemos considerar ambos os dígitos na hora de resetar as horas:
DFF(in=d4, clk=clk_ff4, out=q4, out=q4_not);
DFF(in=q4, clk=clk, out=q3, out=q3_not);
DFF(in=q3, clk=clk, out=q2, out=q2_not);
DFF(in=q2, clk=clk, out=q1, out=q1_not);
DFF(in=q1, clk=clk, out=q0, out=q0_not);
Nand(a=q4, b=q0, out=period12);
Or(a=q0, b=q1, out=or1);
And(a=q4, b=or1, out=and1);
Not(in=q3, out=not3);

Os 4 primeiros flip-flops funcionam muito parecido com os outros de dígitos menores, mas o último AND é responsável por verificar quando o dígito maior é 1 e o menor é 0010.
Agora conseguimos montar um circuíto que conta de 00 até 11 horas, mas ainda queremos resolver o problema de mostrar o 12 ao invés do 00, isso pode ser resolvido com um 5 input NOR:
DFF(in=d4, clk=clk4, out=q4, out=q4_not);
DFF(in=d3, clk=clk, out=q3, out=q3_not);
DFF(in=d2, clk=clk, out=q2, out=q2_not);
DFF(in=d1, clk=clk, out=q1, out=q1_not);
DFF(in=d0, clk=clk, out=q0, out=q0_not);
Or(a=q0, b=q1, out=or_in0);
Or(a=q4, b=q3, out=or_in1);
And(a=q4, b=or_in0, out=and_in0);
Nand(a=q3, b=q2, out=nand_in0);
Not(in=q2, out=not_in0);
Nor(a=q4, b=q3, c=q2, d=q1, e=q0, out=nor_out);
Nand(a=q4, b=q0, out=period12);
Or(a=period12, b=q3, out=clk4);
Or(a=q1, b=q0, out=d4);

O NOR só vai retornar 1 quando todos os flip-flops virarem 0, e são conectados em mais dois OR's, e agora ao invés do relógio mostrar 0 0000, vai mostrar 1 0010.
O NAND no final do código, é normalmente 1, menos quando o horário é 1 0001, daí o output vai para 0, isso pode funcionar como um sinal de AM PM.
Cada um dois 6 circuítos tem um NAND conectado que serve para mandar um sinal para o próximo circuíto, o output dele é 0 a menos quando as entradas são 0, aí o output dele muda para 1.
250
