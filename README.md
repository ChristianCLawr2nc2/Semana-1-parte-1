# Parte 1 da ponderada da Semana 1

## Introdução

  A atividade foi dividida em duas partes complementares: o controle do LED interno da placa e o controle de um LED externo conectado a uma protoboard.

  Na Parte 1, foi realizado o clássico projeto “Blink”, em que o LED interno (conectado ao pino 13 do Arduino) é programado para piscar em intervalos definidos. Essa etapa permite compreender o funcionamento básico das funções setup() e loop(), além do uso dos comandos pinMode(), digitalWrite() e delay() para controlar saídas digitais.

## Blink do LED Interno do Arduino

#### Código de Funcionamento do Arduino:

```C++
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);
  delay(800);
  digitalWrite(13, LOW);
  delay(700);
}

```

---
<br>

![Código no IDE](/assets/IDEPrintScreen.png)

<br>

---

<br>

![Arduino Funcionando](/assets/ArduinoLEDON.jpg)

---

# Parte 2 da ponderada da Semana 1

## Introdução

    Na Parte 2, o mesmo princípio foi aplicado a um LED externo, utilizando componentes físicos como resistores, jumpers e protoboard, simulando o circuito no Tinkercad antes da montagem prática. Essa parte reforça o entendimento sobre conexões elétricas, polaridade de componentes e controle de dispositivos externos por meio de portas digitais do Arduino.

## Blink do LED externo usando Arduino

### Imagem do Protótipo feito no Tinkercad

![Protótipo do Tinkercad](/assets/TinkercadON.png)

----

# Passo a Passo

#### 1.

  **Adicionar o Arduino Uno.**

#### 2.

  **Adicionar a ProtoBoard.**

#### 3.

  **Colocar um fio/Jumper que ligue o polo negativo da ProtoBoard a Porta GND/Ground.**

#### 4.

  **Colocar um fio/Jumper que ligue o polo positivo da ProtoBoard à porta 10 do Arduino.**

#### 5.

  **Colocar um Resistor que passe a tensão desejada para o LED na placa metálica central.(funciona como um Jumper)**

#### 6.

  **Colocar um fio/Jumper que funcione como um fio terra para o LED ou como simplesmente o polo negativo.**

#### 7.

  **Colocar o LED na posição correta para que ele pisque como desejado.**

#### 8.

  **Abrir a aba para inserir o código e coloque o seguinte código onde o LED fica ligado por 10000ms e desligado por 1000ms:**
```C++
  // C++ code
  //
  void setup()
  {
    pinMode(10, OUTPUT);
  }

  void loop()
  {
    digitalWrite(10, HIGH);
    delay(10000);// Wait for 1000 millisecond(s)
    digitalWrite(10, LOW);
    delay(1000); // Wait for 1000 millisecond(s)
  }
```

#### 9.

  **Conectar o Arduino e testar o código e seu funcionamento.**

  Link do Protótipo do Tinkercad:
  ---
  **https://www.tinkercad.com/things/9aPOYJp2bUI/editel?returnTo=%2Fdashboard**