# Bistrô Elegance - Website

Website institucional para o restaurante **Bistrô Elegance**, um estabelecimento sofisticado que oferece uma experiência gastronômica refinada. O projeto apresenta design elegante e minimalista com navegação intuitiva entre três páginas.

## 📋 Páginas

| Página | Arquivo | Seções |
|--------|---------|--------|
| **Home** | `index.html` | Header fixo, Hero, Destaques (3 cards), Sobre, Mapa integrado, Footer |
| **Cardápio** | `cardapio.html` | Hero, Entradas, Pratos Principais, Sobremesas, Chef, Footer |
| **Reservas** | `reservas.html` | Hero, Informações, Formulário de reserva, Footer |

## 🎨 Design System

### Cores

| Variável | Valor | Uso |
|----------|-------|-----|
| `--gold` | `#c8a97e` | Detalhes, botões, ícones |
| `--dark` | `#222222` | Fundos escuros, textos |
| `--light` | `#f8f8f8` | Fundo de seções |
| `--gray` | `#555555` | Textos secundários |

### Tipografia

- **Títulos:** Cormorant Garamond (serifada) — elegância e sofisticação
- **Textos:** Montserrat (sans-serif) — legibilidade e contraste
- Pesos utilizados: Light 300, Regular 400, Medium 500, SemiBold 600, Bold 700

### Componentes

- Botão dourado (`btn-gold`) com hover efeito
- Cards com sombras e zoom em hover
- Linha dourada decorativa (`::after`) abaixo de títulos
- Ícones do Font Awesome 6.5.1

## 🚀 Funcionalidades

### Navegação
- **Header fixo** com logotipo e navegação responsiva
- **Menu mobile** com animação via botão hambúrguer
- Navegação entre páginas (Home, Cardápio, Reservas)
- Links internos para seções Sobre e Contato

### Interação
- **Botão flutuante "Reserva"** — acesso rápido à página de reservas (fixo no canto inferior)
- **Botão "Voltar ao topo"** — aparece com fade-in ao scroll ultrapassar 300px
- **Scroll reveal** — animações de entrada nas seções ao rolar a página (Intersection Observer API)
- Efeitos hover em cards, botões e links

### Página de Reservas
- Formulário completo com campos: nome, e-mail, telefone, data, horário, número de pessoas e observações
- Validação HTML5 nos campos obrigatórios
- Design responsivo com duas colunas (informações + formulário)
- Confirmação via `alert()` ao enviar

### Mapa
- Mapa interativo incorporado via OpenStreetMap
- Exibido no rodapé da página inicial
- Carregamento lazy para performance

## 🛠️ Tecnologias

### Frontend
- **HTML5** — Estrutura semântica e acessível
- **CSS3** — Estilização avançada com:
  - Variáveis CSS customizadas
  - Flexbox para layouts responsivos
  - Transições e animações suaves
  - Design responsivo com 3 breakpoints

### Bibliotecas e Recursos Externos
- [Font Awesome 6.5.1](https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css) — Ícones
- [Google Fonts](https://fonts.google.com/) — Cormorant Garamond + Montserrat
- [Unsplash](https://unsplash.com/) — Imagens reais de alta qualidade
- [OpenStreetMap](https://www.openstreetmap.org/) — Mapa interativo

### APIs Web
- **Intersection Observer API** — Detecta visibilidade de elementos para scroll reveal
- **scroll-behavior: smooth** — Rolagem suave âncoras

## 📐 Responsividade

O layout se adapta a três breakpoints principais:

| Breakpoint | Alvo | Ajustes |
|-----------|------|---------|
| 1024px | Tablets paisagem | Hero reduzido, gaps ajustados |
| 768px | Tablets retrato / Mobile grande | Layout empilhado, menu mobile, form em coluna |
| 480px | Smartphones | Padding reduzido, fonte ajustada, botões menores |

## 📁 Estrutura do Projeto

```
/
├── index.html          # Página inicial
├── cardapio.html       # Página do cardápio
├── reservas.html       # Página de reservas
├── style.css           # Estilos globais
├── cardapio.css        # Estilos específicos do cardápio
├── readme.md           # Documentação
└── LICENSE             # Licença MIT
```

## 📄 Licença

Distribuído sob licença MIT. Veja `LICENSE` para mais informações.

---

Desenvolvido como projeto de estudo de desenvolvimento web.
