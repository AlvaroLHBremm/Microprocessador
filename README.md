# Processador programavel de 8 bits.

Projeto pessoal desenvolvido no simulador Deeds com o objetivo de simular a arquitetura de um processador hipotético de 8 bits. 
Video descritivo e simulação: https://www.youtube.com/watch?v=KcWQU9CIYoI&t=136s

![image alt](https://github.com/AlvaroLHBremm/Processador-programavel-de-8-bits/blob/main/Estrutura%20do%20Processador.png?raw=true)

Seções:
* Vermelho:  Unidade de controle
* Azul:      Unidade lógica arimética e flags
* Verde:     Controle de fluxo de memória

Descrição:
* É possivel programar codigos em assembly/código de maquina para ser executado pelo processador.
* O processador lê e executa instruções, carregando-as da memoria ROM para RAM. 
* Unidade de controle decodifica instruções e controla o fluxo de dados.
* Unidade logica aritmética realiza calculos e sinaliza estados de flags.

| Instruções | Descrição |
| :---: | :--- |
| `LDA_[20][XX]` | Carrega endereço X de memória ao acumulador. |
| STA_[20][XX] | salva acumulador para endereço X de memória. |
| ADD_[30][XX] | Soma acumulador com endereço X de memória. |
| NOT_[40]____ | Inverte acumulador. |
| AND_[50][XX] | Realiza operação AND bitwise com endereço X de memória. |
| OR__[60][XX] | Realizar operação OR bitwise com endereço X de memória. |
| JMP_[70][XX] | Pulo sem condição para X endereço de memória. |
| JZ__[71][XX] | Pulo para endereço X de memória quando acumulador igual a 0. |
| JN__[72][XX] | Pulo para endereço X de memória quando acumulador é negativo. | 
