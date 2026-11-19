# DevHub — Aplicação com Tailwind CSS & Spectra Design System

Projeto acadêmico aplicando integralmente o **Spectra Design System** sobre **Tailwind CSS v4** na plataforma **DevHub — Portal de Trilhas & Projetos Tech**, utilizando mais de **30 classes utilitárias distintas** abrangendo cores, tipografia, dimensões, bordas, Flexbox, CSS Grid e responsividade.

---

## Link da Aplicação em Funcionamento

- **Aplicação online (GitHub Pages):** https://ahslammendes.github.io/projeto_em_tailwind_css/Frontend/
- **Repositório GitHub:** https://github.com/ahslammendes/projeto_em_tailwind_css

---

## Componentes do Spectra Design System Aplicados

- **Paleta & Tokens (`@theme`):** Escala customizada `forest-50` (`#f2f8f6`) até `forest-950` (`#0a1814`) combinada com acentos `emerald` e superfícies translúcidas (*light glass* `bg-white/60 backdrop-blur-md` e *dark glass* `bg-forest-950/80 backdrop-blur-2xl`).
- **Tipografia Dual:** Display em **DM Sans** (`font-dm-sans font-light tracking-tighter`), corpo em **System UI** (`font-sans`) e índices/telemetria em **Monospace** (`font-mono`).
- **Navbar adaptativa:** `mix-blend-difference` no topo da página com transição automática para `bg-black/95 backdrop-blur-xl` ao rolar, além de menu mobile em drawer glass.
- **Hero Editorial:** Grade arquitetural de 12 colunas (`opacity-[0.08]`), botão primário com gradiente esmeralda + sheen animado, botão secundário com `--border-gradient`, *Hero Preview Card* com hotspot `animate-ping` e pill `Conectado`, além dos dois cartões *Hero Dark Glass*.
- **Catálogo Interativo de Trilhas:** *Toggle Well* (`bg-forest-900/50`) com filtro funcional por categoria (Todas, Front-end, Back-end, UI/UX) e *Process Cards* com reveal de seta no hover.
- **Application Media Cards + Telemetria:** Grade assimétrica 8/4 com zoom suave (`duration-700`), painel branco elevado (`rounded-[2.5rem]`), 4 *Feature Items* com ícones `solar:*` e overlay de telemetria com gráfico semanal.
- **Marquee Infinito em Duas Linhas:** *Quote Cards* com rolagem contínua (`scroll-left` / `scroll-right`), pausa no hover e máscara lateral (`mask-gradient-x`).
- **Planos com Billing Toggle:** Alternador interativo Mensal / Anual (`-20%`), 3 *Plan Cards* com destaque elevado no plano central (`Mais Popular`).
- **Documentação + FAQ Accordion:** *Documentation Card* com selo `V 4.0 Docs` e acordeão com transição suave em CSS Grid (`grid-rows-[0fr]` → `grid-rows-[1fr]`) e ícones `lucide:plus`/`lucide:minus`.
- **Closing Band & Footer Elevado:** Formulário de inscrição com glow esmeralda superior e rodapé branco elevado com marca d'água tipográfica, colunas numeradas (`01`, `02`, `03`) e ícones sociais `ri:*`.
- **Ícones & Animações:** Pacotes Iconify (`lucide`, `solar` linear e `ri`), `IntersectionObserver` (`.reveal-on-scroll`), `animate-pulse`, `animate-ping` e microinterações em hover.

---

## Prints da Aplicação e do Código-Fonte

### 1. Aplicação Executando — Desktop (`1440px`)

![Aplicação DevHub com Spectra Design System em Desktop](docs/prints/app-desktop.png)

### 2. Aplicação Executando — Mobile Responsivo (`520px`)

![Aplicação DevHub com Spectra Design System em Mobile](docs/prints/app-mobile.png)

### 3. Código-Fonte (`index.html`)

![Código-fonte do projeto com Spectra Design System e Tailwind CSS](docs/prints/codigo-fonte.png)

---

## Tabela de Classes Utilitárias Utilizadas (35 Classes)

Abaixo estão documentadas **35 classes utilitárias distintas** efetivamente utilizadas no arquivo [`Frontend/index.html`](Frontend/index.html), cobrindo todas as 7 categorias exigidas:

| # | Classe Utilitária | Categoria | Finalidade |
| :-: | :--- | :--- | :--- |
| 1 | `bg-forest-950` | **Cores** | Define o fundo verde-escuro profundo (`#0a1814`) nas bandas escuras e superfícies glass. |
| 2 | `bg-forest-50` | **Cores** | Aplica o fundo claro característico (`#f2f8f6`) da paleta Spectra nas seções claras. |
| 3 | `bg-emerald-500` | **Cores** | Aplica a cor de destaque esmeralda em selos (*Mais Popular*), ícones de check e barras. |
| 4 | `text-forest-950` | **Cores** | Define a cor principal dos títulos e textos de alto contraste sobre fundos claros. |
| 5 | `text-emerald-400` | **Cores** | Destaca trechos de títulos, índices e indicadores de status sobre fundos escuros. |
| 6 | `text-4xl` | **Tipografia** | Define tamanho de fonte grande (`2.25rem`) para títulos de seção e métricas de destaque. |
| 7 | `text-sm` | **Tipografia** | Define tamanho de fonte reduzido (`0.875rem`) para descrições, links e itens de lista. |
| 8 | `font-light` | **Tipografia** | Aplica peso tipográfico leve (`300`) característico dos títulos display em DM Sans. |
| 9 | `tracking-tighter` | **Tipografia** | Aproxima o espaçamento entre letras nos títulos grandes para estética editorial. |
| 10 | `leading-relaxed` | **Tipografia** | Aumenta a altura de linha (`1.625`) em parágrafos para leitura confortável. |
| 11 | `min-h-screen` | **Dimensões** | Garante que o corpo e a seção Hero ocupem no mínimo 100% da altura da tela. |
| 12 | `max-w-6xl` | **Dimensões** | Limita a largura máxima do conteúdo principal (`72rem`) mantendo proporção equilibrada. |
| 13 | `w-full` | **Dimensões** | Faz o elemento ocupar 100% da largura disponível do seu container pai. |
| 14 | `p-6` | **Dimensões** | Aplica espaçamento interno uniforme (`1.5rem`) nos cartões e containers principais. |
| 15 | `mx-auto` | **Dimensões** | Centraliza horizontalmente os containers na tela utilizando margens automáticas. |
| 16 | `border` | **Bordas** | Adiciona borda sólida de `1px` ao redor de cartões, botões, pills e painéis. |
| 17 | `border-white/10` | **Bordas** | Aplica borda translúcida sutil (*hairline*) em cartões de vidro escuro e controles. |
| 18 | `rounded-3xl` | **Bordas** | Aplica cantos amplamente arredondados (`1.5rem`) nos cartões de trilha e mídia. |
| 19 | `rounded-full` | **Bordas** | Arredonda totalmente botões pílula, avatares, badges de status e chips de ícone. |
| 20 | `shadow-2xl` | **Bordas** | Aplica sombra profunda para destacar painéis elevados e cartões glassmorphism. |
| 21 | `flex` | **Flexbox** | Ativa o modelo de layout Flexbox no container. |
| 22 | `flex-col` | **Flexbox** | Organiza os elementos filhos empilhados verticalmente (coluna). |
| 23 | `items-center` | **Flexbox** | Alinha os elementos filhos ao centro no eixo transversal. |
| 24 | `justify-between` | **Flexbox** | Distribui os elementos nas extremidades com espaço igual entre eles (navbar, cards, footer). |
| 25 | `gap-4` | **Flexbox** | Define espaçamento consistente (`1rem`) entre elementos filhos flexíveis. |
| 26 | `grid` | **Grid** | Ativa o modelo de layout CSS Grid no container. |
| 27 | `grid-cols-1` | **Grid** | Define a grade com 1 coluna por padrão (abordagem *mobile-first*). |
| 28 | `gap-6` | **Grid** | Define espaçamento (`1.5rem`) entre linhas e colunas da grade de cartões e seções. |
| 29 | `col-span-1` | **Grid** | Faz o item ocupar 1 coluna na grade base em telas pequenas. |
| 30 | `place-items-center` | **Grid** | Centraliza ícones nos eixos horizontal e vertical dentro de chips circulares em Grid. |
| 31 | `sm:flex-row` | **Responsividade** | Altera a direção do Flexbox para horizontal em telas a partir de `640px`. |
| 32 | `sm:text-5xl` | **Responsividade** | Aumenta o tamanho do título principal para `3rem` em telas `≥ 640px`. |
| 33 | `md:grid-cols-2` | **Responsividade** | Expande a grade de trilhas e recursos para 2 colunas em tablets (`≥ 768px`). |
| 34 | `lg:grid-cols-3` | **Responsividade** | Expande a grade de trilhas e planos para 3 colunas em desktops (`≥ 1024px`). |
| 35 | `lg:col-span-7` | **Responsividade** | Faz blocos de destaque (Hero, glass stat card e FAQ) ocuparem 7 de 12 colunas em `≥ 1024px`. |

---

## Estrutura do Repositório

```text
projeto_em_tailwind_css/
├── Frontend/
│   ├── index.html                      # Aplicação completa (Tailwind CSS v4 + Spectra Design System)
│   └── assets/
│       ├── img/                        # Imagens e avatares do Spectra Design System
│       └── js/
│           ├── iconify-preload.js      # Preload dos ícones Lucide, Solar e Remix Icon
│           ├── unicorn-scene.js        # Cena WebGL animada (Aurora + Voronoi + GlyphDither)
│           └── unicornStudio.umd.js    # Runtime WebGL Unicorn Studio
├── docs/
│   └── prints/
│       ├── app-desktop.png             # Print da aplicação em execução (Desktop)
│       ├── app-mobile.png              # Print da aplicação em execução (Mobile)
│       └── codigo-fonte.png            # Print do código-fonte HTML + Tailwind CSS
└── README.md                           # Documentação da entrega, prints e tabela de classes
```

---

## Como Executar Localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/ahslammendes/projeto_em_tailwind_css.git
   ```
2. Acesse a pasta `Frontend/` e abra o arquivo `Frontend/index.html` diretamente no navegador (ou utilize a extensão *Live Server* no VS Code).
