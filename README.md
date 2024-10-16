# Ponderada Programação - Módulo 4 - Semana 01

## Parte 1: Blink Led Interno

Este repositório contém a documentação para fazer o LED interno do Arduino piscar, utilizando a Arduino IDE.

### Requisitos para a realização da atividade
Antes de iniciar, certifique-se de que você possui:

- Arduino Uno
- Cabo USB para conectar o Arduino ao computador
- Arduino IDE instalada na sua máquina
- Led

## Passo-a-Passo

1. **Instalar a Arduino IDE**
Baixe e instale a Arduino IDE no seu computador clicando <a src = https://www.arduino.cc/en/software> aqui </a>
2. **Abra a IDE após a instalação.**
3. **Conectar o Arduino**
Conecte o Arduino Uno ao seu computador utilizando o cabo USB. O Arduino IDE deve reconhecer automaticamente o dispositivo.
4. **Seleção do modelo no IDE**
Selecione o modelo Arduino Uno em Ferramentas > Placa > Arduino Uno. Em seguida, selecione a porta correta em Ferramentas > Porta (normalmente aparece o nome do Arduino seguido da porta, por exemplo, COM3).

4. **Ação Blink** Selecionar o Exemplo "Blink"
Na Arduino IDE, vá até a aba Arquivo > Exemplos > 01.Basics > Blink.
O código do exemplo "Blink" aparecerá automaticamente na tela da IDE.
Esse código faz o LED embutido piscar, permanecendo aceso por um tempo determinado e depois apagando por um período, repetidamente.

4. **Upload** Fazer Upload do Código
Com o código já inserido, clique no botão Verificar (ícone de "check") para compilar.
Depois, clique no botão Carregar (ícone de seta) para enviar o código ao Arduino.
Se tudo estiver funcionando corretamente, o LED embutido no Arduino começará a piscar.

## Código de Piscar LED com Arduino

```cpp
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

## Fotos

<div align="center">
  <p><strong>Figura 1:</strong> Arduino conectado ao computador</p>
  <img src="assets/arduino_conectado_na_maquina.jpg" alt="Arduino conectado" />
  <p><em>Créditos: material produzido pelo autor (2024)</em></p>
</div>

<div align="center">
  <p><strong>Figura 2:</strong> IDE </p>
  <img src="assets/IDE.jpg" alt="Arduino conectado" />
  <p><em>Créditos: material produzido pelo autor (2024)</em></p>
</div>

<div align="center">
  <p><strong>Figura 3: Led aceso</strong> IDE </p>
  <img src="assets/led_aceso.jpg" alt="Arduino conectado" />
  <p><em>Créditos: material produzido pelo autor (2024)</em></p>
</div>

## Vídeo

Para acessar o vídeo do led piscando, clique <a src= "https://drive.google.com/file/d/1y30d7vNQkCkcW0dwd2n7T1avsZpiDvq-/view?usp=sharing"> aqui </a>

## Conclusão da parte 01
O projeto "Blink" permite demonstrar o funcionamento básico de controle do LED embutido no Arduino Uno. As imagens e o vídeo mostram o processo e o resultado final.