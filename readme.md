# Projeto Arduino - LED Control

Este repositório contém o projeto desenvolvido para o controle de LED utilizando Arduino.

## 📷 Screenshots

### 1. IDE com Código
Aqui está uma imagem da tela do meu IDE.

![IDE com Código](/assets/codigo.png)

### 2. Arduino Ligado ao Computador
Imagem demonstrando o Arduino conectado ao computador.

![Arduino Conectado](assets/cabo.jpeg)

### 3. LED Aceso
Imagem do LED sendo aceso com sucesso.

![LED Aceso](assets/led.jpeg)

## 🎥 Vídeo de Demonstração
Funcionamento completo do Arduino e do LED no vídeo a seguir.

[Link para o Vídeo](assets/video.mp4)

## 🛠️ Código

Código que utilizei para o controle do LED.

```cpp
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  
  delay(1000);                      
  digitalWrite(LED_BUILTIN, LOW);   
  delay(1000);                      
}
```

## 🚀 Como Executar

1. Conecte o Arduino ao computador.
2. Compile e faça o upload do código no IDE Arduino.
3. Verifique se o LED está acendendo e apagando conforme o código.

---

## Parte 2: Simulando Blink Externo

### Descrição

Nesta parte, realizei uma simulação no Tinkercad com um Arduino Uno e um protoboard, conectando um LED externo (OFF_BOARD) para criar um pisca-pisca controlado pelo Arduino. 

### Objetivo

- Simular o funcionamento de um LED externo controlado pelo Arduino, utilizando Tinkercad.
- Ao clicar no **play** no Tinkercad, o projeto deve executar corretamente, simulando o LED piscando com qualquer cadência.
- A montagem deve incluir:
  - Protoboard
  - Ligações elétricas
  - LED (OFF_BOARD)
  - Resistor
  - Arduino Uno

### 🛠️ Código para o Blink Externo

```cpp
int ledPin = 6; // Pino onde o LED está conectado

void setup() {
  pinMode(ledPin, OUTPUT); // Configura o pino 6 como saída
}

void loop() {
  digitalWrite(ledPin, HIGH); // Liga o LED
  delay(500);                 // Espera 500 milissegundos
  digitalWrite(ledPin, LOW);  // Desliga o LED
  delay(500);                 // Espera 500 milissegundos
}
```

### 🎥 Simulação no Tinkercad

[Tinkercad Simulação](https://www.tinkercad.com/things/f4UbGFhrSkU-pisca-pisca-ponderada?sharecode=SCBV4frkBzzoMGeRryf0DI8N6RjLT-6B1Zu8GtLbb-A)

### 📋 Instruções

1. Acesse o Tinkercad e monte o circuito com os componentes indicados.
2. Use o código acima para controlar o LED no pino 6.
3. Inicie a simulação e verifique o funcionamento do LED piscando.

