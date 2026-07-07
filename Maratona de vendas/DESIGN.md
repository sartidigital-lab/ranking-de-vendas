---
name: Maratona de Vendas Allvino
description: Landing page clara e sofisticada para campanha de vendas, guiada por parreiras, Mendoza e dourado contido.
colors:
  page-bg: "oklch(0.975 0.008 92)"
  wine-ink: "oklch(0.245 0.045 34)"
  allvino-red: "oklch(0.480 0.160 29)"
  copper-foil: "oklch(0.670 0.095 74)"
  label-paper: "oklch(0.930 0.028 85)"
  logo-white: "oklch(0.985 0.000 0)"
  cellar-mist: "oklch(0.430 0.020 58)"
typography:
  display:
    fontFamily: "Marcellus, Georgia, serif"
    fontSize: "clamp(3rem, 8vw, 5.75rem)"
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  headline:
    fontFamily: "Marcellus, Georgia, serif"
    fontSize: "clamp(2rem, 4vw, 3.5rem)"
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: "-0.015em"
  body:
    fontFamily: "Source Sans 3, Verdana, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Source Sans 3, Verdana, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.08em"
rounded:
  sm: "4px"
  md: "8px"
  lg: "12px"
spacing:
  xs: "6px"
  sm: "12px"
  md: "20px"
  lg: "36px"
  xl: "64px"
components:
  button-primary:
    backgroundColor: "{colors.allvino-red}"
    textColor: "{colors.logo-white}"
    rounded: "{rounded.md}"
    padding: "14px 26px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.logo-white}"
    rounded: "{rounded.md}"
    padding: "13px 24px"
  prize-panel:
    backgroundColor: "{colors.wine-ink}"
    textColor: "{colors.logo-white}"
    rounded: "{rounded.lg}"
---

<!-- SEED -->

# Design System: Maratona de Vendas Allvino

## 1. Overview

**Creative North Star: "Pódio em Mendoza"**

O sistema visual deve parecer uma campanha de conquista à luz de vinhedos: parreiras ao fundo, superfícies claras e translúcidas, garrafas reais em primeiro plano, brilho controlado de dourado/cobre e o vermelho Allvino como gesto de ação. A página precisa vender a viagem a Mendoza como prêmio aspiracional sem perder o foco comercial do ranking.

A estética é premium, sofisticada e próxima. Ela rejeita o e-commerce comum, o luxo frio e qualquer vitrine genérica de produtos. O visitante deve sentir que está diante de uma campanha interna importante, feita por uma marca que entende vinho e também entende o ritmo de representantes em disputa.

**Key Characteristics:**
- Fundo claro com imagem de parreira tratada por overlay, sem virar fundo genérico bege.
- Vermelho Allvino reservado para ação, marcação de prêmio e pontos de energia.
- Dourado/cobre usado de forma sofisticada em bordas, detalhes e hierarquia.
- Composição com garrafas grandes, recortes precisos e poucas superfícies em painel.
- Ranking e período da campanha sempre claros, sem deixar a página virar catálogo.

## 2. Colors

A paleta usa uma estratégia restrained/committed: superfícies claras e limpas dominam a arquitetura, enquanto vermelho Allvino e dourado/cobre criam ação, prêmio e sofisticação.

### Primary
- **Allvino Red** (`oklch(0.480 0.160 29)`): cor de ação principal, detalhe da garrafa no logo, marcações de ranking e chamadas de urgência. Usar com texto branco quando for preenchimento.

### Secondary
- **Copper Foil** (`oklch(0.670 0.095 74)`): brilho de cápsula, prêmio, detalhes finos e divisores especiais. Deve sugerir dourado sofisticado, não amarelo chamativo.

### Tertiary
- **Label Paper** (`oklch(0.930 0.028 85)`): superfície de informação curta inspirada nos rótulos dos vinhos. Usar em blocos contidos, nunca como fundo geral sem imagem ou direção.

### Neutral
- **Page BG** (`oklch(0.975 0.008 92)`): fundo claro principal sob overlays de parreira.
- **Wine Ink** (`oklch(0.245 0.045 34)`): texto principal, base escura da logo e contraste premium.
- **Logo White** (`oklch(0.985 0.000 0)`): texto principal sobre fundos escuros e uso do logo.
- **Cellar Mist** (`oklch(0.430 0.020 58)`): texto secundário, metadados e descrições em superfícies claras.

### Named Rules
**The No Generic Wine Beige Rule.** O fundo claro precisa ser sustentado por parreiras, produto e direção; não virar creme/areia padrão.

**The Red Means Action Rule.** Vermelho Allvino é para CTA, disputa, ranking e marca. Se tudo fica vermelho, nada parece importante.

## 3. Typography

**Display Font:** Marcellus, com Georgia como fallback.
**Body Font:** Source Sans 3, com Verdana como fallback.

**Character:** Marcellus aproxima a página das capitulares elegantes do logo e dos rótulos sem cair no excesso ornamental. Source Sans 3 mantém instruções, datas, regras e CTAs nítidos para leitura rápida por representantes.

### Hierarchy
- **Display** (400, `clamp(3rem, 8vw, 5.75rem)`, 0.95): mote principal, chamada de prêmio e momentos de alto impacto. Usar `text-wrap: balance`.
- **Headline** (400, `clamp(2rem, 4vw, 3.5rem)`, 1.05): seções de premiação, mecânica e produtos.
- **Title** (700, 1.125rem, 1.25): títulos de blocos operacionais, ranking e regras.
- **Body** (400, 1rem, 1.65): textos explicativos, com largura máxima de 65-75ch.
- **Label** (700, 0.8125rem, 0.08em): datas, posições, metadados e chips curtos. Usar maiúsculas apenas em rótulos pequenos.

### Named Rules
**The Label Is Not The Voice Rule.** Não repetir pequenos eyebrows em todas as seções. O ritmo vem de escala, imagem e material, não de etiquetas decorativas.

## 4. Elevation

O sistema deve ser quase plano em repouso, com profundidade construída por contraste tonal, recortes de produto, brilho de metal e sombras curtas. Sombras largas em cartões com borda fina devem ser evitadas; a página precisa parecer material e dirigida, não um grid de cards flutuantes.

### Shadow Vocabulary
- **Bottle Lift** (`box-shadow: 0 8px 18px oklch(0 0 0 / 0.32)`): usado em garrafas e elementos que precisam se separar do fundo escuro.
- **Copper Glint** (`box-shadow: 0 0 0 1px oklch(0.720 0.105 62 / 0.35)`): usado para foco, estados selecionados e detalhes de premiação.

### Named Rules
**The Product Carries Depth Rule.** Garrafas e materiais reais criam profundidade; painéis só sustentam informação.

## 5. Components

### Buttons
- **Shape:** retângulos refinados com raio moderado (8px), nunca pílulas grandes.
- **Primary:** fundo Allvino Red com texto Logo White, padding `14px 26px`, peso 700.
- **Hover / Focus:** escurecimento leve, Copper Glint como foco visível e transição curta `180ms` com curva ease-out.
- **Secondary:** transparente, texto Logo White, borda fina em Copper Foil ou Cellar Mist conforme contraste.

### Chips
- **Style:** fundo Wine Ink, texto Cellar Mist, detalhe Copper Foil quando o chip representa período ou posição.
- **State:** chips de ranking ativo podem usar Allvino Red com texto branco; chips informativos ficam discretos.

### Cards / Containers
- **Corner Style:** 8px a 12px no máximo.
- **Background:** Wine Ink para blocos profundos; Label Paper apenas para notas ou mecânica curta.
- **Shadow Strategy:** sem sombra decorativa em painéis comuns; usar contraste e bordas sutis.
- **Border:** 1px no máximo, preferencialmente cobre translúcido ou divisão tonal.
- **Internal Padding:** `clamp(20px, 4vw, 48px)` conforme densidade.

### Inputs / Fields
- **Style:** fundo Bottle Black ou Wine Ink, texto Logo White, borda 1px em Cellar Mist translúcido.
- **Focus:** Copper Glint e borda Copper Foil.
- **Error / Disabled:** erro em Allvino Red com texto claro; desabilitado reduz contraste e não remove rótulo.

### Navigation
- **Style:** logo Allvino em branco, navegação curta e CTA de ranking à direita no desktop. No mobile, priorizar logo, campanha e CTA, evitando menu pesado.

### Prize Feature
- **Style:** seção de prêmio com tratamento mais cinematográfico: garrafa/produto em escala grande, detalhe de Mendoza, posição em destaque e descrição objetiva do benefício.
- **Behavior:** primeiro lugar precisa ter peso visual maior que o segundo, mas ambos devem ser fáceis de comparar.

## 6. Do's and Don'ts

### Do:
- **Do** usar os assets reais da Allvino e dos vinhos como centro da composição.
- **Do** manter o ranking como CTA principal e deixar o período `01/07/2026 a 31/12/2026` legível.
- **Do** usar Bottle Black como fundo dominante para o logo branco e as garrafas parecerem premium.
- **Do** reservar Allvino Red para ação, disputa e detalhe de marca.
- **Do** respeitar WCAG AA, pt-BR e preferência de movimento reduzido.

### Don't:
- **Don't** parecer um e-commerce comum.
- **Don't** criar luxo frio ou distante; a campanha fala com representantes.
- **Don't** produzir uma vitrine genérica de produtos sem narrativa de campanha.
- **Don't** usar fundo creme/sand/bege como solução automática para vinho.
- **Don't** usar gradient text, side-stripe borders, glassmorphism decorativo ou grids de cards idênticos.
- **Don't** colocar texto grande que estoure no mobile; todo título precisa ser testado em larguras estreitas.