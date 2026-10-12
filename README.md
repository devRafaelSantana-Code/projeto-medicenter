# 🏥 Medicenter — Portal Corporativo e Institucional

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/CSS_Grid-6C63FF?logo=css3&logoColor=white" alt="CSS Grid">
  <img src="https://img.shields.io/badge/Flexbox-6C63FF?logo=css3&logoColor=white" alt="Flexbox">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript">
</p>

## 🌐 Demonstração Online

Acede à versão publicada do projeto através do Vercel:

**[🚀 Visualizar Medicenter Online](https://projeto-medicenter-zeta.vercel.app/)**

## 📌 Sobre o Projeto

O **Medicenter** é um projeto de interface institucional desenvolvido para representar um portal destinado a clínicas, hospitais e organizações da área da saúde.

Baseado nos exercícios práticos da **B7Web**, o projeto foi desenvolvido com foco na organização do código, na apresentação de informações institucionais, na estruturação de áreas de notícias e na criação de uma experiência de navegação responsiva.

O principal objetivo deste repositório é demonstrar a aplicação de **HTML5 semântico, CSS3, variáveis nativas, Flexbox, CSS Grid e JavaScript Vanilla**, explorando a construção de interfaces adaptáveis, a manipulação do DOM e a implementação de elementos interativos.

> **Nota:** Este projeto tem finalidade exclusivamente educacional e não representa uma plataforma médica real nem fornece serviços de saúde.

---

## 🛠️ Tecnologias e Conceitos Aplicados

### 🧱 HTML5 Semântico e Acessibilidade

A estrutura utiliza elementos semânticos para organizar o conteúdo, melhorar a legibilidade do código e contribuir para a compreensão da página pelos motores de pesquisa e pelas tecnologias de apoio.

- **`<header>` e `<nav>`:** estruturação do cabeçalho e da navegação institucional.
- **`<main>`:** delimitação do conteúdo principal da página.
- **`<article>`:** organização de publicações independentes na área de notícias.
- **`<aside>`:** apresentação de conteúdos complementares, como departamentos e chamadas para ação.
- **`<footer>`:** organização das informações institucionais e dos contactos.

### 📐 Sistema de Layout Híbrido — Flexbox e CSS Grid

A interface combina diferentes sistemas de layout para organizar os elementos de forma consistente e adaptável.

- **CSS Grid:** organização das notícias e dos departamentos em colunas, com controlo do espaçamento e da distribuição dos elementos.
- **Flexbox:** criação de layouts flexíveis para o cabeçalho, os elementos do banner, os componentes de contacto e o rodapé.
- **CSS Variables (`:root`):** centralização de cores e outros valores reutilizáveis, facilitando a manutenção e a consistência visual.
- **Media Queries:** adaptação da estrutura, das dimensões e da disposição dos elementos a diferentes tamanhos de ecrã.

### 📱 Design Responsivo Multibreakpoint

A interface foi estruturada para adaptar a apresentação do conteúdo a diferentes resoluções, com especial atenção à legibilidade e à navegação em dispositivos móveis.

- **Desktop e portáteis:** apresentação horizontal do conteúdo principal e da barra lateral.
- **Tablets:** reorganização das áreas de conteúdo, com empilhamento da barra lateral e distribuição das notícias em duas colunas.
- **Smartphones:** adaptação para uma coluna, com aproveitamento do espaço disponível e imagens ajustadas ao contentor.
- **Ecrãs pequenos:** ajustes nas dimensões e nos elementos de contacto para reduzir o risco de rolagem horizontal.

### ⚙️ JavaScript e Manipulação Dinâmica do DOM

O JavaScript é utilizado para implementar o comportamento interativo do menu de navegação em dispositivos móveis.

- **`DOMContentLoaded`:** inicialização da lógica de interação após a análise do documento HTML.
- **Estado de acessibilidade:** atualização do atributo `aria-expanded` de acordo com o estado do menu.
- **Menu hambúrguer animado:** transformação visual do botão de navegação através de transições CSS.
- **Redimensionamento da janela:** tratamento da mudança entre os modos de navegação móvel e desktop.

---

## 📐 Estrutura Avançada da Interface

### 🏥 Hero — Área de Destaque

A área principal de destaque apresenta a identidade visual do portal e organiza as chamadas para ação, facilitando o acesso às principais secções da interface.

O botão do menu móvel utiliza transições CSS para transformar as três linhas do ícone num símbolo de fecho quando a navegação está ativa.

### 📰 Grid de Notícias Adaptável

A área de notícias utiliza CSS Grid para distribuir os conteúdos em colunas, com espaçamento consistente entre os elementos.

```css
.flex {
   display: grid;
   grid-template-columns: repeat(2, 1fr);
   gap: 20px;
}

/* Em ecrãs pequenos, o conteúdo passa para uma coluna. */
```

A quantidade de colunas é ajustada através de media queries, permitindo adaptar a apresentação ao espaço disponível.

### 📅 Atendimento e Canais de Contacto

A interface organiza os horários de atendimento e os canais de contacto em blocos informativos de fácil leitura.

Os links com os protocolos `mailto:` e `tel:` permitem iniciar, respetivamente, uma ação de envio de e-mail ou de chamada telefónica através das aplicações compatíveis do dispositivo.

---

## 📱 Comportamento Responsivo

| Dispositivo           | Intervalo de referência       | Comportamento do layout                                           |
| :-------------------- | :---------------------------- | :---------------------------------------------------------------- |
| 🖥️ **Desktop**        | Acima de 1024px               | Conteúdo principal e barra lateral apresentados horizontalmente.  |
| 💻 **Tablet**         | Aproximadamente 768px a 900px | Reorganização dos blocos e notícias distribuídas em duas colunas. |
| 📱 **Smartphone**     | Até 720px                     | Conteúdo organizado numa coluna e navegação móvel.                |
| 📟 **Ecrãs pequenos** | Até 360px                     | Ajustes adicionais de dimensões e espaçamentos.                   |

---

## 🚀 Como Executar o Projeto Localmente

### 1. Clonar o repositório

```bash
git clone https://github.com/SEU-USUARIO/projeto-medicenter.git
```

### 2. Aceder ao diretório

```bash
cd projeto-medicenter
```

### 3. Executar a aplicação

Por se tratar de uma aplicação estática desenvolvida com HTML, CSS e JavaScript, basta abrir o ficheiro `index.html` num navegador moderno.

Para uma experiência de desenvolvimento mais prática, recomenda-se a utilização da extensão **Live Server** no Visual Studio Code, permitindo visualizar as alterações durante a edição dos ficheiros.

---

## 📂 Estrutura do Projeto

```text
projeto-medicenter/
│
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
│       └── ...
│
└── README.md
```

---

## 👨‍💻 Autor

Desenvolvido por **Rafael Santana** 🚀

**Estudante de Engenharia da Computação**, com foco no desenvolvimento Full-Stack, na criação de interfaces responsivas, na organização de código e na construção de aplicações web modernas.

---

<p align="center">
  Projeto desenvolvido para fins educacionais e para consolidação de conhecimentos em HTML5, CSS3, CSS Grid, Flexbox e desenvolvimento de interfaces responsivas.
</p>
