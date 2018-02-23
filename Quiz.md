# Compilers Quiz
## CEFSA - FTT - EC

1) Qual a diferença entre uma linguagem compilada e uma linguagem interpretada? Cite exemplos de linguagens.

__R:Uma linguagem compilada é executada diretamente pelo sistema operacional/processador, depois do código fonte ser transformado em código de máquina pelo compilador. Uma linguagem interpretada depende de um intermediário (virtual machine), que é o responsável por interpretar o código fonte e compilá-lo, em tempo de execução, tranformando-o em código de máquina para que o processador consiga executar o programa.__

Exermplos:

Linguagens interpretadas: Javascript, Lua, Python

Linguagens compiladas: Cobol, Fortran, Java, C# e Pascal.

2) Quais são os prós e contras entre linguagens compiladas e interpretadas?

3) Qual a diferença entre assembler e assembly?
__R: Assembly é uma linguagem de programção de baixo nível mas ainda inteligível pelos programadores, assembler é o programa montador
que transforma as instruções escritas na linguagem assembly para códigos binários e endereços de memória, instruções de baixo nível (instruções de máquina) que serão utilizadas diretamente pelo processador.

4) O que é lexema?
__R:O analisador léxico lê um fluxo de caracteres que compõem o programa fonte e os agrupa em seqüências significativas, chamadas lexemas. (Curiosidade: Para cada lexema, o analisador léxico produz como saída um token no formato). ~Raquel Sales__

5) Qual é o autômato finito que representa a expressão regular: [a-zA-Z_0-9] e o que ela está reconhecendo?

6) Porque é interessante desenvolver programas em linguagem de alto nível ao invés de utilizar direto código de máquina? 
__R: Porque a linguagem de alto nível é mais intuitiva ao usuário, sendo assim mais produtiva e inteligível. Ao invés de digitar inúmeras linhas na linguagem de baixo nível, o usuário pode apenas chamar funções prontas - que ele consiga entender o intuito - na linguagem de alto nível.__

7) Estabeleça uma regra para criar nomes de variáveis em uma linguagem de programação, e defina sua expressão regular e autômato finito.

8) Qual a diferença entre analisador sintático e semântico?

9) Explique o analisador semântico.

10) Quais as fases de compilação?
__R: Análise e Síntese. (Sub-fases descritas na questão 16) ~Raquel Sales_

11) Onde as linguagens de programação, regexp e os idiomas (inglês, português e francês) se encaixam na hierarquia de Chomsky?

12) Como se chama um programa que converte uma linguagem de programação de alto nível em outra, e porque isso é interessante?

13) O que são OPCODEs e mnemônicos?

14) O que pode ser programado em assembly que não pode ser feito em linguagens de alto nível?
__R: Nada. ~Raquel Sales_

15) Porque há engenheiros que programam em assembly atualmente?

16) Explique cada uma das fases de compilação.
__R: Análise Sintática: 
 Verifica a estrutura gramatical do programa especificadas por gramática livre do contexto (GLC);
 Verifica se a sentença pertence a linguagem;
 Recebe os tokens e gera árvore de derivação (Observação: os tokens são os símbolos terminais da GLC).__

__Análise semântica: 
 A informação é adiciada a árvore;
 Verificação de tipos e erros;
 Verifica inicialização de variáveis;
 Verifica tipos de objetos;
 Prepara a geração de códigos. ~Raquel Sales__

17) Explique processador RISC e CISC.

18) Qual a diferença entre linguagens estáticas e dinâmicas, cite linguagens destes dois tipos.

19) Os seguintes termos se aplicam a quais linguagens de programação?

| ID | Tipo |
| ---|---| 
| A | Imperativo |
| B | Declarativo |
| C | Von Newman |
| D | OO |
| E | Funcional |
| F | 3G |
| G | 4G |
 
 | ID | Linguagem |
 | --- | --- |
 | 1 | C |
 | 2 | C++ |
 | 3 | COBOL |
 | 4 | Fortran |
 | 5 | Java |
 | 6 | Lisp |
 | 7 | ML ('Meta Language') |
 | 8 | Perl |
 | 9 | Python |
 |10 | VB |

20) O que é e dê exemplos de linguagens dinamicamente tipadas.

21) O que são linguagens fortemente tipadas e fracamente tipadas? Cite exemplos.

22) O que é um bloco de código?

23) Porque variáveis devem ser inicializadas antes do uso?

24) SQL é uma linguagem declarativa ou imperativa? Porque?

25) Quais as duas partes/fases principais de um compilador?
