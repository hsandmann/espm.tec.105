# Ambiente de Produção

## Máquina de Turing

Proposta pelo matemático [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing), trata de uma máquina de computação universal que tem funcionalidade processar símbolos e suportar programação dinâmica<sup>[1](##Referências)</sup>. 

De forma resumida, a máquina de Turing propõe um cabeçalho e uma fita, onde o cabeçalho lê símbolos da fita executa a operação ali descrita. Generalizando, é uma forma de construir um autômato.

![Máquina de Turing](/assets/img/turing_tape_header.png)

O funcionamento da máquina se resume ao algoritmo de:
```
1. Ler o posição da fita;
2. Interpreta o símbolo;
3. Executa a operação ali descrita;
4. Vai para a próxima posição da fita;
5. Volta para o passo 1.
```
 
Ao analisar o resumo do algoritmo, é possível levantar a questão da parada da máquina, um problema tratado no artigo de Turing.

Confira uma animação da máquina de Turing em: [https://youtu.be/gJQTFhkhwPA](https://youtu.be/gJQTFhkhwPA)

## Arquitetura von Neumann

Baseando na teoria da máquina de Turing, o físico e matemático [John von Neumann](https://en.wikipedia.org/wiki/John_von_Neumann) desenvolveu uma arquitetura que era capaz de executar tal tarefa: arquitetura de Von Neumann ou arquitetura de Princeton.

![von Neumann Architecture](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Von_Neumann_Architecture.svg/2880px-Von_Neumann_Architecture.svg.png)
*![Wikipedia](https://en.wikipedia.org/wiki/Von_Neumann_architecture)*

Onde o cabeçalho passa a ser uma CPU (Central Processing Unit), que lê os símbolos da fita - a fita moderna é a memória RAM - e executa uma operação. A operação por sua vez está construinda em portas lógicas e contída em uma área da circuitaria chamada ALU (Arithmetic/Logic Unit).

A maoria dos computadores modernos são construídos sobre a *praxis* de uma arquitetura von Neumann. 

## Simulador ESPM 16bits

A fim de simular um processador moderno de forma didática, o ESPM 16bits apresenta as principais características de um processador moderno e permite a sua programação utilizando um Assembly de 16 instruções.

Como na arquitetura de von Neumann esse computador é composto por memória e CPU.

A CPU possui registradores, são eles:

| Registrador | Descrição |
| --- | --- |
| AC  | Acumulador, registrador mais importante, onde as operações são executadas |
| IC  | Contador de instrução, é a posição do cabeçalho na fita, ou seja, do processador em relação a memória |

Já a ALU (ULA em português) possuí 16 instruções, sendo elas:

| Opcode | Mnemônico | Descrição | 	
| --- | --- | --- |
| 0      | JMP       | Desvio incondicional |
| 1      | JZ        | Desvio se acumulador for zero |
| 2      | JNZ       | Desvio se acumulador não for zero |
| 3      | LV        | Deposita uma constante no acumulador |
| 4      | ADD       | Soma |
| 5      | SUB       | Subtração |
| 6      | MUL       | Multiplicação |
| 7      | DIV       | Divisão |
| 8      | LOAD      | Carrega da memória no acumulador |
| 9      | STOR      | Grava do acumulador na memória |
| A      | SC        | Desvio de subprograma (função) |
| B      | RS        | Retorno de subprograma (função) |
| C      | END       | Fim de programa |
| D      | IN        | Entrada |
| E      | OUT       | Saída |
| F      | NOP       | Ciclo de processamento nulo |

A simulação está disponível em:
[ESPM 16bits](/espm.16bits)

## Sistemas Operacionais (SO)
1. [Resumo SO](/assets/pdf/ESPM-ResumoSO.pdf)

### Memória

### Arquivos

### Processos

### Dispositivos

### Usuários

#### Ubuntu

##### Criar usuário

``
$ sudo adduser <username>
``




## Referências

1. Turing, A. M. (1936). ["On Computable Numbers, with an Application to the Entscheidungsproblem"](/assets/pdf/Turing_1936.pdf)
2. Gödel, K. (1931). ["Über formal unentscheidbare Satze der Principia Mathematica und verwandter Systeme, I"](/assets/pdf/Godel_1931.pdf)
