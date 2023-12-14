# MorseCode Numbers

Esta implementação contempla o uso de um módulo buzzer (figura abaixo) como periférico. Que recebe um sinal de entrada e converte para um sinal sonoro itermitente que é representado por pontos e traços. Atualmente está implementado os números do código morse.
# modulo buzzer 

O ponto tem o periodo de T e o traço 3T emitindo som, intervalo entre caracter tem 3T e entre palavras 7T. O período T pode variar de acordo com a experiência do operador de código morse.
# imagem da tabela de codigo morse numeros 

Este periférico possui 3 pinos, VCC de 3V3, GND e o pino de controle, no qual envia um sinal que emite som quando '0' e fica sem som quando '1'

Utilizou-se uma tabela para converter a entrada em pontos e traços (pontos são represnetados por '0' traços representados por '1') e uma maquina de estados para realizar os diferentes periodos de operação 

# imagem da maquina de estados 

# Simulação
A primeira simulação foi feita ainda antes do periférico ser implementado no projeto como um todo e pode ser visto nos arquivos [testbench2.vhd](https://github.com/luiz-sene/riscv-multicycle/blob/master/peripherals/keyboard/testbench2.vhd) e [testbench2.do](https://github.com/luiz-sene/riscv-multicycle/blob/master/peripherals/keyboard/testbench2.do)
