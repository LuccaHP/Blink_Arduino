### Parte 1 - Blink Led Interno
Instale a Arduino IDE em seu computador e assista aos vídeos indicados nos autoestudos conforme o roteiro descrito anteriormente. Você deverá realizar o "blink" com esse LED Interno e postar em seu GitHub as evidências dessa realização.

Você vai fazer o led ficar aceso por um tempo X, apagar e aguardar Y segundos e depois voltar a acender, propondo um loop que gera uma "luz piscando".

## Vídeo de demonstração

[Assita o Vídeo de demonstração](./Blink_Video.mp4)

## Código

```int ledPin = 13; // LED interno no pino 13 para a maioria das placas
int tempoAceso = 1000;  // Tempo que o LED ficará aceso (em milissegundos)
int tempoApagado = 500; // Tempo que o LED ficará apagado (em milissegundos)

void setup() {
  pinMode(ledPin, OUTPUT); // Configura o pino como saída
}

void loop() {
  digitalWrite(ledPin, HIGH);  // Liga o LED
  delay(tempoAceso);           // Aguarda tempo aceso
  digitalWrite(ledPin, LOW);   // Desliga o LED
  delay(tempoApagado);         // Aguarda tempo apagado
}
```