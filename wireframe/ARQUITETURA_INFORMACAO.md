# Arquitetura de Informação — Site Rede Gasfort

**Data:** 2026-06-15  
**Baseado em:** Brief da Rede Gasfort + Benchmark Shell/Ipiranga

---

## 1. Estrutura de Navegação

```
Home
├── Sobre a Gasfort (história / timeline)
├── Nossos Postos
│   ├── Localizador de Postos (com mapa + filtros)
│   ├── Lista de Filiais
│   └── Detalhe da Filial
├── Serviços
│   ├── Combustíveis
│   ├── Loja de Conveniência
│   ├── Troca de Óleo
│   ├── Lavagem / Lava-Rápido
│   ├── Restaurante / Lanchonete
│   └── Fidelidade (App)
├── App Gasfort
├── Para Empresas (cotação / frotas)
├── Trabalhe Conosco
├── Blog / Novidades
└── Contato
```

---

## 2. Mapa de Páginas e Seções

### 2.1 Home
**Objetivo:** Converter visitante em ação (encontrar posto ou baixar app).

| Ordem | Seção | Função |
|-------|-------|--------|
| 1 | Header fixo | Logo, menu, CTA "Encontrar Posto", botão App |
| 2 | Hero | Imagem de posto, headline 30 anos, 2 CTAs |
| 3 | Nossos Números | 30+ anos, 25+ postos, 12+ cidades, 5 bandeiras |
| 4 | Nossos Postos (destaque) | Cards das principais cidades + CTA para localizador |
| 5 | Serviços | Ícones dos serviços oferecidos |
| 6 | App Gasfort | Download iOS/Android + benefícios |
| 7 | História / Timeline | 1995 → 2024 → hoje |
| 8 | Cotação para Empresas | CTA B2B |
| 9 | Depoimentos / Confiança | (texto mockup) |
| 10 | Footer | Contato, redes, links úteis, SAC |

### 2.2 Nossos Postos / Localizador
**Objetivo:** Achar o posto mais próximo com filtros.

| Ordem | Componente |
|-------|------------|
| 1 | Título + subtítulo |
| 2 | Campo de busca + botão geolocalização |
| 3 | Filtros: cidade, bandeira, serviço |
| 4 | Mapa (Google Maps) |
| 5 | Lista de cards de resultado |
| 6 | Card detalhado ao clicar (nome, endereço, serviços, rota) |

### 2.3 Sobre
**Objetivo:** Contar a história e gerar confiança.

| Ordem | Componente |
|-------|------------|
| 1 | Hero institucional |
| 2 | Texto sobre a rede |
| 3 | Timeline interativa |
| 4 | Missão / Visão / Valores (mockup) |
| 5 | Nossas bandeiras |

### 2.4 Serviços
**Objetivo:** Apresentar o ecossistema de serviços.

| Ordem | Componente |
|-------|------------|
| 1 | Hero serviços |
| 2 | Grid de serviços com ícones |
| 3 | Destaque App / Fidelidade |
| 4 | CTA para encontrar posto |

### 2.5 App
**Objetivo:** Levar para download.

| Ordem | Componente |
|-------|------------|
| 1 | Hero com mockup de celular |
| 2 | Benefícios: descontos, cashback, pontos |
| 3 | QR codes / badges App Store + Play Store |

### 2.6 Para Empresas
**Objetivo:** Captar leads B2B/frotas.

| Ordem | Componente |
|-------|------------|
| 1 | Hero B2B |
| 2 | Benefícios para frotas |
| 3 | Formulário de cotação |

### 2.7 Trabalhe Conosco
**Objetivo:** Recrutamento.

| Ordem | Componente |
|-------|------------|
| 1 | Cultura Gasfort (mockup) |
| 2 | Vagas em aberto (mockup) |
| 3 | Formulário |

---

## 3. Componentes Reutilizáveis

- `Header` — fixo, com scroll behavior
- `Hero` — imagem + headline + 2 CTAs
- `SectionTitle` — título + subtítulo centralizado
- `StatsBar` — 4 números em destaque
- `CityCard` — imagem, cidade, quantidade de postos, CTA
- `ServiceCard` — ícone, título, descrição
- `StationCard` — logo bandeira, nome, endereço, serviços, botão rota
- `TimelineItem` — ano, título, descrição
- `AppCTA` — celular mockup + badges
- `Footer` — 4 colunas + redes + copyright

---

## 4. Decisões de UX

- **Mobile-first:** todos os componentes priorizam telas pequenas.
- **CTA duplo fixo no header:** "Encontrar Posto" (primário) e "Baixar App" (secundário).
- **Cookie banner minimalista:** barra na base, não modal central.
- **Scroll suave:** evitar transições de cores agressivas.
- **Acessibilidade:** contraste AAA, alt texts, foco visível.
- **Performance:** imagens otimizadas, sem frameworks pesados.

---

## 5. Wireframes a serem gerados

1. `wireframe-home-desktop.html`
2. `wireframe-home-mobile.html`
3. `wireframe-localizador-desktop.html`
4. `wireframe-localizador-mobile.html`

*Textos em placeholder/marcado como [TEXTO MOCKUP].*
