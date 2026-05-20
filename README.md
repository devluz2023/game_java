# 🎮 Game Development Lab - Native Java Object-Oriented Simulation

Este repositório centraliza o desenvolvimento de uma aplicação de simulação interativa ou jogo digital, construída nativamente na linguagem **Java**. O projeto explora os recursos fundamentais da plataforma Java Standard Edition (Java SE) para renderização gráfica, controle de estados e processamento de eventos em tempo real, demonstrando a aplicação prática de padrões avançados de Programação Orientada a Objetos (POO) e arquiteturas baseadas em eventos.

---

## 🏗️ Estrutura e Governança do Projeto

O espaço de trabalho segue a convenção de pacotes recomendada para o desenvolvimento estruturado na comunidade Java:

* **`src/br/com/gamejava/main/`:** Diretório que armazena os arquivos de código-fonte (`.java`). Centraliza as classes principais da aplicação, incluindo o ponto de entrada do sistema (`main`), controladores gráficos, lógicas de movimentação de entidades, detecção de colisões e gerenciamento do ciclo de vida da simulação.
* **`bin/br/com/gamejava/main/`:** Pasta destinada a armazenar o bytecode compilado (`.class`), separando as lógicas legíveis do ambiente de execução interpretado pela Java Virtual Machine (JVM).
* **⚙️ Configurações de Ambiente (`.project`, `.classpath`, `.settings/`):** Arquivos nativos de ambientes de desenvolvimento integrados (IDEs), garantindo a consistência das flags de compilação, build path de bibliotecas padrão e compatibilidade de ambiente entre diferentes plataformas de desenvolvimento.

---

## 🛠️ Stack Tecnológica & Engenharia de Jogos

* **Linguagem Core:** Java (Strongly Typed & Object-Oriented).
* **Ambiente de Execução:** Java Virtual Machine (JVM) / JDK Core.
* **Conceitos de Engenharia de Software Aplicados:**
  * **Game Loop Pattern:** Implementação de uma estrutura de repetição contínua (loop) assíncrona responsável por sincronizar a taxa de atualização lógica do jogo (*Ticks*) e a taxa de renderização de quadros na tela (*FPS - Frames Per Second*).
  * **Event-Driven Architecture:** Uso de rotinas de captura e tratamento de interrupções de periféricos (como eventos de teclado e mouse) para controle em tempo real.
  * **Concorrência e Multi-Threading:** Gerenciamento de tarefas em segundo plano através de Threads nativas para garantir que o processamento lógico da aplicação não bloqueie a interface gráfica principal (*UI Thread*).

---

## 🎯 Impacto Prático no Perfil de Engenharia de Software

O desenvolvimento de jogos e simulações gráficas do zero na linguagem Java é uma das melhores maneiras de consolidar competências críticas de arquitetura que são altamente valorizadas em sistemas empresariais complexos:

1. **Domínio Avançado de POO:** Exige o uso pesado e refinado de herança, polimorfismo, encapsulamento e composição para gerenciar diferentes entidades do sistema (cenários, jogadores, inimigos, scores) de forma desacoplada e limpa.
2. **Gerenciamento Eficiente de Memória e Performance:** Jogos rodam sob restrições rígidas de tempo de execução. Desenhar estruturas lógicas eficientes evita o acionamento excessivo do *Garbage Collector* da JVM, o que causaria quedas de performance (*lags*) na aplicação.
3. **Resolução Complexa de Problemas:** A criação de mecânicas, algoritmos de inteligência artificial simples para entidades automatizadas e lógica de colisão matemática desenvolve um raciocínio lógico profundo e focado em otimização computacional.

---
## 🚀 Como Compilar e Executar a Simulação

Você pode rodar este projeto utilizando o terminal de comandos padrão do seu sistema operacional (com o JDK configurado):

1. Acesse a pasta raiz do repositório.
2. Compile todas as classes java estruturadas a partir do diretório de pacotes:
   ```bash
   javac -d bin src/br/com/gamejava/main/*.java
