# 🎮 Roadmap Completo de Criação de Jogos
> Programação • Game Design • Escrita de Histórias

---

## 🧠 Sumário
- [🔧 Programação de Jogos](#-programação-de-jogos)
- [🎨 Game Design](#-game-design)
- [✍️ Escrita de Histórias / Narrativa](#-escrita-de-histórias--narrativa)
- [📚 Materiais de Apoio](#-materiais-de-apoio)
- [🚀 Próximos Passos](#-próximos-passos)

---

## 🔧 Programação de Jogos

### 🏗️ Fundamentos de Programação
- **Lógica de programação**
- **Estruturas de dados:** listas, filas, pilhas, árvores, grafos
- **Algoritmos:** busca, ordenação, pathfinding
- **Programação Orientada a Objetos (POO)**
- **Matemática para jogos:**
  - Vetores, matrizes
  - Trigonometria (ângulos, senos, cossenos)
  - Física (gravidade, aceleração, colisões)
  - Álgebra linear (essencial em 3D)

---

### 💻 Linguagens de Programação
- **GDScript (Godot)** — simples, ideal para iniciantes
- **C# (Unity)** — robusto e popular na indústria
- **C++ (Unreal Engine)** — alta performance, AAA
- **Python** — ótimo para prototipagem e lógica

---

### 🚀 Motores de Jogos
| Motor        | Linguagem | Prós                           | Contras                   |
|---------------|-----------|---------------------------------|----------------------------|
| **Godot**     | GDScript, C#, C++ | Leve, open-source, fácil de usar | Menor comunidade que Unity |
| **Unity**     | C#        | Ampla comunidade, multiplataforma | Licenciamento recente polêmico |
| **Unreal**    | C++, Blueprints | Gráficos AAA, realismo, otimização | Mais complexo para começar |
| **Construct** | Visual    | Sem código, rápido para 2D       | Pouco flexível, limitado |
| **GameMaker** | GML       | Fácil para 2D, bom suporte       | Limitado para 3D |

---

### 🔥 Habilidades-Chave em Programação
- Sistema de movimento (2D/3D)
- Sistema de colisões
- Sistema de input (teclado, mouse, joystick, toque)
- Gerenciamento de cenas e estados
- Sistema de UI (vida, mana, menus, inventário)
- Controle de som (música, efeitos sonoros, mixer)
- Inteligência artificial:
  - Pathfinding (A*)
  - FSM (Finite State Machine)
  - Behavior Trees
- Sistema de física:
  - Gravidade, força, atrito
- Save/Load de dados (JSON, SQLite, PlayerPrefs, arquivos)
- Multiplayer (Sockets, RPC, Servers — avançado)

---

### 🧠 Padrões e Arquitetura
- **ECS (Entity-Component-System)**
- **MVC (Model-View-Controller)**
- **State Machine (Máquina de Estados)**
- **Event-driven Programming (Programação baseada em eventos)**
- **Singletons e Service Locators**

---

### 📈 Aprofundamento Técnico
- Otimização (renderização, memória, scripts)
- Streaming de assets
- LOD (Level of Detail)
- Gerenciamento de memória (garbage collection, leaks)
- Shaders (GLSL, HLSL)
- Redes (multiplayer e servidores dedicados)
- Portabilidade (PC, Console, Mobile, Web)

---

## 🎨 Game Design

### 📖 O que é Game Design?
> Game Design é a arte e a ciência de criar sistemas, regras, mecânicas e experiências significativas e divertidas.

---

### 🏗️ Fundamentos do Game Design
- **MDA Framework:**  
  - **Mecânica:** regras, sistemas e interações básicas  
  - **Dinâmica:** como os sistemas interagem durante o jogo  
  - **Estética:** as sensações e emoções geradas
- **Tipos de Jogos:** plataforma, puzzle, RPG, FPS, RTS, MOBA, roguelike, etc.
- **Loops de jogo:**  
  - **Core Loop:** ação principal repetida (ex.: atirar, coletar, melhorar)  
  - **Meta Loop:** progresso a longo prazo (ex.: desbloquear fases, itens, conquistas)

---

### 🎯 Criação de Sistemas
- Sistema de progressão (níveis, XP, habilidades)
- Sistema de combate (balística, melee, magias)
- Sistema de recursos (dinheiro, vida, energia, inventário)
- Sistema de crafting
- Economia do jogo (loja, upgrades)
- Sistema de riscos e recompensas

---

### ⚖️ Balanceamento
- Curva de dificuldade
- Economias internas (escassez, abundância)
- Ritmo do jogo (picos de tensão, relaxamento)
- Fairness (justiça para o jogador)

---

### 🎨 UI/UX para Jogos
- Interfaces claras e intuitivas
- Feedback visual e sonoro
- HUD (vida, score, ammo, minimap)
- Acessibilidade (cores, fonte, legibilidade)

---

### 🔍 Análise e Teoria dos Jogos
- Psicologia do jogador (Flow, motivação intrínseca e extrínseca)
- Modelos:
  - **Bartle Types:** Achiever, Explorer, Socializer, Killer
  - **Octalysis:** Framework de gamificação
- Design de emoções (medo, surpresa, alívio, euforia)

---

### 📝 Documentação de Game Design
- **Game Design Document (GDD):**
  - Visão geral
  - Mecânicas
  - Personagens
  - História
  - Interface
  - Cronograma
- **Level Design Document (LDD)**
- **Narrative Design Document (NDD)**

---

## ✍️ Escrita de Histórias / Narrativa

### 🎭 Fundamentos da Narrativa em Jogos
- Diferença entre narrativa linear e interativa
- Storytelling emergente (histórias que surgem da jogabilidade)
- Ludonarrativa (quando a jogabilidade complementa ou contradiz a história)

---

### 🌎 Worldbuilding (Construção de Mundo)
- História do mundo
- Cultura, religião, política
- Ecossistema, clima, fauna, flora
- Tecnologia e magia
- Línguas e dialetos
- Cronologia (timeline de eventos)

---

### 🎭 Criação de Personagens
- Backstory (história anterior)
- Motivações e objetivos
- Defeitos, traumas e virtudes
- Desenvolvimento de arco narrativo
- Relações entre personagens

---

### 🧠 Estrutura Narrativa
- **Modelo de Jornada do Herói** (Joseph Campbell)
- **Estrutura de Três Atos**
- **Estrutura de Cinco Atos (Freytag)**
- Estruturas ramificadas:
  - Árvores de decisão
  - Sistemas de múltiplos finais
- Narrativa não linear

---

### 💬 Diálogos e Texto
- Árvores de diálogo
- Escolhas com consequências
- Texto adaptável ao contexto (condicional, procedural)
- Ferramentas:
  - **Ink** (Inkle)
  - **Twine** (HTML)
  - **Articy Draft** (profissional)

---

### 🧠 Técnicas de Escrita para Jogos
- **Mostrar, não contar:** narrativa visual e ambiental
- **Foreshadowing:** antecipação
- **Pacing:** controle do ritmo da narrativa
- **Simbolismo e metáforas visuais**

---

### 🎧 Narrativa Ambiental
- Cenários contam histórias:
  - Objetos quebrados, grafites, cadáveres, luzes
  - Sons e trilhas que ambientam
  - Cores e direção de arte

---

## 📚 Materiais de Apoio

### 📖 Livros
- **Game Design**
  - *The Art of Game Design* – Jesse Schell
  - *Game Design Workshop* – Tracy Fullerton
  - *Rules of Play* – Katie Salen & Eric Zimmerman
  - *Level Up!* – Scott Rogers
- **Narrativa**
  - *Wonderbook* – Jeff VanderMeer
  - *Into The Woods* – John Yorke
  - *The Writer's Journey* – Christopher Vogler
  - *Invisible Ink* – Brian McDonald
- **Programação de Jogos**
  - *Game Programming Patterns* – Robert Nystrom
  - *3D Math Primer for Graphics and Game Development* – Dunn & Parberry

### 🎥 Canais YouTube
- **Game Design:** Extra Credits, Game Maker's Toolkit, Design Doc
- **Programação:** Brackeys (Unity), HeartBeast (Godot), Mix and Jam
- **Narrativa:** GDC (Game Developers Conference), StoryMode, Behind the Screenplay

### 🧠 Cursos
- **Udemy:** GameDev.tv, cursos de Godot, Unity, Unreal
- **Coursera:** Michigan Game Design
- **Alura:** Desenvolvimento de Jogos (português)
- **Brackeys Academy:** Unity
- **GDC Vault:** Palestras avançadas

---

## 🚀 Próximos Passos

1. **Escolha seu motor de jogo:**  
   Recomendo começar com **Godot** (open-source) ou **Unity**.

2. **Faça projetos pequenos:**  
   Pong, Flappy Bird, Endless Runner, Plataforma simples.

3. **Documente tudo:**  
   Crie seu próprio **Game Design Document (GDD)**.

4. **Publique seus jogos:**  
   Plataformas: **Itch.io**, **GameJolt**, **Steam** (futuro).

5. **Monte portfólio:**  
   Demonstre seus projetos, mostre suas habilidades.

6. **Itere:**  
   Crie, teste, aprenda, melhore, repita.

---

## 💡 Dicas Finais
> Jogos são a interseção perfeita de arte, tecnologia e narrativa.  
> Comece simples. Nunca subestime um jogo pequeno — ele te ensina tudo que um grande ensina.

---
