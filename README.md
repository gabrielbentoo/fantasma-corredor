# 👻 Jogo do Fantasma na Torre

Este projeto é um jogo 2D desenvolvido em **JavaScript** utilizando a biblioteca **p5.js** juntamente com **p5.play**.  
O jogador controla um fantasma que sobe uma torre infinita, desviando de obstáculos e utilizando plataformas para não cair.

---

## 🎮 Objetivo do Jogo

Controlar o fantasma e sobreviver o maior tempo possível enquanto a torre se move para baixo.  
O jogo termina quando o fantasma cai da torre ou colide com um bloco invisível.

---

## 🕹️ Controles

- ⬅️ **Seta para a esquerda**: Move o fantasma para a esquerda  
- ➡️ **Seta para a direita**: Move o fantasma para a direita  
- ⬆️ **Barra de espaço**: Faz o fantasma pular  

---

## 🧠 Mecânicas do Jogo

- A torre se move continuamente para baixo, criando a ilusão de subida
- Portas e grades aparecem a cada **240 frames**
- As grades funcionam como plataformas
- Blocos invisíveis fazem o jogador perder ao encostar
- A gravidade afeta o fantasma constantemente
- O jogo possui dois estados:
  - `play`: jogo em execução
  - `end`: fim de jogo

---

## 🧱 Elementos do Jogo

### Sprites
- **Fantasma (ghost)**: Personagem controlado pelo jogador
- **Torre (tower)**: Fundo em movimento
- **Portas (door)**: Obstáculos visuais
- **Grades (climber)**: Plataformas
- **Blocos invisíveis**: Causam o fim do jogo ao serem tocados

### Grupos
- `doorsGroup`: Grupo das portas
- `climbersGroup`: Grupo das grades
- `invisibleBlockGroup`: Grupo dos blocos invisíveis

---

## 🔊 Sons e Imagens

### Imagens Utilizadas
- `tower.png`
- `door.png`
- `climber.png`
- `ghost-standing.png`

### Som
- `spooky.wav` (som ambiente em loop durante o jogo)

---

## ⚙️ Funções Principais

### `preload()`
Carrega todas as imagens e sons do jogo.

### `setup()`
Cria a tela, sprites iniciais e grupos.

### `draw()`
Controla a lógica principal do jogo, movimentação, colisões e estados.

### `spawnDoors()`
Gera portas, grades e blocos invisíveis periodicamente com posições aleatórias.

---

## ❌ Condições de Fim de Jogo

O jogo termina quando:
- O fantasma toca um bloco invisível  
- O fantasma cai abaixo da tela (posição Y > 600)

Ao final, é exibida a mensagem **"Fim de jogo"** e o som é interrompido.

---

## 📦 Requisitos para Executar

- Navegador moderno (Chrome, Edge, Firefox)
- Bibliotecas:
  - `p5.js`
  - `p5.play.js`
- Arquivos de imagem e som na mesma pasta do código

---

## 🚀 Possíveis Melhorias

- Adicionar sistema de pontuação
- Corrigir reinício do som (play em loop contínuo)
- Tela de reinício do jogo
- Animação do fantasma
- Aumentar progressivamente a dificuldade

---

## 🧑‍💻 Autor

Projeto desenvolvido para fins educacionais utilizando **JavaScript + p5.js**.

---

👻 **Divirta-se explorando a torre assombrada!**
