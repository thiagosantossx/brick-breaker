# 🧱 Brick Breaker

Um jogo simples de "quebra-blocos" desenvolvido com **Pygame**, onde você controla uma plataforma e rebate a bola para destruir todos os blocos.

## 🎮 Como jogar

- Use as **setas do teclado (← →)** para mover a plataforma para a esquerda ou direita.
- O objetivo é **destruir todos os blocos** sem deixar a bola cair.
- Se a bola tocar o fundo da tela, o jogo termina.

## 📦 Requisitos

Antes de rodar o jogo, instale o Pygame:

```bash
pip install pygame
```

## ▶️ Como executar

Clone este repositório e execute o arquivo Python:

```bash
git clone https://github.com/seu-usuario/brick-breaker.git
cd brick-breaker
python main.py
```

> 🧠 **Dica**: Verifique se o Python está instalado corretamente e que você está usando uma versão compatível com o Pygame (ex: Python 3.8+).

## 🛠️ Estrutura do Projeto

```
brick-breaker/

-----main.py         
-----README.md  
----images/images/brick-breaker0.png	
----images/images/brick-breaker1.png
	
```


## ✨ Funcionalidades

- Movimento suave do jogador
- Detecção de colisão com blocos e jogador
- Contador de pontuação
- Final de jogo quando todos os blocos são destruídos ou a bola cai
- Código simples e comentado, ideal para iniciantes

## 🚧 Melhorias futuras (ideias)

- Adicionar sons e música de fundo
- Vidas extras
- Níveis com dificuldades diferentes
- Power-ups (aumentar plataforma, bola dupla, etc.)

## 📸 Capturas de Tela

> _Você pode adicionar imagens aqui, como por exemplo:_
> ![Tela Inicio](images/brick-breaker0.png
>  [Tela com pontuação](images/brick-breaker1.png)



---
ste é um jogo estilo *Brick Breaker* desenvolvido com a biblioteca `pygame` em Python.

## 🎮 Desenvolvimento do Jogo - Passo a Passo

### 🛠️ 1. Preparação do Ambiente
- Instalei a biblioteca `pygame` usando o comando:
  ```bash
  pip install pygame
  ```
- Inicializei o Pygame com `pygame.init()` e criei a tela do jogo com o tamanho de `800x800`.

### 🎮 2. Estrutura da Tela
- Defini o título da janela com `pygame.display.set_caption('Brick Breaker')`.
- Criei os principais objetos do jogo usando `pygame.Rect()`:
  - A **bola**: um quadrado branco que se move na tela.
  - O **jogador**: uma barra azul na parte inferior da tela que o jogador controla.
  - Os **blocos**: vários blocos verdes posicionados no topo da tela.

### 🧱 3. Geração de Blocos
- Usei uma função `criar_blocos()` para gerar automaticamente os blocos com base em:
  - Quantidade por linha
  - Quantidade de linhas
  - Distâncias entre eles
- Os blocos são armazenados em uma lista e desenhados com `pygame.draw.rect()`.

### 🕹️ 4. Controle do Jogador
- Criei a função `movimentar_jogador()` que verifica se as teclas de seta esquerda/direita foram pressionadas e move a barra azul de acordo.

### ⚽ 5. Movimento da Bola
- Desenvolvi a função `movimentar_bola()` que atualiza a posição da bola com base em sua direção.
- Implementei colisões:
  - Com as bordas da tela (rebatendo)
  - Com o jogador (rebatendo)
  - Com os blocos (remoção e mudança de direção)

### 🧠 6. Lógica de Pontuação
- Cada bloco destruído aumenta a pontuação.
- Usei a função `atualizar_pontuacao()` para desenhar o texto da pontuação na tela e verificar se todos os blocos foram destruídos.

### 🔁 7. Loop Principal do Jogo
- Criei um loop `while not fim_jogo:` que:
  - Atualiza a tela com `tela.fill()` e `pygame.display.flip()`
  - Desenha o jogador, bola e blocos
  - Verifica eventos como pressionamento de teclas e encerramento do jogo
  - Atualiza a movimentação da bola e do jogador

### ✅ 8. Finalização
- Quando a bola cai (sai da tela inferior), o jogo é encerrado.
- O `pygame.quit()` é chamado para fechar a janela do jogo corretamente.


Feito com 💙 usando [Pygame]
