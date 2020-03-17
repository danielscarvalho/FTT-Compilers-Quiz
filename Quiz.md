# Compilers Quiz
## CEFSA - FTT - EC

- Use notação **markdown** para responder
- Faça um **fork** e depois **pull request**

### Fase de análise - front-end

1) Qual a diferença entre uma linguagem compilada e uma linguagem interpretada? Cite exemplos de linguagens.

__R: Uma linguagem compilada é executada diretamente pelo sistema operacional/processador, depois do código fonte ser transformado em código de máquina pelo compilador. Uma linguagem interpretada depende de um intermediário (virtual machine), que é o responsável por interpretar o código fonte e compilá-lo, em tempo de execução, tranformando-o em código de máquina para que o processador consiga executar o programa.__

__Exemplos:

Linguagens interpretadas: Javascript, Lua, Python

Linguagens compiladas: Cobol, Fortran, Java, C# e Pascal.__

2) Quais são os prós e contras entre linguagens compiladas e interpretadas?

3) Qual a diferença entre assembler e assembly?

__R: Assembly é uma linguagem de programação legível para nós humanos, com maior facilidade de assimilação, desenvolvimento e análise. Assembler é um compilador de programas Assembly, ou seja, ele é um tradutor, um programa ou conjunto de programas que transformará a linguagem de alto nível entendida pelo homem para um linguagem de baixo nível, a linguagem de máquina. O Assembler é o responsável por gerar o arquivo binário a partir do código Assembly. ~ Respondido por Fabio e Matheus Barreto__  __Revisado por Matheus Alberto e Mateus Moura__

__R: Assembly pode ser considerada uma linguagem intermediária, que se aproxima muito a linguagem de baixo nível, isto é, linguagem de máquina. O Assembler gera um código de máquina relocável, a partir do Assembly. Isto é, o Assembler o processo de atribuir endereços de memória para as várias partes do programa e ajustar o código e dados no programa para refletir os endereços atribuídos. (Eduardo Alves - 082170006)

4) O que é lexema?

__R: Um lexema é uma sequencia de caracteres no programa fonte que casa com o padrão para um token e é identificado pelo analisador léxico como uma instancia desse token. ~ Mateus Moura e Matheus Alberto.__  __Revisado por Matheus Barreto e Fabio__

5) Qual é o autômato finito que representa a expressão regular: [a-zA-Z_0-9] e o que ela está reconhecendo?
__R: Essa expressão regular reconhece caracteres de A a Z, maiúsculos e minúsculos, o símbolo _ e números de 0 a 9.__

6) Por que é interessante desenvolver programas em linguagem de alto nível ao invés de utilizar direto código de máquina? 

__R: Porque softwares desenvolvidos em linguagem de alto nível são mais fáceis de se ler, entender e, portanto, manter. Com o grande avanço e aperfeiçoamento dos compiladores até os dias de hoje, um código em alto nível pode ser traduzido para uma linguagem de baixo nível, mantendo uma performance satisfatória. - Murilo Kakazu__

7) Estabeleça uma regra para criar nomes de variáveis em uma linguagem de programação, e defina sua expressão regular e autômato finito.
__R:Só poderam ser criadas variaveis que contenham letras ou numeros ou _, tendo obrigatoriamente no começo uma letra, nao podendo contar caracteres especiais, espaço ou pontuações. Regexp: ^[a-zA-Z_$][a-zA-Z_$0-9]*$ .__

8) Qual a diferença entre analisador sintático e semântico?
__R: O analisador sintático prepara a árvore sintática e a encaminha ao analisador semântico que analisa os lexemas separados, verificando a semântica gerada anteriormente. Enquanto o analisador sintático verifica se os tokens pertencem à linguagem livre de contexto, a semântica verifica se os valores e as declarações correspondem ao padrão solicitado.__

9) Explique o analisador semântico.
__R: Verifica os erros semânticos referentes ao escopo em que uma variável foi declarada, fazendo a ligação entre seu tipo, nome e valor, além de  validação de tipo. Ex: Correspondência entre declarações de variáveis.__

10) Quais as fases de compilação?

__R: Análise e Síntese. (Sub-fases descritas na questão 16) ~Raquel Sales__

11) Onde as linguagens de programação, regexp e os idiomas (inglês, português e francês) se encaixam na hierarquia de Chomsky?
__R: Os idiomas estão contidos na categoria 0, recursivamente enumeraveis e identificados apenas pelo maquina de Turing. As linguagens de programação se encontram na categoria 2, reconhecidas por automatos finitos com pilha e o regexp se encontra na categoria 3 reconhecida por autômato finito, pois são as linguagens regulares.__

12) Como se chama um programa que converte uma linguagem de programação de alto nível em outra, e porque isso é interessante?

__R: É chamado de transpilador (ou Source-to-source compiler), ele é interessante pois podemos escrever código em versões
melhoradas de linguagens que não são suportadas nativamente pelo sistema e então transpilar esses códigos para algo que
o sistema suporte.
Exemplos: Sass e Less para Css, Jade para HTML, TypeScript para JavaScript, EcmaScript 8 para versões anteriores, etc. ~Laion__



13) O que são OPCODEs e mnemônicos? 

__R: OPCODEs são codigos de operação que identificam uma instrução que será realizada pelo processador.
Mnemônicos são sequencias de caracteres que lembram uma palavra e podem executar um OPCODE.__


14) O que pode ser programado em assembly que não pode ser feito em linguagens de alto nível?

__R: Nada. ~Raquel Sales__
__R: Qualquer programação em assembly pode ser feita com linguagem de alto nível, pois as instruções contidas nestas linguagens representam uma série de instruções em assembly de modo que otimize o tempo de programação e facilite a manutenção e interpretação do código. Além disso, de acordo com a Lei de Moore, qualquer linguagem de programação com instruções sequenciais, loops e condições (como assembly e nas linguagens de alto nível), permite a criação de qualquer programa. ~Bruno Chaves__

15) Porque há engenheiros que programam em assembly atualmente?

__R: Existem engenheiros que programam em assembly atualmente pois em alguns momentos do desenvolvimento de código C, os profissionais acabam percebendo que certos pedaços do código estão com uma performance menor do que a esperada, logo este trecho do código é convertido para linguagem assembly, melhorando assim sua performance.
Além disso também existem alguns microcontroladores que só podem ser programados em linguagem assembly.__

16) Explique cada uma das fases de compilação.

__R: Análise Sintática: 
 - Verifica a estrutura gramatical da tabela gerada pela analise lexica;
 - Verifica se a sentença pertence a linguagem;
 - Recebe os tokens e gera árvore de derivação (Observação: os tokens são os símbolos terminais da GLC).__

__Análise semântica: 
 - A informação é adiciada a árvore;
 - Verificação de tipos e erros;
 - Verifica inicialização de variáveis;
 - Verifica tipos de objetos;
 - Prepara a geração de códigos. ~Raquel Sales__
__R: Análise Lexica:
 - lê o arquivo de código fonte
 - ela faz o papel do Scanner que por sua vez, analisa caracter por caracter até achar um caracter de parada, geralmente um espaço ou um; conforme a sintaxe da linguagem.
 - Assim reconhece como um lexima e o coloca em uma tabela de leximas(tokens)
 - Ela pode reconhecer por exemplo, se um nome de uma variavel está iniciando com um número por meio de uma regexp e emitir 
 um erro. ~Bruno N.__

17) Explique processador RISC e CISC.
__R: Processador Cisc (Complex Instruction Set Computer) é capaz de executar centenas de instruções complexas e mais rapidamente, enquanto que o Risc (Reduced Instruction Set Computer) consegue executar poucas instruções simples por vez, ~~por essa razão ele se torna
mais barato~~. ~Michele.__

__R: Without commercial interest, processor developers were unable to manufacture RISC chips in large enough volumes to make their price competitive. [RISC vs. CISC](https://cs.stanford.edu/people/eroberts/courses/soco/projects/risc/risccisc/)__

18) Qual a diferença entre linguagens estáticas e dinâmicas, cite linguagens destes dois tipos.

__R: A diferença está relacionada a uma "exigência" da linguagem na declaração de suas variáveis. Nas linguagens estáticas, ao se declarar uma variável, o tipo deve ser obrigatoriamente informado. Quando houver uma atribuição de valor, o compilador se encarrega de verificar se o dado informado corresponde ao tipo declarado. Nas linguagens dinâmicas não é necessário declarar o tipo da variável. Nesse caso, a correspondência entre o valor atribuído à uma variável e seu tipo é feita em tempo de execução,  não durante a compilação. Java e C# são linguagens estáticas, enquanto JavaScript, Python, Ruby e PHP são linguagens dinâmicas. ~Armando Dias.__

19) Os seguintes termos se aplicam a quais linguagens de programação?

| ID | Tipo |
| ---|---| 
| A | Imperativo |
| B | Declarativo |
| C | Dinâmica |
| D | OO |
| E | Funcional |
| F | Tipada |
| G | Não tipada |
| H | Compilada |
| I | Interpretada |


 | ID | Linguagem |
 | --- | --- |
 | 1 | C |
 | 2 | C++ |
 | 3 | COBOL |
 | 4 | Fortran |
 | 5 | Java |
 | 6 | Lisp |
 | 7 | SQL |
 | 8 | Perl |
 | 9 | Python |
 |10 | VB |
 |11 | Lua |
 |12 | HTML |
 |13 | PHP |
 |14 | C# |
 |15 | Wolfram Language |
 
 _RESPOSTA:_
 | Tipo | Linguagem |
 | --- | --- |
 | A,F,H | C |
 | A,D,F,H | C++ |
 | A,H | COBOL |
 | A,F,H | Fortran |
 | A,C,D,F,H | Java |
 | B,E,I | Lisp |
 | B,I | SQL |
 | A,C,D,I | Perl |
 | A,C,D,I | Python |
 | A,D,H | VB |
 | A,C,D | Lua |
 | B | HTML |
 | A,C,D | PHP |
 | A,C,D | C# |
 | A,C,D | Wolfram Language |

20) O que é e dê exemplos de linguagens dinamicamente tipadas.

__R: são linguagens que o tipo da variavel não é determinada quando declarada, ela assume o tipo de acordo com o codigo.
Exemplo: Javascript.__

21) O que são linguagens fortemente tipadas e fracamente tipadas? Cite exemplos.
__R:Linguagens fortemente tipadas são linguagens que exigem que na declaração da variável o seu tipo seja obrigatoriamente explicitado. Como por exemplo, na linguagem Java devemos escrever as variáveis da seguinte maneira:
	int numero = 0;
		String texto = “olá mundo”;
	Boolean flag = true;
São exemplos de linguagens fortemente tipadas: Java, C#, C++, C, COBOL, Fortran.
Já nas linguagens fracamente tipadas o programador não deve explicitar o tipo da variável pois a linguagem é capaz de identificar o tipo da variável de acordo com o valor que a variável assume em tempo de execução do programa. Nas linguagens com essa tipagem, uma variável pode alterar seu tipo quantas vezes forem necessárias, sempre de acordo com o valor que recebe. Abaixo um exemplo de como são declaradas as variáveis em Javascript, que é uma linguagem fracamente tipada.

__R:|	x = 5
	ou 
	var x = 5|
Neste caso, o programa assume que a variável x é do tipo int.
	__R:|y = ”ola mundo”
	ou
	var y = “ola mundo”|
	Neste caso o programa assume que a variável y é do tipo string.
São exemplos de linguagens fracamente tipadas: PHP, Javascript, Ruby, Python.

22) O que é um bloco de código?

__R: Blocos de programação são aglomerados de instruções e declarações que têm escopo conjunto. Ou seja, as variáveis definidas como locais dentro de um bloco somente serão presentes dentro deste bloco assim como as instruções ali presentes. Geralmente são delimitados por chaves ({...}) e podem ser aninhados - colocados um dentro do outro__

23) Por que variáveis devem ser inicializadas antes do uso?
__R: As variáveis são apontadores para endereços de memória. Devem ser inicializadas antes de ser atribuídas pois precisam realizar um alocamento de memória compatível com o dado que será guardado. Não há como armazenar um objeto criado a partir de uma classe em uma variável que alocou memória suficiente para um tipo Inteiro. ~Jorge Henrique__

24) SQL é uma linguagem declarativa ou imperativa? Porque?

__R: SQL é uma linguagem declarativa. Por que você especifica como quer o resultado, mas exatamente como o banco de dados irá achar o resultado desejado é problema dele. SQL padrão não é uma linguagem de programação. Com algumas extensões pode ser. Uma linguagem imperativa é aquele que o programador define como o algoritmo deve funcionar. Felipe__

25) Quais as duas partes/fases principais de um compilador?
__R: Fase de síntese e fase de análise.__

26) Qual a diferença entre tokens, patterns e  lexema.
__RTokens, patterns e lexemas são termos relacionados a implementação de um analisador léxico.
Token – É um par composto pelo nome do token e um valor de atributo (opcional).  O nome do token é sempre um símbolo abstrato que representa a unidade léxica, por exemplo: Palavras reservadas, números, identificadores e etc.
Padrão – É a forma que os lexemas de uma cadeia de caracteres podem assumir, por exemplo: o padrão de uma palavra reservada é a sequência de caracteres que fazem parte da formação da palavra; O padrão de um identificador é a sequência de caracteres que fazem parte da formação dos nomes de variáveis e funções.
Lexema – É uma sequência de caracteres reconhecidos por um padrão.

27) Explique a fase de análise léxica.

__R: A análise léxica consiste na primeira análise realizada durante o processo de compilação e tem por objetivo identificar os denominados lexemas, e transformá-los em tokens que formarão a tabela de lexemas. Um ponto importante dessa etapa, é que ela se assemelha a um scanner, pois passa por todo o código e "enumera" as variáveis sem se aprofundar em sua aplicação.__

__R: A fase de análise léxica é responsável por scannear ao código, fazendo uma varredura por todo código procurando por algo que não faça parte da biblioteca da linguagem de programação em questão. 

28) Escreva uma expressão reguar que reconheça números ponto flutuantes: 1.2, 3, 4.50, .03, 0.000032, -0.2, +3.0014

__R: ^[-+]?[0-9]*\.?[0-9]+$

29) Porque estudamos compiladores?
__R: Para que seja possível obter maior conhecimento sobre o processo de geração de um software, entendendo intrinsecamente, a partir da camada de mais alto nível, quais as ações necessárias para torná-las entendíveis para as máquinas, ou seja, baixo nível, porém mantendo a funcionalidade equivalente à estrutura inicial.__

30) Qual a diferença do Scanner e Parser?
__R: O Scanner realiza a análise dos símbolos inseridos no código e é ligado ao processo de análise léxica. Já o Parser tem a função de verificar o conjunto de símbolos e está ligado ao processo semântico de compilação.

31) Que tipo de linguagem pode ser reconhecida pela máquina de Turing?
__R: Qualquer linguagem pode ser reconhecida. Pois seu conceito é de um computador na esfera teórica, abstraído apenas de seus aspecos lógicos. ~ Lucas__

32) Com base na figura abaixo, explique o processo de compilação:

__R: O processo de compilação é definido por 6 etapas, sendo elas:
Analisador Léxico: Converte a sequência de caracteres do código fonte em tabela de palavras ou tokens(Scanner)
Analisador Sintático: Converte a sequência de token sem uma arvore (parse tree) de forma hierárquica
Analisador Semântico: Manipula a arvore para símbolos e tipos
Gerador de código intermediário: Converte a arvore e uma sequência intermediária de instruções
Otimizador de código: Manipula o código para otimização
Gerador de código objeto: Converte o código otimizado para linguagem de máquina (Assembly)

__R: Analisador Léxico: É um scanner que faz a varredura do código, procurando algo que não faça parte da linguagem.
Analisador Sintático: É responsável por verificar se a sequência de símbolos geram um programa válido ou não.
Analisador Semântico: É responsável por verificar a estrutura já construída e para ser executada. Verifica inicialização de variáveis.
Gerador de código intermediário: Gera o primeiro código do programa, na linguagem assembly.
Otimizador/Gerador de código: Otimiza desempenho e uso de memória e após isso gera um executável final, eficiente para o hardware específico. (Eduardo Alves - 082170006)

33) Qual a diferença entre erro de sintaxe e erro semântico?
__R: A diferença entre um erro de sintaxe e um erro semântico é que no erro sintático ele apresenta um erro quando não consegue entender aquela instrução escrita, como por exemplo estar escrito “FORM” ao invés do “FROM” em uma consulta do SQL. Já no erro semântico, se trada de quando compilador não entende o significado daquilo escrito no código.

34) Write a regexp that accepts all strings of a's and b's that do not contain the subsequence “abb”.
__R:^(a(?!(b{2}))|b)+$

35) Escreva uma expressão regular que reconheça vogais em letras maiúsculas e consoantes em legras minúsculas
__R:([AEIOUbcdfghjklmnpqrstvwxyz]) Respondido por Carlos e Caue - 082170042/081170042__ (Revisada por Letícia Jordão e Gabriel Teixeira)


36) Exercise 3.3.4 : Most languages are case sensitive, so keywords can be written only one way, and the regular expressions describing their lexemes are very simple. However, some languages, like SQL, are case insensitive, so a keyword can be written either in lowercase or in uppercase, or in any mixture of cases. Thus, the SQL keyword SELECT can also be written select, Select, or sElEcT, for instance. Show how to write a regular expression for a keyword in a case-insensitive language. Illustrate the idea by writing the expression for select in SQL.

__R: ([A-Za-z])+ Respondido por João Machado e Igor Cruz - 081170036/081170008
 
37) Qual a diferença entre erro de sintaxe e erro semântico?
__R: Erros de sintaxe estão resumidos a características não obedecidas há regras na forma lógica em que seus símbolos estão dispostos em uma linguagem e como se comportam, tal como sequência de palavras ou uso de parenteses (abertura e fechamento). 
Já erros da esfera semântica estão relacionados a problemas de significados na linguagem ao tentar passar a informação desejada, assim como em uma linguagem natural, pode estar gramáticamente correta porém não haver sentido algum, um código pode seguir todas as regras gramaticais da linguagem e possuir instruções sem sentido lógico, como atribuir uma variávelo declarada como string e, ao mesmo tempo ser atribuida a um inteiro. ~ Lucas__ 

38) Write a regexp that accepts all strings of digits with no repeated digits. Hint: Try this problem with a few digits, such as {0; 1; 2}.
__R: ^(?:(?!([0-2])\1).)*$ ~Respondido por Fabio e Matheus Barreto__ __Revisado por Matheus Alberto e Mateus Moura__

39) Que tipo de linguagem o NFA e DFA podem reconhecer?
__R: Linguagens regulares que podem ser expressas usando expressões regulares, ou seja, uma linguagem produzida utilizando as operações de concatenação, união e fecho de Kleene sobre os elementos de um alfabeto.
Respondido por *Jonatas João - 081170035*

40) Qual é a expressão regular para o autômato:https://pt.wikipedia.org/wiki/Ficheiro:NFAexample.svg, seja M = ({s0, s1, s2, s3, s4}, {0, 1}, Δ, s0, {s1, s3}) onde a função de transição Δ é definida pela tabela de transição de estados abaixo:

|  | 0 | 1 | ε |
| ---|---|---| ---|
| S0 | {} | {} | {S1, S3} | 
| S1 | {S2} | {S1} | {} |
| S2 | {S1} | {S2} | {} |
| S3 | {S3} | {S4} | {} |
| S4 | {S4} | {S3} | {} |

__R: (1*(01*01*)*) ∪ (0*(10*10*)*)
Respondido por *Jonatas João - 081170035*

41) Escreva um autômato que reconheça: A|E JK U|O
__R: **->Q0->(AEIOU)->Q1(ESTADOFINAL)->ESPAÇO->Q2->(BCDFGHJKLMNPQRSTVWXYZ)->Q2 ->(BCDFGHJKLMNPQRSTVWXYZ)->Q3->(ESPAÇO)->Q0**
Respondido por *Carlos e Caue - 082170042/081170042*__

42) Escreva um autômato que reconheça: 
```html
<H1>
```
e
```html
</H1>
```
R:[<][/]*[H][1][>] (Letícia Jordão e Gabriel Teixeira) 

43) HTML e CSS são linguagems (de marcação) declarativas ou imperativas? Explique?
__R:  São linguagens de marcação (declarativas), pois nelas o programador fornece apenas o conjunto das tarefas a serem realizadas, não estando preocupado com os detalhes de como o executor da linguagem realmente implementará essas tarefas. ~Rodrigo__ (Revisada por Letícia Jordão e Gabriel Teixeira)
44) Defina a tabela de símbolos.

__R: Tabela de símbolos é uma estrutura de dados, geralmente uma árvore ou tabela de hash, utilizada em compiladores para o armazenamento de informações de identificadores, tais como constantes, funções, variáveis e tipos de dados. É utilizada em quase todas as fases de compilação, como a varredura, a análise sintática, a análise semântica, otimização e geração de código. Em cada fase ela pode ser utilizada como base para comparações ou mesmo atualizada com novos identificadores durante a saída de cada fase.

45) Qual é a entrada e a saída da fase de análise sintática?
__R: A análise sintática (segunda fase de compilação) tem como entrada um conjunto de tokens, após a realização da análise léxica (primeira fase de compilação), e tem como saída a árvore de derivação (parser tree)

46) De exemplos de parsers.

47) Que tipo de linguagem um automato finito reconhece?
__R: Um automato finito reconhece linguagens que são regulares, ou seja, são descritas por expressões regulares. ~ Mateus Moura e Matheus Alberto.__ __Revisado por Matheus Barreto e Fabio__

48) Quais ferramentas (softwares) podemos utilizar para nos ajudar a criar um compilador? Como elas se integram?

49) O que representa o "id" na tabela de símbolos?
__R: Durante a criação da tabela de símbolos, na fase de análise léxica, todas as variáveis do código, que está sendo compilado, são salvas com o nome de "id", sendo distinguidas a partir de então pela posição em que estão na string (já reduzida para uma string única) do código. Logo, os "id" na tabela de símbolos, são as variáveis do código compilado. ~Filipe__
50) Quais as linguagens/compiladores criadas por brasileiros?
R: Elixir, Lua (Letícia Jordão e Gabriel Teixeira)

### Fase de síntese - back-end

---------------

*Respostas na bibliografia, "Livro do Dragão" na biblioteca virtual* e físico na biblioteca "Compiladores - Princípios, Técnicas e Ferramentas, Sethi,Ravi, Aho,Alfred V."

