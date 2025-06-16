# FlappyPi
Projeto universitário para demonstração de conceitos matemáticos utilizados como fundamentos para o jogo e para elucidamentos e aprendizados dinâmicos sobre esses conceitos.

## Visão Geral

**π Flappy Enhanced** é uma releitura interativa e educativa do clássico Flappy Bird, que combina mecânicas de jogo com conceitos matemáticos. Nesta versão, o jogador controla um personagem representado pelo símbolo π, enfrentando obstáculos enquanto a física do jogo é governada por funções matemáticas escolhidas pelo próprio jogador.

---

## Principais Diferenças em Relação ao Flappy Bird Tradicional

| Aspecto                    | Flappy Bird Original | π Flappy Enhanced                                                   |
| -------------------------- | -------------------- | ------------------------------------------------------------------- |
| Gravidade e pulo           | Fixos e constantes   | Variáveis, moduladas por funções matemáticas                        |
| Obstáculos                 | Canos retangulares   | Obstáculos em forma de parábolas                                    |
| Personalização da física   | Não existe           | Escolha de função (linear, quadrática, etc.) e parâmetro "a"        |
| Feedback visual matemático | Nenhum               | Grade cartesiana, trilha da trajetória e gráfico da função ao final |
| Enfoque educativo          | Ausente              | Forte, com foco em visualização de funções e seus efeitos           |

---

## Conceitos Matemáticos Utilizados

### 1. Funções Matemáticas Parametrizadas

* **Tipos de Função Disponíveis:**

  * Linear
  * Quadrática
  * Polinomial (cúbica)
  * Exponencial
  * Logarítmica
* **Aplicação:** O jogador escolhe uma dessas funções para determinar como a gravidade e o impulso de salto vão variar ao longo do tempo.
* **Por quê?** Permite ao jogador sentir na prática como diferentes tipos de funções influenciam o comportamento de um sistema dinâmico.

### 2. Transformações de Funções

* **Escala e Parâmetro "a":** Multiplicação de cada função por um parâmetro ajustável para controlar sua intensidade.
* **Objetivo:** Demonstrar como o ajuste de parâmetros afeta o gráfico e a resposta física no jogo (exemplo: maior "a" = pulo mais forte ou gravidade mais intensa).

### 3. Dinâmica Discreta (Integração Numérica)

* **Modelo:** Método de Euler discreto para atualização de posição e velocidade.
* **Fórmula:**

  ```
  velocity += currentGravity;
  y += velocity;
  ```
* **Por quê?** Representa uma simulação simplificada de movimento sob a ação de forças, facilmente visualizável no gameplay.

### 4. Obstáculos Parabólicos

* **Geometria:** Obstáculos são seções de parábolas (funções quadráticas).
* **Objetivo:** Adicionar variedade geométrica e desafiar o jogador com formas de gap que não são retangulares.

### 5. Coordenadas Cartesiana e Visualização de Trajetória

* **Grade de Fundo:** Plano cartesiano com eixos x e y.
* **Trilha de Movimento:** O deslocamento de π é mostrado com uma sequência de pontos conectados, formando um gráfico da trajetória.

### 6. Visualização Gráfica da Função

* **Após o Game Over:** Exibe um gráfico da função escolhida, reforçando a ligação entre teoria matemática e efeito prático na jogabilidade.

---

## Tecnologias Utilizadas

* **HTML5:** Estrutura básica do jogo.
* **CSS3:** Estilização do layout, cores, animações de interface e responsividade.
* **JavaScript (Vanilla JS):**

  * Lógica de física e movimentação.
  * Manipulação do Canvas para renderização dos gráficos.
  * Gerenciamento de estados do jogo (início, execução, game over).
  * Interface de usuário (seleção de função, exibição de pontuação, etc).
* **Canvas API:**

  * Desenho da grade, obstáculos, trajetória e gráficos de funções.

---

## Objetivo Educacional

Este projeto busca transformar um conceito simples de jogo em uma ferramenta de aprendizagem matemática intuitiva e divertida. O jogador experimenta em tempo real os efeitos de diferentes tipos de funções matemáticas na física do jogo, desenvolvendo uma compreensão mais sensorial de conceitos como:

* Variação de parâmetros
* Curvas de crescimento
* Trajetórias físicas
* Relação entre funções teóricas e resultados práticos

Ideal para uso em aulas de matemática, feiras de ciências ou como projeto de demonstração de aplicações interativas de matemática na programação.

---

## Como Jogar

1. Escolha uma função matemática e ajuste o parâmetro "a".
2. Pressione **Start Game**.
3. Use a **barra de espaço** ou **clique na tela** para fazer π saltar.
4. Tente passar pelo máximo de obstáculos parabólicos.
5. Após o fim, analise seu desempenho e veja o gráfico da função utilizada.

---

Divirta-se explorando matemática de forma interativa!

