# 🏥 Medicenter — Portal Corporativo e Institucional

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" alt="CSS3">
  <img src="https://shields.io" alt="CSS Layouts">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript">
</p>

## 📌 Sobre o Projeto

O **Medicenter** é um projeto de interface institucional desenvolvido para representar um portal destinado a clínicas, hospitais e organizações da área da saúde.

O projeto foi estruturado com base nos exercícios práticos da **B7Web**, recebendo uma refatoração completa com foco em boas práticas modernas de arquitetura front-end, garantindo uma navegação limpa, áreas de notícias dinâmicas e blocos informativos robustos.

O principal objetivo deste repositório é demonstrar o uso avançado de **HTML5 semântico, CSS3 (com arquitetura de Variáveis Nativas), layouts responsivos híbridos (Flexbox + Grid) e JavaScript Vanilla** orientado a eventos e acessibilidade.

> **Nota:** Este projeto tem finalidade exclusivamente educacional e não representa uma plataforma médica real nem fornece serviços de saúde.

---

## 🛠️ Tecnologias e Conceitos Aplicados

### 🧱 HTML5 Semântico & Acessibilidade

A estrutura foi desenhada utilizando tags semânticas estritas para otimizar a legibilidade do código e o SEO estrutural:

- `<header>` e `<nav>` gerenciando o fluxo de navegação institucional;
- `<main>` delimitando o núcleo de dados da página;
- `<article>` encapsulando cada publicação da área de notícias de forma independente;
- `<aside>` organizando componentes complementares (como o bloco de departamentos e chamadas para ação);
- `<footer>` estruturando o fechamento institucional e dados cadastrais.

### 📐 Sistema de Layout Híbrido (Flexbox + CSS Grid)

A distribuição espacial dos elementos foi atualizada para extrair o melhor de dois mundos:

- **CSS Grid:** Aplicado na área de notícias (`.flex`) e departamentos para renderizar colunas matemáticas exatas e dinâmicas, eliminando cálculos manuais de margem.
- **Flexbox:** Utilizado no alinhamento de componentes unidimensionais, como a centralização de itens do cabeçalho, distribuição dos blocos do banner principal e organização interna do rodapé.
- **CSS Variables (:root):** Centralização de toda a paleta de cores e limites de largura em variáveis globais, simplificando manutenções futuras.

### 📱 Design Responsivo Multi-Breakpoint (320px a 1024px)

Diferente de layouts baseados em apenas um ponto de quebra, a responsividade deste projeto foi refatorada e testada cirurgicamente sob três cenários críticos de visualização:

- **Desktop & Laptops (Acima de 1024px):** Layout amplo em proporção `flex: 2` para conteúdo e `flex: 1` para barra lateral.
- **Tablets (Breakpoint 900px / Foco em 768px):** Transição inteligente onde a barra lateral é empilhada verticalmente abaixo das notícias para evitar o esmagamento de texto. O bloco de notícias reorganiza-se automaticamente em **2 colunas perfeitas**.
- **Smartphones Ultra-Pequenos (Breakpoint 360px / Foco em 320px):** Proteção especial para telas estilo iPhone SE. Os componentes de contato convertem suas larguras rígidas para preenchimento fluído (`height: auto`), impedindo o surgimento de barras de rolagem horizontal.

### ⚙️ JavaScript & Manipulação Dinâmica do DOM

O comportamento do menu mobile foi blindado contra falhas comuns de renderização:

- **Garantia de Ciclo de Vida:** O código é disparado via `DOMContentLoaded`, permitindo a interação instantânea antes mesmo do carregamento total de imagens pesadas.
- **Controle de Estado de Acessibilidade:** O clique gerencia os atributos `aria-expanded` dinamicamente entre `true` e `false`.
- **Efeito Anti-Quebra no Redimensionamento:** Inclui um observador do evento `resize` da janela do navegador que limpa automaticamente as classes móveis se o usuário expandir a tela de um smartphone diretamente para o Desktop.

---

## 📐 Estrutura Avançada da Interface

### 🏥 Hero / Área de Destaque Animada

O banner principal utiliza o conceito de posicionamento centralizado combinado com opções de ações imediatas. O botão expansível do menu mobile recebeu estilos nativos que **transformam as 3 linhas clássicas num "X" animado via CSS Transitions** assim que o menu é ativado.

### 📰 Grid de Notícias Adaptável

As publicações se reorganizam de forma totalmente responsiva:

```css
.flex {
   display: grid;
   grid-template-columns: repeat(2, 1fr);
   gap: 20px;
}
/* No mobile o grid colapsa para apenas uma coluna (1fr) de forma fluida */
```

### 📅 Atendimento e Canais de Contato

Estrutura adaptada com herança de fontes controlada para links telefônicos (`mailto:` e `tel:`), oferecendo uma experiência de usabilidade real ao usuário final em dispositivos móveis.

---

## 📱 Tabela de Comportamento Responsivo

| Dispositivo           | Breakpoint Alvo   | Comportamento do Layout                           | Navegação de Cima              |
| :-------------------- | :---------------- | :------------------------------------------------ | :----------------------------- |
| 🖥️ **Desktop**        | Superior a 1025px | Multi-colunas horizontais completas               | Horizontal Estendida           |
| 💻 **Tablet**         | 768px a 900px     | Empilhamento de Blocos + Notícias em 2 Colunas    | Compacta / Ativação Antecipada |
| 📱 **Mobile Normal**  | Até 720px         | Coluna única vertical, imagens em tamanho total   | Menu Hambúrguer Oculto         |
| 📟 **Mobile Pequeno** | Até 320px         | Fontes reduzidas, contatos adaptáveis sem quebras | Menu Hambúrguer Oculto         |

---

## 🚀 Como Executar o Projeto Localmente

### 1. Clonar o repositório

```bash
git clone https://github.com/SEU-USUARIO/projeto-medicenter.git
```

### 2. Aceder ao diretório do projeto

```bash
cd projeto-medicenter
```

### 3. Execução

Por tratar-se de uma aplicação estática construída com JavaScript puro, basta abrir o arquivo `index.html` diretamente em qualquer navegador moderno.

_Dica de Desenvolvimento:_ Recomenda-se o uso da extensão **Live Server** no VS Code para refletir alterações em tempo real durante os testes de responsividade.

---

## 📂 Estrutura Estrutural do Repositório

```text
projeto-medicenter/
│
├── index.html          # Estrutura semântica e lógica JS unificada/corrigida
├── assets/
│   ├── css/
│   │   └── style.css   # Estilização com variáveis CSS, Grid, Flexbox e queries
│   └── images/
│       └── ...         # Assets visuais do template
└── README.md           # Documentação técnica do projeto
```

---

## 👨‍💻 Autor

Desenvolvido por **Rafael Santana** 🚀

**Estudante de Engenharia da Computação**, focado no desenvolvimento Front-end de alta performance, arquitetura CSS limpa, semântica e interfaces modernas e inclusivas para a web.

---

<p align="center">
  Projeto desenvolvido para fins educacionais e para consolidação avançada de layouts híbridos e manipulação nativa do DOM.
</p>    └── ...         # Assets visuais do template
└── README.md           # Documentação técnica do projeto
```

---

## 👨‍💻 Autor

Desenvolvido por **Rafael Santana** 🚀

**Estudante de Engenharia da Computação**, focado no desenvolvimento Front-end de alta performance, arquitetura CSS limpa, semântica e interfaces modernas e inclusivas para a web.

---

<p align="center">
  Projeto desenvolvido para fins educacionais e para consolidação avançada de layouts híbridos e manipulação nativa do DOM.
</p>
