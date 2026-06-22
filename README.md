# 🎮 Jogo do Número Secreto

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=%23323330)
![Alura](https://img.shields.io/badge/Alura-Challenge-%23167BF7?style=for-the-badge&logo=codecademy&logoColor=white)

Um jogo interativo e responsivo de adivinhação numérica desenvolvido com tecnologias web nativas. O sistema gera um número secreto aleatório e o jogador deve tentar adivinhá-lo recebendo feedbacks em tempo real.

---

## 📋 Sobre o Projeto

O **Jogo do Número Secreto** é uma aplicação desenvolvida como parte de um desafio prático da **Alura**. O projeto é focado na prática de lógica de programação, manipulação dinâmica do DOM (Document Object Model) e acessibilidade na web. O jogo possui um limite configurado para números de **1 a 50**.

### 🧠 Lógica e Funcionamento

O funcionamento do projeto é estruturado em três arquivos principais:

1. **`index.html`**: Define a estrutura semântica da aplicação. Contém a área de texto, o campo de entrada (`<input>`) para o palpite do usuário e os botões de ação ("Chutar" e "Novo jogo"). Também carrega as fontes externas do Google Fonts (*Chakra Petch* e *Inter*) e o script de acessibilidade.
2. **`style.css`**: Responsável pela identidade visual moderna do jogo. Utiliza um fundo gradiente escuro, efeito de ruído texturizado, posicionamento responsivo e estilização customizada para estados ativos e desativados (`:disabled`). Possui regras de `@media` para adaptar a interface para telas menores e dispositivos móveis, ocultando elementos decorativos e reorganizando o layout.
3. **`app.js`**: Centraliza toda a inteligência e o estado do jogo através das seguintes mecânicas:
   * **Sorteio com Recursividade**: A função `gerarNumeroAleatorio()` sorteia um número de 1 a 50 e verifica se ele já foi sorteado anteriormente. Se sim, a função chama a si mesma recursivamente até encontrar um número inédito.
   * **Controle de Estado de Array**: Os números já jogados são guardados em `listaDeNumerosSorteados`. Quando o tamanho da lista atinge o limite máximo (50), o array é automaticamente limpo para uma nova sequência.
   * **Feedback e Validação**: Valida se o palpite é maior ou menor que o número secreto, contabiliza o número de tentativas (com tratamento gramatical para singular e plural) e gerencia o estado do botão "Novo jogo" (`removeAttribute` e `setAttribute`).

---

## 🛠️ Tecnologias e Recursos Utilizados

* **HTML5** (Estruturação semântica)
* **CSS3** (Estilização avançada, Layout Flexbox e Responsividade)
* **JavaScript ES6+** (Manipulação do DOM, Funções, Arrays e Recursividade)
* **Google Fonts** (Fontes *Chakra Petch* e *Inter*)

---

## 🔧 Como Executar o Projeto Localmente

1. **Clone este repositório:**
```bash
   git clone https://github.com/Gold200707/sorteador-numero.git

```

2. **Navegue até o diretório do projeto:**

```bash
   cd sorteador-numero

```

3. **Abra o jogo:**
Basta abrir o arquivo `index.html` diretamente em seu navegador ou utilizar uma extensão como o *Live Server* no VS Code.

---

## 🎓 Origem e Aprendizado

Este projeto foi desenvolvido como um desafio (Challenge) proposto pela **Alura**, idealizado para aplicar na prática conceitos de funções, estruturas condicionais, arrays e boas práticas de desenvolvimento web.

---

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](./LICENSE) para obter mais detalhes.

---

## ✍️ Autor

Desenvolvido por Gold200707.

Se quiser trocar uma ideia ou acompanhar meus projetos:

* **GitHub**: [@Gold200707](https://github.com/Gold200707)
* **LinkedIn**: [João Lucas Magordo Rodrigues](https://www.linkedin.com/in/joão-lucas-magordo-rodrigues-343a543b5/)
