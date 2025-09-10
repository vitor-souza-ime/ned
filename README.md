# Controle do Robô Ned no Webots

Este repositório contém um programa em C para controlar o robô **Ned** utilizando o simulador **Webots**. O programa permite movimentar as juntas do braço, abrir/fechar a garra e executar demonstrações e sequências de pick and place através do teclado.

## Requisitos

- [Webots](https://cyberbotics.com) (versão compatível com seu sistema)
- Compilador C (ex.: GCC)
- Sistema operacional compatível com Webots

## Estrutura do Código

O arquivo principal é `main.c`, que implementa:

- Inicialização do robô (`wb_robot_init`)
- Controle das juntas e garra (`wb_motor_set_position` e `wb_motor_set_velocity`)
- Interface de teclado para movimentação das juntas e execução de comandos
- Funções de demonstração (`D`) e pick and place (`P`)
- Funções utilitárias de espera passiva e exibição de comandos

### Comandos do Teclado

| Tecla | Ação |
|-------|-----|
| A / Z | Movimenta a junta 1 |
| Q / S | Movimenta a junta 2 |
| W / X | Movimenta a junta 3 |
| Y / U | Movimenta a junta 4 |
| H / J | Movimenta a junta 5 |
| B / N | Movimenta a junta 6 |
| L / M | Abre / Fecha a garra |
| D     | Executa demonstração automática |
| P     | Executa sequência de pick and place |

## Como Compilar e Executar

1. Abra o **Webots**.
2. Adicione o arquivo `main.c` ao seu projeto de robô.
3. Compile o código utilizando o compilador C do Webots.
4. Execute a simulação.
5. Use o teclado para controlar o robô conforme os comandos acima.

## Licença

Este projeto segue a **Apache License 2.0**, conforme indicado nos arquivos de origem.


