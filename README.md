# Simulação de Pêndulo

Este programa em Rust simula o movimento de dois pêndulos usando a biblioteca `speedy2d`. Cada pêndulo consiste em uma haste presa a um ponto de pivô, com um peso (bob) na extremidade. O movimento dos pêndulos é governado por equações físicas, e suas posições são atualizadas e desenhadas na janela.

## Dependências
- [speedy2d](https://crates.io/crates/speedy2d): Uma biblioteca de gráficos 2D simples e fácil de usar para Rust.

## Uso
1. Certifique-se de ter o Rust instalado. Se não tiver, você pode baixá-lo [aqui](https://www.rust-lang.org/tools/install).
2. Clone este repositório.
3. Navegue até o diretório contendo este arquivo `main.rs`.
4. Compile e execute o programa usando o seguinte comando:
    ```
    cargo run
    ```
5. Assista à simulação de dois pêndulos balançando na janela.

## Detalhes de Implementação
- `main.rs` contém a lógica principal do programa. Ele inicializa uma janela e executa o loop de eventos.
- A estrutura `MyWindowHandler` implementa o traço `WindowHandler` fornecido pelo `speedy2d`. Ela lida com o desenho na janela.
- A estrutura `Pendulum` representa um único pêndulo. Ela armazena propriedades como origem, posição, ângulo, velocidade angular, aceleração angular, comprimento da haste, massa e gravidade.
- O método `update()` na estrutura `Pendulum` atualiza a posição do pêndulo com base em seu estado atual.
- O método `draw()` na estrutura `Pendulum` desenha o pêndulo na janela usando primitivas gráficas.
- O módulo `vector` contém uma estrutura simples `Vector` usada para cálculos de posição.

## Créditos
Este programa foi digitado a partir do tutorial do YT -> Manual do Código [linkYT](https://www.youtube.com/watch?v=U-X51GsTAzA)
