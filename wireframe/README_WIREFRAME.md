# Wireframe Rede Gasfort — Resumo

**Data:** 2026-06-15  
**Baseado em:** Brief da empresa + Benchmark UX/UI Shell/Ipiranga

---

## 📁 Arquivos Gerados

| Arquivo | Tipo | Descrição |
|---------|------|-----------|
| `ARQUITETURA_INFORMACAO.md` | Documento | Mapa de navegação e estrutura de páginas |
| `wireframe-home-desktop.html` | HTML navegável | Home desktop (1440px) |
| `wireframe-home-desktop.png` | Screenshot | Home desktop renderizada |
| `wireframe-home-mobile.html` | HTML navegável | Home mobile (390px) |
| `wireframe-home-mobile.png` | Screenshot | Home mobile renderizada |
| `wireframe-localizador-desktop.html` | HTML navegável | Localizador desktop (1440px) |
| `wireframe-localizador-desktop.png` | Screenshot | Localizador desktop renderizado |
| `wireframe-localizador-mobile.html` | HTML navegável | Localizador mobile (390px) |
| `wireframe-localizador-mobile.png` | Screenshot | Localizador mobile renderizado |

---

## 🏗️ Arquitetura Definida

```
Home
├── Sobre a Gasfort
├── Nossos Postos (Localizador + Lista)
├── Serviços
├── App Gasfort
├── Para Empresas
├── Trabalhe Conosco
├── Blog/Novidades
└── Contato
```

---

## 🎨 Decisões de Design

- **Cores:** amarelo Gasfort `#FFC400`, quase-preto `#1C1C1E`, cinza `#E4E4E7`, branco puro.
- **Tipografia:** Inter (escolha do linktree atual) — 400/500/700/800.
- **Estilo visual:** cards arredondados (squircle 22px), sombras suaves, inspirado no linktree atual mas expandido para site institucional.
- **Mobile-first:** todas as páginas priorizam telas pequenas.

---

## 📱 Home — Estrutura

1. **Header fixo** — Logo + menu + CTA "Encontrar Posto" + "Baixar App".
2. **Hero escuro** — Headline "A energia que move o Rio Grande do Sul", 2 CTAs, foto de posto mockup.
3. **Stats bar** — 30+ anos, 25+ postos, 12+ cidades, 5 bandeiras.
4. **Nossos Postos** — Cards de cidades com scroll horizontal no mobile.
5. **Serviços** — Grid de 8 serviços com ícones.
6. **App Gasfort** — Seção amarela com badges App Store/Google Play.
7. **Nossa História** — Timeline 1995 / 2008 / 2024.
8. **Para Empresas** — Formulário de cotação para frotas.
9. **Footer** — 4 colunas + copyright.
10. **Cookie banner** — Barra mínima na base (não modal).

**Mobile extra:** sticky CTA no rodapé com "Encontrar Posto" + "App".

---

## 📍 Localizador — Estrutura

1. **Header fixo** (mesmo da home).
2. **Page header escuro** — título e explicação.
3. **Barra de busca** — input de localização + filtros bandeira/serviço.
4. **Chips de filtro** — Conveniência, Troca de Óleo, Lavagem, Restaurante, 24h, Lavanderia.
5. **Desktop:** layout 2 colunas — lista de postos à esquerda, mapa à direita.
6. **Mobile:** toggle Mapa/Lista + filtros scroll horizontal + sticky CTA "Traçar rota".
7. **Card de posto:** logo da bandeira, nome, endereço, distância, serviços em pills, botões "Traçar rota" e "Detalhes".

---

## ✅ Pontos Fortes do Wireframe

1. CTA principal "Encontrar Posto" presente no header e na hero.
2. App destacado em duas seções + sticky CTA mobile.
3. Localizador com filtros úteis e reutiliza dados da planilha existente.
4. Cookie banner discreto (diferente dos concorrentes).
5. Paleta coerente com a marca Gasfort já existente.
6. Mobile-first: navegação por scroll, cards carrossel, CTA sticky.

## ⚠️ Pontos a Refinar no Mockup Final

1. **Fotos reais:** todos os espaços de imagem estão com placeholders `[FOTO MOCKUP]`.
2. **Textos reais:** headlines e descrições são placeholders; precisarão de copy final.
3. **Microcopy dos CTAs:** trocar genéricos por textos específicos (ex: "Abastecer agora").
4. **Validar localizador:** decidir se usa Google Maps embed, Mapbox ou planilha CSV + geocoding.
5. **Acessibilidade:** revisar contrastes e navegação por teclado no mockup de alta fidelidade.
6. **Animações:** definir se terá scroll reveal, hover states, skeleton loading.

---

## 🚀 Próximo Passo Sugerido

Criar o **mockup de alta fidelidade** no Figma ou HTML/CSS refinado, com:
- fotos reais ou placeholders de qualidade,
- copy final (ou mockup mais próximo do real),
- componentes interativos,
- design system completo (cores, tipografia, espaçamentos, componentes).

---

*Wireframe produzido por Nexo (Operator).*
