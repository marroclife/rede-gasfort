# Benchmark UX/UI — Concorrentes Rede Gasfort

**Data:** 2026-06-15  
**Concorrentes analisados:**
- Shell Brasil — https://www.shell.com.br/motoristas/postos-shell.html
- Ipiranga Brasil — https://www.ipiranga.com.br/wps/portal/pt-br/ipiranga/inicio

**Método:** screenshots desktop/mobile via Playwright + análise de HTML/JSON da SPA do Shell + análise visual via modelo de visão.

---

## 1. Visão Geral

| Aspecto | Shell Brasil | Ipiranga Brasil |
|---------|--------------|-----------------|
| **Modelo de site** | SPA headless baseada em AEM (Adobe Experience Manager) + JSON | Portal corporativo em IBM WebSphere Portal (WCM) |
| **Estilo visual** | Minimalista, corporativo global, muito espaço em branco | Landing page vertical, alto impacto visual, blocos coloridos |
| **Tom de voz** | Tecnologia, qualidade, confiança | "Parada completa", jornada, energia |
| **Localizador de postos** | Página dedicada, mas não é o foco da home | Botão fixo no header "Encontrar posto" |
| **App móvel** | Não evidenciado na home | Botão "Baixe o app" fixo no header |
| **Foco de conversão** | Conteúdo institucional + cards de destaque | Download do app + captura de lead + encontrar posto |

---

## 2. Shell Brasil — Análise Detalhada

### 2.1 Estrutura técnica (do `postos-shell.model.json`)

```
Page: Postos Shell
├── Container.Raw (Metadata, ContentOwner, Header)
│   └── Breadcrumb
├── Container.Main
│   ├── Container.Section
│   │   ├── PageHeader — "Postos Shell"
│   │   ├── PromoSimple.Text — "Veja aqui"
│   │   └── PromoCard — "Sobre os postos Shell"
│   └── Container.Section — "Destaques"
│       ├── PromoCard — "Promoções e ações"
│       ├── PromoCard — "Combustíveis"
│       ├── PromoCard — "Lojas Shell Select"
│       └── Experience Fragment
└── Container.Footer
```

### 2.2 Desktop — observações visuais
- **Header:** duas camadas (barra utilitária + navegação principal). Logo Shell, menus suspensos, ícone de busca.
- **Hero:** imagem larga com recorte diagonal dinâmico, transição para conteúdo.
- **Tipografia:** fonte própria `shell-typeface-la-heavy`, sans-serif geométrica, pesada.
- **Cores:** amarelo Shell como cor primária de destaque, vermelho sutil, branco/cinza neutros.
- **Componentes:** breadcrumbs, cards promocionais com imagem + título + CTA, banner de cookies.
- **Página linear:** poucos elementos por dobra, muito whitespace.

### 2.3 Mobile — observações visuais
- Menu hambúrguer visível.
- **Problema crítico:** o banner de cookies ocupa ~80% da primeira tela, bloqueando o conteúdo principal.
- Breadcrumbs adaptados; header compacto.
- Ação de "encontrar posto" não é óbvia na primeira dobra.

### 2.4 O que funciona bem
| + | Explicação |
|---|------------|
| Branding consistente | Cor, tipografia e tom globais são impecáveis. |
| Limpeza visual | Pouca poluição; foco no conteúdo. |
| Breadcrumbs | Ótima orientação de navegação em site grande. |
| Imagens de qualidade | Fotos realistas de postos, alta resolução. |
| Hierarquia clara | Título H1 grande, corpo legível, CTAs secundários bem posicionados. |

### 2.5 O que NÃO funciona bem
| − | Explicação |
|---|------------|
| CTA fraco para postos | "Encontrar posto mais próximo" não é destaque; fica escondido no texto. |
| Banner de cookies intrusivo | No mobile, ocupa a tela toda e rouba a primeira impressão. |
| Espaço morto | Excesso de whitespace abaixo do texto introdutório parece página quebrada. |
| Pouca conversão na home | Página é institucional demais; poucos gatilhos de ação. |
| Ausência de utilidades | Não mostra ícones de serviços (wifi, lavagem, etc.) na primeira dobra. |

---

## 3. Ipiranga Brasil — Análise Detalhada

### 3.1 Estrutura técnica (do HTML)

- **Plataforma:** IBM WebSphere Portal (WCM) — portal antigo, URLs complexas (`/wps/portal/...`).
- **Fonte:** Roboto (Google Fonts) — 400, 500, 700.
- **CSS:** tema institucional v4, home.min.css customizado.
- **Frameworks legados:** Dojo, jQuery, qTip.
- **Meta description:** "Abasteça com a qualidade e confiança dos combustíveis Ipiranga. Encontre o posto mais próximo e mantenha-se em movimento!"

### 3.2 Seções principais da homepage (desktop/mobile)
1. **Header** — Logo + menu hambúrguer + CTA "Baixe o app" + "Encontrar posto".
2. **Hero carrossel** — Promoção "Parada Completa" + CTA "Saiba Mais".
3. **Vídeo/bloco preto** — "No posto Ipiranga, a parada é completa.".
4. **Produtos** — Blocos zig-zag: Combustíveis, Ipimax, Original, Ipimax Pro, Lubrificantes.
5. **Conveniência** — Seção amPm.
6. **Saúde na Estrada** — Serviço/parceria.
7. **Carreiras** — "Movimente sua carreira com a Ipiranga".
8. **Localizador** — "Encontre o Posto Ipiranga mais próximo".
9. **B2B** — "A gente completa o seu negócio".
10. **Newsletter** — Formulário com Nome, E-mail, CPF.
11. **Footer** — links legais, redes sociais.

### 3.3 Desktop — observações visuais
- **Alta densidade visual:** cores fortes (amarelo, azul, preto) em seções alternadas.
- **Tipografia:** Roboto, pesos bem distribuídos, títulos grandes.
- **Componentes:** carrossel, blocos de imagem + texto, CTAs com seta, formulário de captura, ícone de acessibilidade (VLibras), widget de suporte.
- **Formas geométricas:** recortes curvos, círculos, transições entre seções.

### 3.4 Mobile — observações visuais
- **Problema:** primeira dobra poluída — banner promocional + aviso de cookies + botão do app competem atenção.
- **Scroll intenso:** transições bruscas de amarelo para azul para preto criam "fadiga visual".
- **Menu hambúrguer:** pouco evidente; navegação fica escondida.
- **Formulário final:** fundo azul escuro + texto amarelo pode cansar na leitura.
- **Carrosséis:** economizam espaço, mas dependem de descoberta.

### 3.5 O que funciona bem
| + | Explicação |
|---|------------|
| Identidade visual forte | Amarelo Ipiranga dominante; reconhecimento instantâneo. |
| Foco em conversão | App, posto e newsletter são CTAs claros e repetidos. |
| Escanabilidade | Títulos grandes e blocos temáticos permitem "scrolar e entender". |
| Jornada do cliente | Narrativa lógica: oferta → produto → conveniência → localizador → lead. |
| Download do app no header | Boa estratégia de levar usuário para o ecossistema digital. |

### 3.6 O que NÃO funciona bem
| − | Explicação |
|---|------------|
| Poluição visual | Primeira dobra mobile congestionada; cookies ocupam muito espaço. |
| Ritmo visual agressivo | Cores muito contrastantes em seções sucessivas cansam. |
| Textos genéricos de CTA | "Saiba Mais" repetido demais; perde SEO e clareza. |
| Formulário pede CPF | Fricção desnecessária para newsletter. |
| Localizador não é hero | Botão "Encontrar posto" está no header, mas não na primeira dobra como elemento principal. |
| Plataforma legada | WCM antigo dificulta performance, SEO e manutenção. |

---

## 4. Análise dos Localizadores de Postos

### 4.1 Ipiranga — Encontre seu posto
**Screenshot:** `ipiranga-localizador.png` (1440x1665 px)

- **Estrutura:** título "Encontre o Posto Ipiranga mais próximo" + campo de busca + botão de geolocalização + filtros + mapa + lista de resultados.
- **Busca:** input simples com placeholder; botão de localização atual.
- **Filtros:** checkbox/switches para serviços (Loja de Conveniência, Troca de Óleo, Posto 24h, etc.).
- **Resultados:** cards laterais com nome do posto, endereço, distância, serviços e botão "Traçar rota".
- **Mapa:** ocupando a maior parte da tela à direita; marcações de postos.
- **Cores:** azul Ipiranga para primários, amarelo para destaques, fundo claro.

**Veredito:** funcional, mas a tela pode ficar sobrecarregada com filtros + mapa + lista. Em mobile, a alternância mapa/lista exige bom controle de abas.

### 4.2 Shell — Encontre um posto Shell
**Screenshot:** `shell-localizador.png` (1440x1528 px)

- **Estrutura:** página limpa com campo de busca + mapa + cards de resultado.
- **Visual:** mais minimalista que a Ipiranga; menos filtros visíveis.
- **Cores:** amarelo Shell, branco, cinza.
- **Resultados:** lista compacta ao lado/esquerda do mapa.

**Veredito:** design mais enxuto, mas pode sacrificar filtros úteis. Ação principal clara: buscar.

---

## 5. Padrões Comuns entre Concorrentes

| Padrão | Shell | Ipiranga | Recomendação para Gasfort |
|--------|-------|----------|---------------------------|
| Hero com imagem de posto/carro | ✅ | ✅ | ✅ — usar fotos reais dos postos Gasfort |
| CTA "Encontrar posto" em destaque | ⚠️ (fraco) | ⚠️ (no header) | ✅ — botão principal na hero, sticky ou header |
| Download do app | ❌ evidência | ✅ header | ✅ — destacar app com QR code |
| Cards de produtos/serviços | ✅ | ✅ | ✅ — combustíveis, conveniência, troca de óleo, lavagem |
| Localizador com mapa | ✅ | ✅ | ✅ — integrar planilha existente + Google Maps |
| Filtros de serviços no localizador | ⚠️ | ✅ | ✅ — filtro por cidade, bandeira, serviço |
| Newsletter/lead capture | ❌ | ✅ | ⚠️ — pode usar para empresas/frotas |
| Cookie banner agressivo | ⚠️ (intrusivo) | ⚠️ (intrusivo) | ✅ — banner mínimo na base |
| Acessibilidade | ❌ evidência | ✅ VLibras | ✅ — incluir acessibilidade básica |
| Breadcrumbs | ✅ | ⚠️ | ✅ — para páginas internas |
| Footer robusto | ✅ | ✅ | ✅ — links úteis, redes, SAC |

---

## 6. Oportunidades de Diferenciação para Rede Gasfort

Com base nos gaps observados, o mockup do site Gasfort pode se destacar em:

### 6.1 Primeira dobra (Hero)
- **Título forte:** "30 anos abastecendo o Rio Grande do Sul" ou "A rede que cresce com você".
- **Dois CTAs principais:**
  1. "Encontrar posto mais próximo" (ação de consumidor)
  2. "Baixar o App Gasfort" (fidelidade)
- **Foto real de um posto Gasfort** (a confirmar com cliente; usar placeholder genérico por enquanto).
- **Destaque para múltiplas bandeiras:** "Gasfort, Shell, Ipiranga, Charrua e Santa Lúcia".

### 6.2 Localizador
- **Integrar a planilha Google Sheets** já existente.
- **Filtros por:** cidade, bandeira, serviço (conveniência, troca de óleo, lavagem, restaurante, 24h).
- **Card de resultado:** logo da bandeira, nome, endereço, serviços em pills, botão "Traçar rota".
- **Mobile-first:** alternância suave mapa/lista; geolocalização.

### 6.3 Seções institucionais
- **Linha do tempo 1995→2024→hoje** com a transição Assunção → Gasfort.
- **Números/destaques:** 30+ anos, 25 filiais, 12+ cidades, 5 bandeiras.
- **Serviços:** ícones para cada serviço (já mapeados no site atual).

### 6.4 App e fidelidade
- Destaque claro para download iOS/Android.
- Mencionar: descontos, cashback, troca de pontos por produtos.

### 6.5 Cotação empresas / frotas
- CTA separado para B2B; form de captura.

### 6.6 Design system
- **Cores:** manter amarelo Gasfort `#FFC400` como cor primária; cinza escuro `#1C1C1E`; fundo cinza claro `#E4E4E7`.
- **Tipografia:** Inter (já usada no linktree) ou evoluir para "Plus Jakarta Sans" para mais peso institucional.
- **Componentes:** cards arredondados (squircle 22px), sombras suaves, animações sutis.
- **Evitar:** banners de cookies gigantes, transições de cores agressivas, CTAs genéricos repetidos.

---

## 7. Lições Aprendidas — Do's and Don'ts

### ✅ Fazer (inspirado no que funciona)
1. Manter identidade visual forte e consistente.
2. Hero com proposta de valor clara + foto de posto.
3. CTA "Encontrar posto" em destaque na primeira dobra e no header.
4. Download do app visível.
5. Localizador funcional com filtros por cidade/serviço.
6. Cards de serviços com ícones claros.
7. Footer com links úteis e redes sociais.
8. Mobile-first: botões grandes, scroll fluido, pouca poluição.

### ❌ Evitar (inspirado nos erros dos concorrentes)
1. Banner de cookies ocupando a tela toda no mobile.
2. Paleta visual agressiva que cansa ao scrollar.
3. CTAs genéricos tipo "Saiba Mais" em todos os blocos.
4. Formulários que pedem dados sensíveis demais logo de cara.
5. Páginas institucionais sem ação clara.
6. Sites monolíticos lentos (WCM); preferir stack leve (Next.js/Astro + planilha).

---

## 8. Screenshots Coletados

| Arquivo | Dimensões | Tamanho | Conteúdo |
|---------|-----------|---------|----------|
| `shell-postos.png` | 1440 x 2540 | 372 KB | Página "Postos Shell" desktop |
| `shell-postos-mobile.png` | 390 x 3827 | 87 KB | Versão mobile da mesma página |
| `shell-localizador.png` | 1440 x 1528 | 86 KB | Localizador de postos Shell |
| `ipiranga-home.png` | 1440 x 8166 | 1.2 MB | Homepage Ipiranga desktop |
| `ipiranga-mobile.png` | 390 x 8380 | 487 KB | Homepage Ipiranga mobile |
| `ipiranga-localizador.png` | 1440 x 1665 | 543 KB | Localizador de postos Ipiranga |
| `ipiranga-combustiveis.png` | 1440 x 900 | 74 KB | Página de combustíveis Ipiranga (404) |

**Local no workspace:** `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/competidores/`

---

## 9. Próximos Passos Recomendados

1. Definir arquitetura de informação do novo site Gasfort.
2. Criar wireframes de baixa fidelidade (desktop + mobile).
3. Escolher stack técnica leve (recomendação: Next.js/Astro + Tailwind + integração com planilha CSV existente).
4. Produzir mockup de alta fidelidade em Figma/HTML.
5. Validar com Marroc e depois com o cliente.

---

*Benchmark produzido por Nexo (Operator).*
