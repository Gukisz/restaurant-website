<div align="center">
  <h1>Bistrô Elegance</h1>
  <p><strong>Website Institucional para Restaurante Sofisticado</strong></p>
  <p>
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
    <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
    <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="MIT License">
  </p>
</div>

---

## Sobre

O **Bistrô Elegance** é um website institucional para um restaurante sofisticado, desenvolvido com HTML5, CSS3 e JavaScript puros. O projeto apresenta design elegante e minimalista com navegação intuitiva entre três páginas, animações suaves e experiência do usuário refinada.

## 📄 Páginas

| Página | Arquivo | Seções |
|--------|---------|--------|
| **Home** | `index.html` | Header fixo, Hero com parallax, Destaques (3 cards), Sobre, Mapa interativo, Footer |
| **Cardápio** | `cardapio.html` | Hero, Entradas, Pratos Principais, Sobremesas, Chef, Footer |
| **Reservas** | `reservas.html` | Hero, Informações, Formulário de reserva completo, Footer |

## ✨ Funcionalidades

### Navegação
- **Header fixo** com logotipo e navegação responsiva entre Home, Cardápio, Reservas, Sobre e Contato
- **Menu mobile** com animação via botão hambúrguer (toggle `nav-active`)
- Links internos suaves para seções Sobre e Contato

### Interação
- **Botão flutuante "Reserva"** — acesso rápido fixo no canto inferior direito com hover animado
- **Botão "Voltar ao topo"** — aparece com fade-in ao scroll ultrapassar 300px
- **Scroll reveal** — animações de entrada nas seções via Intersection Observer API
- **Cards com zoom** — imagem amplia 108% no hover com transição suave
- **Botões com elevação** — `translateY(-3px)` + sombra no hover
- **Navegação suave** — `scroll-behavior: smooth` para âncoras internas

### Página de Reservas
- Formulário completo com validação HTML5: nome, e-mail, telefone, data, horário (select), número de pessoas e observações
- Layout em duas colunas (informações à esquerda, formulário à direita)
- Confirmação via `alert()` ao submeter

### Mapa
- **OpenStreetMap** interativo incorporado no rodapé da página inicial
- Carregamento lazy (`loading="lazy"`) para performance
- Dimensões 100% x 300px

### Destaques Técnicos
- **HTML5 semântico** — estrutura acessível e bem definida
- **CSS3 com variáveis** — `--gold`, `--dark`, `--light`, `--gray` para consistência visual
- **Flexbox** — layouts responsivos sem depender de frameworks
- **Intersection Observer API** — scroll reveal sem bibliotecas externas
- **Sem dependências pesadas** — apenas Font Awesome e Google Fonts como recursos externos
- **Tipografia elegante** — Cormorant Garamond (títulos) + Montserrat (textos)
- **Imagens reais** — fotos do Unsplash (sem PNGs clipart)

## 🎨 Design System

### Cores

| Variável | Valor | Descrição |
|----------|-------|-----------|
| `--gold` | `#c8a97e` | Detalhes, botões, ícones, linha decorativa |
| `--dark` | `#222222` | Fundos escuros (footer), textos principais |
| `--light` | `#f8f8f8` | Fundo de seções alternadas |
| `--gray` | `#555555` | Textos secundários, descrições |
| `--shadow-sm` | `0 2px 20px rgba(0,0,0,0.05)` | Sombra suave em cards |
| `--shadow-md` | `0 5px 20px rgba(0,0,0,0.05)` | Sombra média em componentes |
| `--shadow-lg` | `0 15px 30px rgba(0,0,0,0.1)` | Sombra forte no hover |

### Tipografia

- **Títulos**: Cormorant Garamond (serifada) — 400, 600, 700 — elegância e sofisticação
- **Textos**: Montserrat (sans-serif) — 300, 400, 500 — legibilidade e contraste
- **Linha dourada decorativa**: `::after` com 2px de altura e 60px de largura abaixo de títulos

### Componentes

| Componente | Características |
|------------|-----------------|
| **Header** | Fixo no topo, glassmorphism (fundo escuro), logo + nav + menu mobile |
| **Hero** | Altura 100vh, gradiente overlay, título grande (4rem), CTA dourado |
| **Cards de destaque** | `--radius` 5px, `--shadow-md`, hover com `translateY(-10px)` + `--shadow-lg` + zoom 108% na imagem |
| **Botão padrão** | Borda dourada 2px, transparente, hover com fundo dourado e elevação |
| **Botão dourado** | Fundo `--gold`, hover escurece (`#b8946a`), usado em formulários |
| **Botão flutuante** | Fixo, arredondado (50px), sombra dourada, hover eleva |
| **Scroll reveal** | `opacity: 0` → `1` + `translateY(40px)` → `0` em 0.8s |
| **Formulários** | Inputs com foco estilizado (borda dourada + ring effect) |

## 📐 Responsividade

O layout se adapta a três breakpoints principais:

| Breakpoint | Alvo | Ajustes |
|-----------|------|---------|
| 1024px | Tablets paisagem | Hero reduzido, gaps ajustados, chef-content empilhado |
| 768px | Tablets retrato / Mobile grande | Layout empilhado (sobre, chef, reservas), menu mobile, form em coluna, float-btn sem texto |
| 480px | Smartphones | Padding reduzido, fonte 2.4rem no hero, botões flutuantes menores |

## 📁 Estrutura do Projeto

```
/
├── index.html          # Página inicial
├── cardapio.html       # Página do cardápio
├── reservas.html       # Página de reservas
├── style.css           # Estilos globais (~1100 linhas)
├── cardapio.css        # Estilos específicos do cardápio
├── readme.md           # Documentação
└── LICENSE             # Licença MIT
```

## 🚀 Como Usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Gukisz/restaurant-website.git
   ```

2. Navegue até a pasta do projeto:
   ```bash
   cd restaurant-website
   ```

3. Abra o arquivo `index.html` no seu navegador:
   ```bash
   open index.html   # macOS
   xdg-open index.html  # Linux
   start index.html  # Windows
   ```

Não é necessário instalar dependências ou configurar servidor — o site é 100% estático com HTML, CSS e JavaScript puros.

## 📄 Licença

Distribuído sob licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais informações.

---

<div align="center">
  <p>Desenvolvido como projeto de estudo de desenvolvimento web</p>
</div>
