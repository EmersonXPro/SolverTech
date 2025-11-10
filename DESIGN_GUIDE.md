# SolverTech - Design Guide

## Visão Geral

O SolverTech adota uma linguagem visual dinâmica, inovadora e acessível que reflete a natureza educacional e técnica da plataforma. O design enfatiza clareza, precisão e inspiração através de uma paleta de cores vibrante e tipografia moderna.

## Paleta de Cores

### Cores Primárias

A paleta primária do SolverTech é baseada em tons de roxo e azul, transmitindo criatividade, inteligência e inovação.

| Cor | Código HEX | Código RGB | Uso |
|---|---|---|---|
| Roxo Escuro | `#4C1D95` | rgb(76, 29, 149) | Fundo principal, backgrounds |
| Roxo Médio | `#7C3AED` | rgb(124, 58, 237) | Botões primários, destaques |
| Roxo Claro | `#A78BFA` | rgb(167, 139, 250) | Hover states, elementos secundários |
| Azul Profundo | `#1E3A8A` | rgb(30, 58, 138) | Backgrounds complementares |

### Cores Secundárias

Cores de suporte para estados, mensagens e elementos de interface.

| Cor | Código HEX | Uso |
|---|---|---|
| Verde Sucesso | `#10B981` | Respostas corretas, status ativo |
| Amarelo Aviso | `#FBBF24` | Avisos, problemas em progresso |
| Vermelho Erro | `#F87171` | Erros, respostas incorretas |
| Cinza Neutro | `#9CA3AF` | Texto secundário, bordas |

### Cores de Tema

#### Modo Claro

```css
--background: #FFFFFF;
--foreground: #1F2937;
--primary: #7C3AED;
--primary-foreground: #FFFFFF;
--secondary: #F3F4F6;
--secondary-foreground: #374151;
--accent: #4C1D95;
--accent-foreground: #FFFFFF;
```

#### Modo Escuro

```css
--background: #1F2937;
--foreground: #F9FAFB;
--primary: #7C3AED;
--primary-foreground: #1F2937;
--secondary: #374151;
--secondary-foreground: #F9FAFB;
--accent: #A78BFA;
--accent-foreground: #1F2937;
```

#### Modo AMOLED (Escuro Extremo)

```css
--background: #000000;
--foreground: #FFFFFF;
--primary: #7C3AED;
--primary-foreground: #000000;
--secondary: #111827;
--secondary-foreground: #FFFFFF;
--accent: #A78BFA;
--accent-foreground: #000000;
```

## Tipografia

### Fontes

A plataforma utiliza a família de fontes **Poppins** do Google Fonts para uma aparência moderna e amigável.

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap');

font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

### Escala Tipográfica

| Elemento | Tamanho | Peso | Altura da Linha |
|---|---|---|---|
| Heading 1 (H1) | 52px | 800 | 1.2 |
| Heading 2 (H2) | 40px | 700 | 1.25 |
| Heading 3 (H3) | 32px | 700 | 1.3 |
| Heading 4 (H4) | 24px | 600 | 1.35 |
| Body Large | 18px | 500 | 1.6 |
| Body Regular | 16px | 400 | 1.6 |
| Body Small | 14px | 400 | 1.5 |
| Caption | 12px | 500 | 1.4 |

## Componentes Visuais

### Botões

**Botão Primário** - Ação principal, chamada para ação

- Cor de fundo: Roxo Médio (#7C3AED)
- Cor do texto: Branco
- Padding: 14px 28px
- Border Radius: 10px
- Transição: 200ms
- Efeito: Elevação ao hover

**Botão Secundário** - Ações alternativas

- Cor de fundo: Roxo Claro (#A78BFA)
- Cor do texto: Branco
- Padding: 14px 28px
- Border Radius: 10px

**Botão Outline** - Ações menos importantes

- Cor de fundo: Transparente
- Cor da borda: Roxo Médio (#7C3AED)
- Cor do texto: Roxo Médio
- Padding: 14px 28px
- Border Radius: 10px

### Cards de Problema

Os cards apresentam problemas de forma clara e atrativa.

- Cor de fundo: Branco (modo claro) ou #2D3748 (modo escuro)
- Borda: 2px sólida em Roxo Claro (#A78BFA)
- Border Radius: 12px
- Padding: 24px
- Box Shadow: 0 4px 12px rgba(124, 58, 237, 0.15)
- Transição ao hover: borda mais brilhante, elevação

### Inputs e Textareas

Campos de entrada mantêm consistência visual com a paleta.

- Cor de fundo: Branco (modo claro) ou #1F2937 (modo escuro)
- Borda: 2px sólida em Cinza Neutro (#9CA3AF)
- Borda ao foco: 2px sólida em Roxo Médio (#7C3AED)
- Border Radius: 10px
- Padding: 12px 16px
- Transição: 150ms

### Badges de Status

Indicadores de status das soluções.

| Status | Cor de Fundo | Cor do Texto |
|---|---|---|
| Correto | Verde Sucesso (#10B981) | Branco |
| Incorreto | Vermelho Erro (#F87171) | Branco |
| Em Progresso | Amarelo Aviso (#FBBF24) | Preto |
| Salvo | Roxo Médio (#7C3AED) | Branco |

## Espaçamento

A plataforma utiliza um sistema de espaçamento baseado em múltiplos de 4px para consistência.

| Valor | Pixels | Uso |
|---|---|---|
| xs | 4px | Espaçamento mínimo |
| sm | 8px | Espaçamento pequeno |
| md | 16px | Espaçamento padrão |
| lg | 24px | Espaçamento grande |
| xl | 32px | Espaçamento extra grande |
| 2xl | 48px | Espaçamento duplo |

## Sombras

As sombras adicionam profundidade e hierarquia visual com tons roxos.

| Nível | CSS | Uso |
|---|---|---|
| Sombra Pequena | `0 2px 4px rgba(124, 58, 237, 0.08)` | Elementos sutis |
| Sombra Média | `0 4px 12px rgba(124, 58, 237, 0.15)` | Cards, inputs |
| Sombra Grande | `0 10px 20px rgba(124, 58, 237, 0.2)` | Modais, dropdowns |
| Sombra Extra | `0 20px 40px rgba(124, 58, 237, 0.25)` | Overlays, popovers |

## Ícones

Todos os ícones utilizam a biblioteca **Lucide React** para consistência.

- Tamanho padrão: 24px
- Tamanho pequeno: 16px
- Tamanho grande: 32px
- Tamanho extra grande: 48px
- Cor: Roxo Médio (#7C3AED) ou herda do contexto

## Animações

As animações são fluidas e inspiradoras, melhorando a experiência de resolução.

| Tipo | Duração | Easing |
|---|---|---|
| Hover | 200ms | ease-in-out |
| Fade | 300ms | ease-in-out |
| Slide | 300ms | ease-out |
| Scale | 250ms | cubic-bezier(0.34, 1.56, 0.64, 1) |
| Bounce | 400ms | cubic-bezier(0.68, -0.55, 0.265, 1.55) |

## Responsividade

A plataforma é totalmente responsiva, otimizada para todos os dispositivos.

| Breakpoint | Largura | Uso |
|---|---|---|
| Mobile | < 640px | Telefones |
| Tablet | 640px - 1024px | Tablets |
| Desktop | > 1024px | Computadores |
| Wide | > 1280px | Monitores grandes |

## Acessibilidade

Todos os elementos visuais mantêm contraste adequado para acessibilidade WCAG AA.

- Contraste mínimo de texto: 4.5:1 para texto normal
- Contraste mínimo de texto: 3:1 para texto grande
- Foco visível em todos os elementos interativos
- Suporte para modo de alto contraste
- Ícones acompanhados de texto descritivo

## Padrões de Interface

### Solver Interface

A interface do solver apresenta um layout split com entrada à esquerda e solução à direita, otimizado para resolução de problemas.

### Dashboard

O dashboard mostra histórico de problemas, estatísticas e recomendações com cards e gráficos interativos.

### Leaderboard

Exibe ranking de usuários com avatares, pontos e badges em uma tabela clara e visualmente atrativa.

### Seção de Depoimentos

Apresenta depoimentos de usuários em cards com foto, nome, especialidade e citação destacada.

---

*Guia de Design preparado por Manus AI - Última atualização: Novembro 2025*
