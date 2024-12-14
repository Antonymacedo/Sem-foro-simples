# Semáforo Simples

Um semáforo de transito simples.

**Materiais**

•Arduino Uno

•3 LEDs (vermelho,verde,amarelo)

•3 Resistores de 220Ω

![Opera Instantâneo_2024-12-13_211710_www tinkercad com](https://github.com/user-attachments/assets/1ff23012-2d76-4476-9ba6-2ed0fbe9e772)

# Esquema de Conexão:

Conecte os pinos digitais do Arduino 2,3,4 aos leds vermelho,amarelo e verde respectivamente.

# Código

```
#define RED_LED 2
#define YELLOW_LED 3
#define GREEN_LED 4

void setup() {
  pinMode(RED_LED, OUTPUT);
  pinMode(YELLOW_LED, OUTPUT);
  pinMode(GREEN_LED, OUTPUT);
}

void loop() {
  // Verde - Siga
  digitalWrite(GREEN_LED, HIGH);
  delay(5000); // 5 segundos
  digitalWrite(GREEN_LED, LOW);

  // Amarelo - Atenção
  digitalWrite(YELLOW_LED, HIGH);
  delay(2000); // 2 segundos
  digitalWrite(YELLOW_LED, LOW);

  // Vermelho - Pare
  digitalWrite(RED_LED, HIGH);
  delay(5000); // 5 segundos
  digitalWrite(RED_LED, LOW);
}

```

# Modelo no Tinkercad

https://www.tinkercad.com/things/cZcEvhYEfA7-semaforo-simples
