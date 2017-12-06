# Pré requisitos/Versões das Ferramentas

um arduino;
uma protoboard;
7 fios jumper, sendo 3 pequenos e 4 médios;
um led;
um resistor de 150 ohms e um resistor de 100 ohms;
um push button;
um cabo USB para conectar o arduino no computador;
um computador com a IDE e drivers do arduino instado

# Apresentação

Você aprenderá rapidamente como acender seu primeiro LED no Arduíno

# Resposta

Nessa parte, apresentamos as duas funções necessárias para ligar e desligar o LED, digitalWrite() e delay().

Saída Digital: digitalWrite([pin], [HIGH/LOW])

A função digitalWrite() é usada para definir o estado de um pino para alto ou baixo.

O primeiro parâmetro pin serve para identificar o pino que está sendo acionado, e nos próximos experimentos vamos explorá-lo mais. Por hora, vamos nos concentrar apenas no segundo parâmetro.

Quando um pino está em HIGH, ele produz na saída uma tensão de cerca de 5V, essa tensão faz passar uma corrente através do LED e o mesmo se ilumina. Quando o pino está em LOW, a tensão e saída é de 0V, fazendo com que a corrente pare de circular e o LED fique desligado.

Antes de usar odigitalWrite(), é muito importante se certificar que o pino a ser utilizado foi previamente configurado como saída, pois do contrário, ele não vai funcionar corretamente. Para configurar o pino, nós utilizamos o comando pinMode(), que é inserido usualmente dentro do setup(). Dessa forma temos que inserir a linha de código pinMode(13, OUTPUT); por exemplo, se quisermos usar o pino D13 como saída (veremos mais sobre os pinos do Arduino nos próximos projetos).

Delay de Milissegundos: delay([ms])

O Arduino executa o código tão rápido que às vezes precisamos retardá-lo com um atraso, chamado aqui de delay. Esta função irá interromper o funcionamento do programa por um determinado número de milissegundos. Um segundo é composto por 1000 milissegundos (ms), então, se o parâmetro for de 1000 (ms) o atraso será de um segundo.
