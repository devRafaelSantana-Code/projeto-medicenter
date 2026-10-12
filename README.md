# 🏥 Medicenter — Portal Corporativo e Institucional

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/Flexbox-Layout-6C63FF" alt="CSS Flexbox">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript">
</p>

## 📌 Sobre o Projeto

O **Medicenter** é um projeto de interface institucional desenvolvido para representar um portal destinado a clínicas, hospitais e organizações da área da saúde.

O projeto foi desenvolvido no contexto dos exercícios práticos da **B7Web**, com foco na construção de uma página comercial completa, combinando navegação, áreas de destaque, informações de atendimento, notícias, contactos e elementos de marcação de consultas.

O principal objetivo é demonstrar a utilização de **HTML5 semântico, CSS3, Flexbox, Media Queries e JavaScript** na construção de uma interface responsiva e organizada.

> **Nota:** Este projeto tem finalidade exclusivamente educacional e não representa uma plataforma médica real nem fornece serviços de saúde.

---

## 🛠️ Tecnologias e Conceitos

### 🧱 HTML5 Semântico

A estrutura da página utiliza elementos semânticos para organizar diferentes tipos de conteúdo:

- `<header>` para o cabeçalho e navegação;
- `<main>` para o conteúdo principal;
- `<section>` para diferentes áreas da página;
- `<article>` para conteúdos independentes, como notícias;
- `<aside>` para conteúdos complementares;
- `<footer>` para informações institucionais e links adicionais.

A utilização destes elementos contribui para uma estrutura mais clara e facilita a manutenção do código.

### 📐 CSS3 + Flexbox

O layout utiliza **CSS Flexbox** como principal sistema de distribuição dos elementos.

Entre os conceitos aplicados estão:

- `display: flex`;
- `flex-direction`;
- `flex`;
- `justify-content`;
- `align-items`;
- `flex-wrap`;
- distribuição proporcional entre áreas de conteúdo;
- organização de colunas e componentes.

Em determinadas áreas, o conteúdo principal recebe maior espaço através de uma proporção `flex: 2`, enquanto a área lateral utiliza `flex: 1`.

### 📱 Design Responsivo

A interface adapta-se a diferentes dimensões de ecrã através de **Media Queries**.

A partir do breakpoint definido no projeto, alguns elementos passam de uma organização horizontal para vertical, permitindo uma melhor utilização do espaço disponível em dispositivos móveis.

Entre os ajustes realizados encontram-se:

- alteração da direção dos elementos Flexbox;
- reorganização das colunas;
- adaptação dos espaçamentos;
- ajuste da navegação;
- utilização de largura total em determinados componentes.

### ⚙️ JavaScript

O JavaScript é utilizado para controlar o comportamento da navegação em dispositivos móveis.

O menu hambúrguer permite alternar a visibilidade do menu através da manipulação do DOM, sem necessidade de bibliotecas externas.

A lógica é executada após o carregamento da página, garantindo que os elementos necessários estejam disponíveis antes da interação.

---

## 📐 Estrutura da Interface

O projeto está organizado em diferentes áreas funcionais para criar uma experiência semelhante à de um portal institucional.

### 🏥 Hero / Área de Destaque

A área principal apresenta informações de destaque da instituição, utilizando uma imagem de fundo adaptável através de:

```css
background-size: cover;
```

Esta abordagem permite que a imagem ocupe a área disponível mantendo uma apresentação visual consistente.

### 📰 Área de Notícias

A secção de notícias apresenta artigos organizados através de Flexbox, permitindo que os conteúdos se distribuam de forma flexível e utilizem `flex-wrap` quando necessário.

Cada publicação é estruturada através de elementos semânticos `<article>`.

### 📅 Atendimento e Marcação

A interface inclui áreas destinadas a informações de atendimento, contactos e ações relacionadas com marcações de consultas.

O objetivo é simular uma estrutura comum em websites institucionais da área da saúde.

### 🔗 Navegação

O cabeçalho disponibiliza os principais links de navegação e inclui uma versão adaptada para dispositivos móveis através do menu hambúrguer controlado por JavaScript.

### 📋 Rodapé Institucional

O `<footer>` reúne diferentes grupos de informação, como:

- informações institucionais;
- links;
- conteúdos recentes;
- contactos;
- áreas complementares do portal.

---

## 📱 Responsividade

O projeto foi desenvolvido considerando diferentes dimensões de ecrã:

| Dispositivo | Comportamento                                  |
| ----------- | ---------------------------------------------- |
| 🖥️ Desktop  | Layout horizontal com múltiplas áreas          |
| 💻 Tablet   | Ajuste progressivo de espaçamentos e dimensões |
| 📱 Mobile   | Organização vertical e navegação adaptada      |

O breakpoint principal utilizado no projeto é de **720px**, a partir do qual determinadas estruturas Flexbox passam para uma organização vertical.

---

## 🚀 Como Executar o Projeto Localmente

### 1. Clona o repositório

```bash
git clone https://github.com/SEU-USUARIO/projeto-medicenter.git
```

### 2. Acede ao diretório

```bash
cd projeto-medicenter
```

### 3. Abre o projeto

Podes abrir diretamente o ficheiro:

```text
index.html
```

no navegador.

Como alternativa, recomenda-se utilizar a extensão **Live Server** no Visual Studio Code para obter uma experiência de desenvolvimento mais prática.

---

## 📂 Estrutura do Projeto

```text
projeto-medicenter/
│
├── index.html
├── style.css
├── script.js
├── imagens/
│   └── ...
└── README.md
```

---

## 🎯 Competências Demonstradas

Este projeto permite demonstrar conhecimentos em:

- HTML5 semântico;
- CSS3;
- CSS Flexbox;
- Media Queries;
- Design responsivo;
- JavaScript e manipulação do DOM;
- Estruturação de layouts institucionais;
- Organização de componentes de interface;
- Navegação responsiva;
- Boas práticas de estruturação de páginas web.

---

## 👨‍💻 Autor

Desenvolvido por **Rafael Santana** 🚀

**Estudante de Engenharia da Computação**, com foco no desenvolvimento Front-end, criação de interfaces responsivas, semântica HTML e construção de layouts para aplicações web.

---

<p align="center">
  Projeto desenvolvido para fins educacionais e para consolidação de conhecimentos em HTML5, CSS3, Flexbox, JavaScript e desenvolvimento de interfaces institucionais responsivas.
</p>
