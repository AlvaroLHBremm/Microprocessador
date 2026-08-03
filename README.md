# Processador programavel de 8 bits.

Projeto pessoal desenvolvido no simulador Deeds com o objetivo de simular a arquitetura de um processador hipotético de 8 bits. 
Video descritivo e simulação: https://www.youtube.com/watch?v=KcWQU9CIYoI&t=136s

![image alt](https://github.com/AlvaroLHBremm/Processador-programavel-de-8-bits/blob/main/Estrutura%20do%20Processador.png?raw=true)

Seções:
* Vermelho:  Unidade de controle: Decodificador de instruções e maquina de estado
* Azul:      Unidade lógica arimética e flags de jump
* Verde:     Controle de fluxo de memória: ROM, RAM, Program counter.

Descrição:
* É possivel programar codigos em assembly/código de maquina para ser executado pelo processador.
* O processador carrega da memoria ROM para RAM o código quando pressionado o botão de ligar.
* Ao apertar o botão de executar a unidade de controle lê e executa as instruções presentes na RAM.
* Unidade de controle decodifica instruções e controla o fluxo de dados.
* Unidade logica aritmética realiza calculos e sinaliza estados de flags.

### Tabela de instruções
| Instruções | Syntax | Descrição |
| :--- | :--: | :--- |
| `LDA` | [0x10][0xXX] | Carrega endereço X de memória ao acumulador. |
| `STA` | [0x20][0xXX] | salva acumulador para endereço X de memória. |
| `ADD` | [0x30][0xXX] | Soma acumulador com endereço X de memória. |
| `NOT` | [0x40]____ | Inverte acumulador. |
| `AND` | [0x50][0xXX] | Realiza operação AND bitwise com endereço X de memória. |
| `OR`  | [0x60][0xXX] | Realizar operação OR bitwise com endereço X de memória. |
| `JMP` | [0x70][0xXX] | Pulo sem condição para X endereço de memória. |
| `JZ`  | [0x71][0xXX] | Pulo para endereço X de memória quando acumulador igual a 0. |
| `JN`  | [0x72][0xXX] | Pulo para endereço X de memória quando acumulador é negativo. | 
