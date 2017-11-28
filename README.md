# SeguidorDeLinha
#inicio 07/11


---------------------------Relatorio-------------------------

RELATÓRIO 
DE 
PRINCIPIO DE CONTROLE





Alunos: 
Andrei Moliterno 1420354/X
Erico Rocha 	 1324406/5





Introdução

Nosso projeto tem como objetivo fazer um carro conseguir controlar suas rodas com utilização de sensores e um microcontrolador, sabendo quando o mesmo deve parar uma das rodas para fazer uma curva ou quando quiser ir reto deixando as duas rodas em velocidade constante. 
Para fazer isso utilizaremos um carro que com o módulo seguidor de linha, utilizaremos 3 sensores para detectamos as linhas , terá um sensor na frente, um que estará mais a esquerda e outro que estará mais a direita,  os sensores quando identificarem uma linha, enviaram  para o arduino o valor digital um e quando não encontrar nenhuma linha e o valor digital zero.Dessa forma o arduino consegue de acordo com o que o sensor manda, controlar os servo motores, que os mesmos que estarão conectado as rodas do carro, vão controlar se mantém elas girando ou deixam elas paradas.




Componentes:

Módulo Seguidor de Linha Infravermelho 4 Canais:
O Módulo Seguidor de Linha Infravermelho 4 Canais é baseado em quatro sensores seguidores de linha, o seu diferencial está no fato dele otimizar o projeto, uma vez que o caminho pode ser ao mesmo tempo monitorado em quatro trechos distintos, facilitando dessa forma a estratégia adotada. Cada sensor é independente e possui um trimpot de ajuste de luminosidade de detecção.
O Módulo Seguidor de Linha Infravermelho 4 Canais é compatível com Arduino, Pic, Arm, Raspberry Pi entre outros.

- Especificações:
- Tensão de alimentação: 3.3V - 5V;
- Consumo de Corrente: 1A;
- Temperatura de Operação: -10°C ~ +50°C;
- Distância de detecção: 1mm ~ 60cm (Ajustável);
- Sinal de saída: TTL (Pode ser conectado direto ao microcontrolador);
- Tipo de saída: Nível lógico baixo (0) quando obstáculo detectado, nível lógico alto (1) quando sem obstáculo;
- LED: LED indica quando o sensor foi ativado (Obstáculo detectado);
- Comprimento do jumper: 20cm;
- Dimensões do módulo: 44x40x09mm.

Kit Chassi 2WD
O Kit Chassi 2WD foi desenvolvido com a finalidade de prover ao maker interessado em robótica educacional, uma ferramenta de montagem de um carrinho para aplicações em robótica. O Kit Chassi 2WD é composto pela estrutura fabricada em acrílico, motores com caixa de redução(1:48), rodas com pneu, roda boba, suporte para pilhas e peças de montagem do chassi. O Kit Chassi 2WDpode ser utilizado na construção de um robô seguidor de linha, robô de combate, robô que desvia de obstáculos. Para o controle do Kit Chassi 2WD, podem ser utilizadas diversas placas microcontroladas, Arduino, Raspberry Pi, Beaglebone Black, Orange Pi entre outras.

- Composição:
01 - Chassi em acrílico;
02 - Motores DC (3~6v);
02 - Rodas de Borracha;
01 - Roda Boba;
02 - Discos de Encoder;
01 - Suporte para 4 Pilhas;
01 - Jogo de Parafusos.


Arduino UNO:
A placa pode ser alimentada pela conexão USB ou por uma fonte de alimentação externa, conforme exibido na figura abaixo:
SeguidorDeLinha/arduino.png
Arduino é uma plataforma de computação open-source baseado em uma simples placa com entradas e saídas tanto digitais como analógicas. Possui um próprio ambiente de desenvolvimento que implementa a Linguagem C. O Arduino pode ser usado para desenvolver objetos interativos autônomos ou pode ser conectado a um software em seu computador (ex. Flash, Processing, MaxMSP). O Ambiente de desevolvimento(IDE) open-souce pode ser obtido gratuitamente (atualmente disponível para Mac OS X, Windows, e Linux).
Este é o Arduino Uno R3. É uma placa com microcontrolador Atmega328 (datasheet). Possui 14 entradas/saídas digitais (das quais 6 podem ser usadas como saídas PWM), 6 entradas analógicas, um cristal oscilador de 16MHz, conexão USB, uma entrada para fonte, soquetes para ICSP, e um botão de reset. A placa contém todo o necessário para usar o microcontrolador. Simplesmente conecte-a a um computador com o cabo USB - AB (não acompanha - deve ser comprado separadamente) ou ligue a placa com uma fonte AC-DC(ou bateria). O Uno seleciona automáticamente a fonte de alimentação (USB ou fonte externa). Esta placa já vem pronta e testada com o microcontrolador ATMega328 pré-carregado com "bootloader"
A placa Uno se diferencia das outras por não utilizar o chip da FTDI USB-to-Serial. Ao invés deste chip, um Atmega8U2 já programado faz a função de converter os dados da USB para Serial.

https://github.com/EricoDRocha/SeguidorDeLinha/blob/master/arduino.png?raw=true

- Especificações:
- Microcontrolador: ATMEGA328P-PU
- Tensão de Operação: 5V
- Tensão de Entrada: 7~12V
- Portas Digitais: 14(6 tem função PWM)
- Corrente Pinos de I/O: 40mA
- Corrente Pinos 3.3V: 50ma
- Memória Flash: 32Kb
- SRAM: 2Kb
- EEPROM: 1Kb
- Velocidade Clock: 16Mhz


Servo TowerPro MG995 Metálico
O Servo Motor TowerPro MG995 é um servo motor de alto torque de 13kg/cm a 4.8V e 15kg/cm a 6V,  sua rotação pode chegar a  180 graus, por essas características, ele é muito utilizado em projetos de robótica.
Esse modelo pode ser utilizado com as principais plataformas microcontroladas do mercado, seja ela, pic, arduino, arm entre outros. As conexões do servo motor MG995 segue o padrão dos principais fabricantes do mercado, são elas: Hitec, GWR, Futaba, Cirrus entre outros

- Especificações:
- Modelo: TowerPro MG995;
- Tensão de operação: 4,8-7,2V;
- Tipo de Engrenagem: Metálica;
- Modulação: Analógica;
- Velocidade de operação: 0,17seg/60graus (4,8V sem carga);
- Velocidade de operação: 0,13seg/60graus (6,0V sem carga);
- Torque: 13 kg.cm (4,8V) e 15 kg.cm (6,0V);
- Faixa de Rotação: 180°;
- Tamanho cabo: 300mm;
- Dimensões: 40 x 19 x 43mm



Protoboard
É constituída por uma base plástica, contendo inúmeros orifícios destinados à inserção de terminais de componentes eletrônicos. Internamente existem ligações determinadas que interconectam os orifícios, permitindo a montagem de circuitos eletrônicos sem a utilização de solda.
Explicação Técnica do funcionamento:
Os Servo motores irão fazer girar as rodas(a roda direita e esquerda) dentro do loop fazendo o carro andar em linha reta pois as duas rodas vão estar na mesma velocidade constante. Quando um sensor detecta a linha, o arduino manda um comando para o motor do lado que o sensor detectou a linha fazendo o mesmo parar, assim somente o do outro lado vai girar fazendo ele desviar da linha e continua dessa forma. Conforme a imagem mostra.


OBS: Durante a montagem do carro, observando que as rodas não estavam com velocidade constante ou seja, uma delas estava girando mais rápido do que a outra, mesmo mandando o valor igual em módulo. A lógica abordada é bem simples, quando o sensor da direita mandar mandar o sinal identificando uma linha, irá parar a roda da direita e aumentar a velocidade da roda da esquerda, e visse versa, porém utilizamos uma variável de ajuste para tentar igualar a velocidade da roda, por isso na implementação não colocamos os mesmo nas rodas.


---------------------------------------
Logia de Funcionamento

Como o nosso sensor ele não consegue calcular um valor analogicamente (é apenas digital, zero ou 1) precisamos de uma fórmula para virtualizar.
if (dir+meio+esq>0)
 leitura = (150*dir + 100*meio +50*esq)/(dir+meio+esq);
  “dir” “meio” “esq” são as variáveis que recebem o que é lido  do sensor digital
Dessa forma conseguimos saber o quão perto da esquerda ou da direita ele se encontra.

Utiliziamos o erro para poder otimizar a acertividade do nosso carro.
erro_ant = erro;  -- Como o erro_ant é atualizado antes do erro, garantimos que o erro anterior é salvo antes de pegarmos o novo erro.
erro  = setpoint - leitura;                  
 DErro  = erro - erro_ant; -- variação do erro atual com o erro anterior.
Setpoint = constante que foi escolhida para caso não seja encontrado nada.
Para calcularmos o “P” precisamos do erro corrente multiplicada a uma constante KP

Primeiro passo do codigo   tempo_ant = tempo;
Depois da leitura é feito o cálculo do tempo novamente.  tempo = millis();
Depois é calculado o variação do 	Dtempo = tempo - tempo_ant;

Assim iremos utilizar o Dtempo no cálculo do Kd

Após ter a informação do erro e da variação do tempo, assim podemos calcular o KD;
kd = erro/Dtempo; -- Kd representa a variação do erro ao longo do tempo

Função  para Calcular o valor de “i” com a constante  “Ki” afim de calibrar o resultado
double calc_i(int erro, double tempo, double i){
 i += i + (DErro* tempo)*ki;   return i;   }

Chamado dentro do codigo após ter o valor do DT e do erro.
i = calc_i(erro, Dtempo,i)

Obs: Criamos um metodo para calcular o I afim de deixar o código mais legível, passando o valor I(pois ele é um acumulativo), o erro encontrado e a variação do tempo.

Utilizamos técnica tentativa e erro, os valores de melhor resultado foram;

Kp = 0.5
Kd = 0.1
Ki = 0.1 

Quanto mais aumentamos o valor principalmente do Kd e Ki o tempo de resposta do carro ou era rápido  demais para efetuar a ação ou ele se perdia e não adiantava o valor lido pelo sensor.



Codigo de impementação

---------------------------------------
int   dir;
float meio; 
float esq;   
int Ajust1;  
int Ajust2; 

 // variaveis erro
 int DErro;
 int erro_ant;
 int erro;

 //variaveis tempo
 double tempo;
 double tempo_ant;
 double Dtempo;

//Variaveis de controle
 int leitura;
 int setpoint;
double i;
//Saida total
 double output;


 //constantes 
  int kp;
  int p;
  int kd;
  int ki;


Servo mot_esquerdo,mot_direito;


double calc_i(int erro, double tempo, double i){
  i += i + (DErro* tempo)*ki;
  return i;
  }


void setup() {

 dir        = 0; 
 meio       = 0; 
 esq        = 0; 
 Ajust1     = 10; 
 Ajust2     = 10;
 DErro      = 0;
 erro_ant   = 0;
 erro       = 0;
 tempo      = 0.0;
 tempo_ant  = 0.0;
 Dtempo     = 0.0;
 leitura    = 0;
 setpoint   = 100;
 output     = 0.00;
 i          = 0.0;
 mot_esquerdo.attach(8); 
 mot_direito.attach(9);

 
 kp         = 0.5;
 p          = 0;
 kd         = 0.01;
 ki         = 0.1;
 
}

void loop() {
  //pegando o tempo
  tempo_ant = tempo;

  //  tempo = millis();

   //variaveis de leitura
  int dir   =  digitalRead(3);
  int meio  = digitalRead(2); 
  int esq   = digitalRead(1); 


// atrelando DErroanterior
   erro_ant = erro;

// calculanto leitura
  if (dir+meio+esq>0){
    leitura = (150*dir + 100*meio +50*esq)/(dir+meio+esq);
  }

  // associando novo erro
    erro  = setpoint - leitura;
    DErro  = erro - erro_ant;
  
  //calculando P
    p = erro * kp;
  
    tempo = millis();

  //Calculo do Dtempo
      Dtempo = tempo - tempo_ant;

   //chamando metodo calcular i
      i = calc_i(erro, Dtempo,i);

    //Calculo do Kd
    kd = erro/Dtempo;

    //calculando a saida
      output = p + i + kd;

// rodando as rodas
mot_esquerdo.write(90 + (output+ Ajust1)); 
mot_direito.write(90 - (output+Ajust2));


}

---------------------------------------

Codigo de impementação


		Conclusão

Foi encontrado algumas dificuldades no trabalho, o fato do sensor não está muito perto da linha, causando um sinal não muito preciso. Um aumento na quantidade de sensores poderia dar mais precisão, como as rodas são soldadas manualmente, causou o problema de uma roda não girar com mesma velocidade que a outra.

Tivemos um problema na montagem que o VCC estava causando interferência no sensor digital, que as vezes nos fazia achar que a logica estava errada, pois não estavamos entendendo o comportamento do carro.

Como utilizamos o servor motor e eles so vão de 0 (rodando para um lado ao máximo de velocidade) 90 (parado) até 180(rodando para outro lado ao máximo de velocidade) e como utilizamos variaveis para controlar o valor de saida final, que chamamos de "Output" que estaria entre 0 e 180, se esses valores ou ficassem menor que zero ou maior que 180 ele pagava um valor completamente aleatório.


bibliografia :
https://www.filipeflop.com/blog/projeto-robo-seguidor-de-linha-arduino/
https://www.autocorerobotica.com.br
https://www.robocore.net
 
![Alt Text](https://github.com/EricoDRocha/SeguidorDeLinha/raw/master/path/to/arduino.png)



(https://github.com/EricoDRocha/SeguidorDeLinha/blob/master/arduino.png)
