# Projeto Final: Jogo de Naves

## Descrição do Projeto

Este projeto utiliza a biblioteca de Threads no espaço de usuário, desenvolvida durante o semestre, para implementar um jogo inspirado nos antigos "vídeo games de mão" de naves.

### Descrição do Jogo

O jogo consiste em uma nave controlada pelo jogador, que inicialmente está posicionada no centro da tela. A nave do jogador pode atirar e acertar naves inimigas que se movem e atiram de forma aleatória. No máximo, quatro naves inimigas existem simultaneamente. Essas naves giram e atiram de maneira aleatória.

A nave do jogador possui três vidas. Cada vez que a nave do jogador é atingida por um tiro inimigo, ela perde uma vida. Se o jogador acertar uma nave inimiga, ganha 100 pontos. As naves inimigas que são atingidas desaparecem e reaparecem após 2 segundos. As naves inimigas e a nave do jogador não podem se tocar, e se os tiros de ambas se encontrarem, eles se cancelam e desaparecem.

Para adicionar desafio, o movimento das naves inimigas segue dois algoritmos diferentes, com duas naves usando um algoritmo e as outras duas naves usando outro. Após a nave do jogador destruir quatro naves inimigas, a velocidade das naves inimigas aumenta para o nível 2. Este processo se repete até alcançar o nível 3 de velocidade. A velocidade atual (1, 2 ou 3) e a pontuação (score) são exibidas à direita da tela.

A implementação do jogo utiliza a biblioteca de Threads desenvolvida ao longo do semestre. Cada nave inimiga é uma thread separada, assim como a nave do jogador. Além disso, há uma thread responsável pelo desenho da tela e outra para o tratamento da entrada do teclado, totalizando um mínimo de sete threads. Há liberdade para criar threads adicionais conforme necessário.

![Screenshot from 2024-06-06 16-46-20](https://github.com/vvc-git/UFSC/assets/78426009/ca07e417-79c5-405b-a72d-65a6eb5a2552)

## Instalação

### Dependências

A biblioteca gráfica utilizada é a SFML. Para instalá-la no Ubuntu, execute:
```bash
sudo apt-get install libsfml-dev
```

A documentação da biblioteca SFML pode ser encontrada [aqui](https://www.sfml-dev.org/learn.php).

## Estrutura do Código

O projeto está organizado da seguinte forma:

- `main.cpp`: Arquivo principal que inicializa o jogo.
- `Player.cpp` e `Player.h`: Implementação da nave do jogador.
- `Enemy.cpp` e `Enemy.h`: Implementação das naves inimigas.
- `Bullet.cpp` e `Bullet.h`: Implementação dos tiros.
- `Game.cpp` e `Game.h`: Controle principal do jogo, incluindo lógica de pontuação e níveis.
- `Graphics.cpp` e `Graphics.h`: Desenho da tela utilizando SFML.
- `Input.cpp` e `Input.h`: Tratamento da entrada do teclado.

## Como Executar

Após instalar as dependências, compile o projeto com o seguinte comando:
```bash
make main
```
![Screenshot from 2024-06-06 16-16-52](https://github.com/vvc-git/UFSC/assets/78426009/ab9b09a5-b53d-4dcb-b02d-bab808ed9372)
![Screenshot from 2024-06-06 16-16-37](https://github.com/vvc-git/UFSC/assets/78426009/472cd3c8-9cb5-4b9f-a463-e1b764657f55)

# Final Project: Spaceship Game

## Project Description

This project uses the user-space Threads library, developed during the semester, to implement a game inspired by old handheld video games featuring spaceships.

### Game Description

The game consists of a spaceship controlled by the player, initially positioned at the center of the screen. The player's spaceship can shoot and hit enemy spaceships that move and shoot randomly. A maximum of four enemy spaceships exist simultaneously. These spaceships rotate and shoot randomly.

The player's spaceship has three lives. Each time it is hit by an enemy shot, it loses one life. If the player hits an enemy spaceship, they gain 100 points. Hit enemy spaceships disappear and reappear after 2 seconds. The enemy spaceships and the player's spaceship cannot touch each other, and if their shots collide, they cancel each other out and disappear.

To add challenge, the movement of enemy spaceships follows two different algorithms, with two spaceships using one algorithm and the other two using another. After the player destroys four enemy spaceships, the enemy spaceships' speed increases to level 2. This process repeats until it reaches speed level 3. The current speed level (1, 2, or 3) and the score are displayed on the right side of the screen.

The implementation of the game uses the Threads library developed throughout the semester. Each enemy spaceship is a separate thread, as is the player's spaceship. Additionally, there is a thread responsible for drawing the screen and another for handling keyboard input, totaling a minimum of seven threads. There is freedom to create additional threads as needed.

![Screenshot from 2024-06-06 16-46-20](https://github.com/vvc-git/UFSC/assets/78426009/ca07e417-79c5-405b-a72d-65a6eb5a2552)

## Installation

### Dependencies

The graphical library used is SFML. To install it on Ubuntu, run:
```bash
sudo apt-get install libsfml-dev
```

The documentation for the SFML library can be found [here](https://www.sfml-dev.org/learn.php).

## Code Structure

The project is organized as follows:

- `main.cpp`: Main file that initializes the game.
- `Player.cpp` and `Player.h`: Implementation of the player's spaceship.
- `Enemy.cpp` and `Enemy.h`: Implementation of the enemy spaceships.
- `Bullet.cpp` and `Bullet.h`: Implementation of the bullets.
- `Game.cpp` and `Game.h`: Main game control, including scoring and levels logic.
- `Graphics.cpp` and `Graphics.h`: Screen rendering using SFML.
- `Input.cpp` and `Input.h`: Keyboard input handling.

## How to Run

After installing the dependencies, compile the project with the following command:
```bash
make main
```
![Screenshot from 2024-06-06 16-16-52](https://github.com/vvc-git/UFSC/assets/78426009/ab9b09a5-b53d-4dcb-b02d-bab808ed9372)
![Screenshot from 2024-06-06 16-16-37](https://github.com/vvc-git/UFSC/assets/78426009/472cd3c8-9cb5-4b9f-a463-e1b764657f55)


