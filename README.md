🧟 Jogo Zumbi 2D — Interface Web

Sobreviva ao apocalipse! Uma interface web responsiva e interativa criada para apresentar o universo do Jogo Zumbi 2D, com informações sobre a história, controles, demonstração da jogabilidade e animações dinâmicas de zumbis.

⸻

📖 Sobre o projeto

O Jogo Zumbi 2D — Interface Web é um projeto desenvolvido utilizando HTML, CSS, JavaScript e Bootstrap, com o objetivo de criar um site de apresentação para um jogo de sobrevivência contra zumbis.

A interface possui uma identidade visual inspirada no universo pós-apocalíptico, utilizando tons escuros, detalhes em verde e personagens animados que caminham aleatoriamente pela tela.

O site foi desenvolvido com atenção à responsividade, organização do código, experiência do usuário e acessibilidade, oferecendo uma navegação adaptada a diferentes tamanhos de tela.

Importante: este repositório contém a interface web de apresentação. O jogo desenvolvido em Python/Pygame é um projeto separado.

🎮 Repositório do jogo: Jogo Zumbi 2D — Python

⸻

🎮 Funcionalidades

🏠 Página inicial

* Apresentação do Jogo Zumbi 2D.
* Menu de navegação responsivo.
* Acesso às páginas História, Como Jogar e Download.
* Configurações personalizáveis de acessibilidade.
* Zumbis animados caminhando pelo cenário.

📜 História

* Apresentação do universo pós-apocalíptico.
* Explicação do cenário e da missão do jogador.
* Cronologia com os acontecimentos de seis dias.
* Imagens ilustrativas e organização visual das informações.

🕹️ Como jogar

* Explicação dos comandos do jogo.
* Cartões responsivos com informações sobre os controles.
* Orientações sobre movimentação, ataques e navegação.

Comando	Ação
W, A, S, D	Movimentar o personagem
Clique esquerdo	Atirar
C	Alterar a cor do personagem
Esc	Voltar ao menu

📥 Download

* Vídeo demonstrativo da jogabilidade.
* Reprodução automática sem som, com controles disponíveis.
* Player responsivo em proporção 16:9.
* Botão para baixar um arquivo de vídeo disponibilizado no projeto.

⸻

🧟 Sistema de zumbis animados

Uma das principais funcionalidades da interface é o sistema de zumbis desenvolvido em JavaScript.

Os personagens são criados dinamicamente e caminham pela página com trajetórias e velocidades independentes.

⚙️ Funcionamento

* Os zumbis aparecem a partir de bordas aleatórias da tela.
* Cada personagem possui posição, direção e velocidade próprias.
* A movimentação ocorre continuamente com requestAnimationFrame().
* Quando um zumbi sai da tela, uma nova trajetória é sorteada.
* Novos personagens são adicionados automaticamente com o passar do tempo.
* A quantidade máxima é limitada para evitar crescimento indefinido.
* A contagem reinicia quando a página é recarregada.

📊 Configuração atual

Parâmetro	Valor
Quantidade inicial	4 zumbis
Intervalo de crescimento	30 segundos
Zumbis adicionados	1 por intervalo
Quantidade máxima	12 zumbis
Velocidade	Aleatória entre 70 e 140 px/s

O sistema utiliza funções como Math.random(), Math.hypot() e Math.atan2() para calcular posições, direções e ângulos de movimentação.

⸻

♿ Acessibilidade

O projeto inclui recursos de acessibilidade com foco em melhorar a experiência de navegação.

Funcionalidades implementadas

* Alto contraste: altera a combinação de cores para melhorar a visualização dos elementos.
* Texto grande: aumenta o tamanho base das fontes.
* Preferências salvas: utiliza localStorage para manter as configurações ao navegar entre as páginas.
* Sincronização entre abas: utiliza o evento storage para atualizar preferências modificadas em outra aba.
* Estrutura semântica: utiliza elementos como header, nav, main e section.
* Controles identificados: utiliza labels e atributos ARIA em componentes interativos.
* Movimento reduzido: inclui regras CSS para limitar determinadas animações e transições quando essa preferência está ativa.

O desenvolvimento considera boas práticas relacionadas às WCAG 2.2, mas ainda pode receber melhorias e testes adicionais de conformidade.

⸻

🛠️ Tecnologias utilizadas

Tecnologia	Utilização
HTML5	Estruturação das páginas e organização semântica
CSS3	Estilização, cores, posicionamento e animações visuais
JavaScript	Interatividade, movimentação dos zumbis e acessibilidade
Bootstrap 5.3.8	Layout responsivo, navbar, grid, cartões e botões
LocalStorage	Armazenamento das preferências de acessibilidade
Git e GitHub	Versionamento e armazenamento do projeto

📱 Bootstrap

O Bootstrap foi utilizado principalmente para:

* Criar um sistema de grid responsivo com container, row e col.
* Adaptar a navegação para celulares com navbar e navbar-toggler.
* Estilizar botões e cartões.
* Organizar espaçamentos e alinhamentos.
* Manter o vídeo responsivo com ratio-16x9.
* Criar os controles de acessibilidade utilizando form-switch.

⸻

📁 Estrutura do projeto

interface_jogozumbi2d/
│
├── index.html
├── historia.html
├── como-jogar.html
├── baixar-jogo.html
│
├── style.css
├── script.js
├── zumbi.js
│
├── assets/
│   ├── zumbi-andando.gif
│   ├── apocalipsezumbi1.jpg
│   ├── apocalipsezumbi2.jpg
│   ├── apocalipsezumbi3.webp
│   ├── videogameplay.mp4
│   └── JOGO.mp4
│
└── README.md

📄 Responsabilidade dos arquivos

index.html — Estrutura da página inicial e apresentação do projeto.

historia.html — Conteúdo narrativo e cronologia do apocalipse.

como-jogar.html — Explicação dos controles e objetivos do jogo.

baixar-jogo.html — Vídeo demonstrativo e botão de download.

style.css — Estilos visuais, cores, responsividade e posicionamento.

script.js — Funcionalidades de acessibilidade e persistência das preferências.

zumbi.js — Criação, movimentação e crescimento progressivo dos zumbis.

assets/ — Imagens, animações GIF e arquivos de vídeo.

⸻

🚀 Como executar o projeto

1. Clonar o repositório

git clone https://github.com/leehsantos13/interface_jogozumbi2d.git

2. Abrir a pasta

cd interface_jogozumbi2d

3. Executar o site

Abra o projeto no Visual Studio Code e utilize a extensão Live Server.

Clique com o botão direito no arquivo index.html e selecione Open with Live Server.

O navegador abrirá a interface e você poderá navegar entre as páginas.

Observação: o projeto não exige instalação de dependências pelo npm. O Bootstrap é carregado por CDN, portanto é necessária conexão com a internet para carregar essa biblioteca.

⸻

🧠 Conceitos aplicados

Durante o desenvolvimento, foram utilizados conceitos importantes de programação e desenvolvimento web:

* Manipulação do DOM com JavaScript.
* Eventos e interação com elementos HTML.
* Objetos e arrays.
* Funções e estruturas condicionais.
* Laços de repetição.
* Temporizadores com setInterval().
* Animação com requestAnimationFrame().
* Geração de valores aleatórios.
* Armazenamento local de dados.
* Layout responsivo utilizando Bootstrap.
* Organização de código em arquivos independentes.

⸻

🔮 Possíveis melhorias futuras

* Adicionar uma opção para pausar as animações dos zumbis.
* Melhorar a acessibilidade com testes de teclado e leitores de tela.
* Adicionar legendas ao vídeo de demonstração.
* Criar uma página com informações sobre os personagens e inimigos.
* Integrar o download de uma versão executável do jogo.
* Melhorar o desempenho das animações em dispositivos móveis.

⸻

👨‍💻 Desenvolvimento

Projeto acadêmico desenvolvido com foco na aplicação prática de conceitos de desenvolvimento web, responsividade, JavaScript e acessibilidade.

⸻

🧟‍♂️ O apocalipse começou. Você está preparado para sobreviver?

Desenvolvido com HTML, CSS, JavaScript e Bootstrap.