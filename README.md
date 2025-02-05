# Temporizador Periódico - Semáforo com Raspberry Pi Pico W

## Descrição do Projeto

Esse é um projeto feito em C para simular um semaforo, usando o Wokwi para emular a placa Raspberry Pi Pico W.

## Componentes Utilizados

- **Microcontrolador**: Raspberry Pi Pico W
- **LEDs**: Vermelho, Amarelo e Verde
- **Resistores**: 3x de 330 Ω

## Funcionamento

1. O sistema inicia com o LED **vermelho** ligado.
2. Após **3 segundos**, o LED muda para **amarelo**.
3. Após mais **3 segundos**, o LED muda para **verde**.
4. Após mais **3 segundos**, o LED retorna para **vermelho** e o ciclo se repete.
5. Durante a execução, a cada segundo (1.000ms), uma mensagem é enviada pela porta serial.

## Regras de Operação

- O ciclo do semáforo é controlado por um **callback do temporizador**.
- A execução principal imprime mensagens na **porta serial** a cada segundo.

### Simulação no Wokwi

Caso deseje testar a simulação no Wokwi, siga os seguintes passos:

1. Acesse o [Wokwi](https://wokwi.com/)
2. Crie um novo projeto com o Raspberry Pi Pico
3. Configure os LEDs conforme a descrição acima
4. Carregue o código para testar a funcionalidade
