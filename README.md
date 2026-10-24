# Atividade Prática: Desenvolvimento de Interface Web (HTML5 & CSS3)

**Disciplina:** Desenvolvimento Web  
**Professor:** Alyson Trindade Fernandes  
**Projeto:** Vitrine e Destaques - NexusTech (Loja de Tecnologia e Inovação)  
**Tecnologias:** HTML5 semântico e CSS3 puro (sem JavaScript)  
**Nota Máxima:** 10,0 pontos  

---

## 📁 Estrutura de Arquivos do Projeto

```text
WEB I/
│
├── index.html          # Documento principal com marcação semântica em HTML5
├── css/
│   ├── reset.css       # Reset clássico de estilos (Eric Meyer v2.0)
│   └── estilos.css     # Folha de estilos principal comentada e organizada
├── img/                # Ativos gráficos e imagens da loja
│   ├── logo.png        # Logotipo vetorial da marca NexusTech
│   ├── sacola.png      # Ícone da sacola de compras
│   ├── busca.png       # Ícone da lupa de busca
│   ├── destaque.png    # Banner promocional tecnológico de alta resolução
│   ├── produto1.png    # Smartphone Nexus Z
│   ├── produto2.png    # Smartwatch Pulse Fit
│   ├── produto3.png    # Headphone ANC Hi-Fi
│   ├── produto4.png    # Notebook Titan AI
│   ├── produto5.png    # Console Next 4K
│   ├── produto6.png    # Drone Vision 4K
│   ├── facebook.png    # Ícone oficial para Image Replacement
│   ├── twitter.png     # Ícone oficial para Image Replacement
│   └── fundo-rodape.png# Textura de fundo para o rodapé
└── README.md           # Documentação completa do projeto
```

---

## 📋 Checklist de Requisitos e Critérios de Avaliação

### 1. Estrutura de Arquivos e Cabeçalho Semântico (2,0 pontos)
- [x] **Organização:** Arquivo `index.html` na raiz, pastas `css/` e `img/`.
- [x] **Reset CSS:** `reset.css` (estilo Eric Meyer) importado **antes** de `estilos.css`.
- [x] **Classe `.container`:** Largura fixa de `940px` centralizada na horizontal (`margin: 0 auto;`).
- [x] **Marcação Semântica do Topo:**
  - Título principal `<h1>` com o logotipo da loja e texto alternativo descritivo (`alt`).
  - Parágrafo `<p class="sacola">` indicando os itens do carrinho/sacola.
  - Menu primário dentro de `<nav>` com lista `<ul>` contendo 5 links `<a>`.
- [x] **Posicionamento do Topo:**
  - `<header>` configurado com `position: relative;`.
  - Sacola fixada no canto superior direito (`position: absolute; top: 0; right: 0;`).
  - Menu alinhado no canto inferior direito (`position: absolute; bottom: 0; right: 0;`).
  - Itens da lista (`<li>`) dispostos na horizontal com `display: inline-block;`.

---

### 2. Área de Destaque com Busca e Menu Lateral (2,5 pontos)
- [x] **Formulário de Busca:**
  - Elemento `<section class="busca">` contendo `<form>` com `<input type="search">` e `<input type="image">` (ícone da lupa).
  - Alinhamento vertical do campo e botão com `vertical-align: middle;`.
- [x] **Menu Lateral com Efeito Sanfona em CSS Puro:**
  - `<section class="menu-departamentos">` com links de categorias.
  - Sublistas `<ul>` com subcategorias.
  - Sublistas iniciam ocultas (`display: none;`) e surgem ao passar o mouse sobre o item pai (`:hover -> display: block;`).
- [x] **Flutuação e Quebra de Fluxo:**
  - Bloco de busca com `float: left;`.
  - Menu de departamentos com `float: left; clear: left;` obrigatório.
  - Banner de destaque posicionado ao lado direito (`float: right;`).

---

### 3. Vitrine de Produtos com Display Inline-Block (2,5 pontos)
- [x] **Seções Irmãs:** Seção de vitrine com painéis de **Novidades** e **Mais Vendidos**.
- [x] **Flutuação dos Painéis:** Flutuam lado a lado (`float: left;` e `float: right;`) com largura aproximada de `445px`.
- [x] **Estrutura dos Produtos:**
  - Lista estruturada (`<ol>`) com itens `<li>` contendo `<figure>`, `<img>` e `<figcaption>` (título e preço).
  - Alinhamento horizontal com `display: inline-block;` e alinhamento vertical ao topo (`vertical-align: top;`).
- [x] **Gradientes e Cores:**
  - Fundo suave com `linear-gradient()` do CSS3 em cada painel.
  - Cantos arredondados elegantes com `border-radius`.

---

### 4. Rodapé Semântico e Substituição de Imagem (1,5 ponto)
- [x] **Rodapé Semântico:**
  - Tag `<footer>` com largura de `100%`, cor e imagem de fundo (`background-color` e `background-image`).
  - Propriedade `clear: both;` para não colidir com as seções flutuantes anteriores.
  - Div `<div class="container">` interna mantendo o alinhamento no limite de `940px` do centro da tela.
- [x] **Redes Sociais com Image Replacement:**
  - Estrutura HTML idêntica à solicitada:
    ```html
    <ul class="social">
      <li><a href="http://facebook.com/minhaloja">Facebook</a></li>
      <li><a href="http://twitter.com/minhaloja">Twitter</a></li>
    </ul>
    ```
  - Seletores de atributo (`a[href*="facebook.com"]` e `a[href*="twitter.com"]`) para aplicar as imagens como `background-image`.
  - Esconde o texto dos links usando a técnica clássica de **Image Replacement** (`display: block; width: 36px; height: 36px; text-indent: -9999px;`).

---

### 5. Efeitos CSS3 Avançados, Pseudo-classes e Transições (1,5 ponto)
- [x] **Pseudo-elementos:** Utilização de `::before` nos itens das subcategorias para inserir automaticamente o marcador estético (`content: "▸ ";`).
- [x] **Transições e Efeitos de Hover nos Cards:**
  - Aumento sutil com `transform: scale(1.15);`.
  - Sombra externa destacada com `box-shadow;`.
  - Fundo translúcido com `rgba(255, 255, 255, 0.95);`.
  - Animação suave através de `transition: all 0.5s ease;`.
- [x] **Pseudo-classe `:nth-child`:**
  - Itens pares (`:nth-child(2n):hover`) rotacionam levemente no sentido horário (`rotate(3deg)`).
  - Itens ímpares (`:nth-child(2n+1):hover`) rotacionam no sentido anti-horário (`rotate(-3deg)`).

---

## 🚀 Como Executar

Basta abrir o arquivo `index.html` em qualquer navegador web moderno (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari ou Opera).  
Não é necessária nenhuma instalação adicional nem servidor web, pois o projeto utiliza puramente **HTML5** e **CSS3** estáticos.
