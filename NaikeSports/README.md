# NaikeSports — Equipamentos de Alta Performance

Projeto desenvolvido para a disciplina de **Desenvolvimento Web**, com foco na criação de uma vitrine virtual minimalista e realista para artigos esportivos, aplicando integralmente os fundamentos de marcação semântica e estilização (HTML5 e CSS3 - Capítulos 1 ao 5).

---

## 📋 Sumário
- [Visão Geral](#-visão-geral)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Conceitos e Tecnologias Aplicadas](#-conceitos-e-tecnologias-aplicadas)
  - [HTML5 Semântico e Estrutural](#html5-semântico-e-estrutural)
  - [CSS3 e Arquitetura Visual](#css3-e-arquitetura-visual)
- [Diferenciais de Design (vs. NexusTech)](#-diferenciais-de-design-vs-nexustech)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Autor](#-autor)

---

## 🎯 Visão Geral

O **NaikeSports** é um site de catálogo e apresentação de produtos esportivos de alta performance (corrida, vestuário técnico, smart wearables e cross-training). 

O layout foi planejado do zero com o objetivo de entregar uma experiência suave, sóbria e refinada, afastando-se de efeitos espalhafatosos e privilegiando o espaço em branco, tipografia fluida e imagens autênticas em alta definição.

---

## 📂 Estrutura do Projeto

```text
NaikeSports/
│
├── index.html              # Estrutura e marcação semântica do portal
├── README.md               # Documentação técnica do projeto
│
└── css/
    ├── reset.css           # Normalização de estilos (Eric Meyer Reset)
    └── estilos.css         # Folha de estilos personalizada e modular
```

---

## 🛠️ Conceitos e Tecnologias Aplicadas

O código adota estritamente os padrões fundamentais abordados do Capítulo 1 ao 5 da apostila de desenvolvimento web, dispensando frameworks externos e JavaScript.

### HTML5 Semântico e Estrutural
- **Elementos Estruturais de Seção**: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>` e `<footer>`.
- **Figuras e Imagens**: Emprego do par `<figure>` e `<figcaption>` para os itens do catálogo, com atributos `alt` descritivos e proporções consistentes.
- **Hierarquia de Cabeçalhos**: Encadeamento ordenado de títulos do `<h1>` ao `<h5>`.
- **Listas Semânticas**: 
  - Listas não-ordenadas (`<ul>`) para menus, navegações e subcategorias.
  - Listas ordenadas (`<ol>`) para a vitrine de produtos enumerados.
- **Tabelas Semânticas**: Inclusão de tabela técnica com `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<th>` (com `scope="col"`), `<tr>`, `<td>` e junção de células (`colspan`).
- **Formulários Estruturados**: Campos de busca e atendimento contemplando `<form>`, `<fieldset>`, `<legend>`, `<label>`, `<input>` (`text`, `email`, `search`, `checkbox`, `submit`), `<select>`, `<option>` e `<textarea>`.

### CSS3 e Arquitetura Visual
- **CSS Reset**: Uso do Eric Meyer Reset para anular inconsistências entre navegadores.
- **Box Model**: Controle estrito de `margin`, `padding`, `border`, `width`, `height` e `box-sizing: border-box`.
- **Posicionamento e Fluxo**: Estrutura baseada em `float`, `clear`, clearfix via `overflow: hidden`, `position: relative` e `position: sticky`.
- **Seletores e Pseudo-Classes**: Pseudo-classes de estado e estruturais (`:hover`, `:focus`, `:last-child`), seletores de descendência direta (`>`) e seletores de atributos.
- **Interatividade CSS Pura**: Submenus em cascata acionados por hover e transições suaves (`transition`, `transform`).

---

## 🎨 Diferenciais de Design (vs. NexusTech)

| Característica | NexusTech | NaikeSports |
|---|---|---|
| **Paleta de Cores** | Gradientes marcados em azul e vermelho | Tons minimalistas de verde floresta, sálvia e neutros suaves |
| **Imagens** | Renders/ilustrações genéricas | Fotografias esportivas realistas e de alta nitidez |
| **Microinterações** | Rotação e escala agressiva nos cards | Elevação suave (`translateY(-4px)`) com sombras orgânicas |
| **Navegação** | Menus verticais densos | Cabeçalho fixo com navegação limpa e categorias bem distribuídas |
| **Conteúdo Adicional**| Apenas vitrine de produtos | Manifesto institucional, comparativo de tecnologias e SAC completo |

---

## 🚀 Como Executar o Projeto

1. Certifique-se de que a pasta `NaikeSports` contenha os arquivos `index.html` e o subdiretório `css/`.
2. Dê um duplo clique no arquivo `index.html` ou abra-o diretamente no navegador de sua preferência (Google Chrome, Firefox, Safari, Microsoft Edge).
3. Não requer instalação de dependências ou servidor local.

---

## 👤 Autor

- **Desenvolvedor:** Samuel Ferreira Souto  
- **Disciplina:** Desenvolvimento Web  
- **Ano:** 2026
