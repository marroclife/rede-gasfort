# Mockup de Alta Fidelidade — Rede Gasfort

**Data:** 2026-06-15  
**Arquivo principal:** `index.html` (HTML/CSS/JS responsivo, single-page)

---

## 📁 Arquivos

| Arquivo | Descrição |
|---------|-----------|
| `index.html` | Mockup completo e navegável |
| `assets/` | Logo Gasfort + logos das bandeiras |
| `mockup-desktop-full.png` | Screenshot desktop full-page |
| `mockup-mobile-full.png` | Screenshot mobile full-page |
| `README_MOCKUP.md` | Este documento |

---

## ✨ Destaques do Mockup

### Identidade Visual
- Paleta oficial da Gasfort: amarelo `#FFC400`, quase-preto `#0D0D0F`/`#1C1C1E`, cinza `#F5F5F7`.
- Tipografia: **Plus Jakarta Sans** para títulos, **Inter** para corpo.
- Logo real da Gasfort aplicada no header e footer.
- Cards arredondados (squircle), sombras suaves, transições suaves.

### Seções Implementadas

1. **Header fixo** com blur — logo, navegação, CTA "Encontrar Posto" + "Baixar App".
2. **Hero escuro** com ilustração de bombas de combustível e stats.
3. **Stats bar** — 30+ anos, 25+ postos, 12+ cidades, 5 bandeiras.
4. **Nossos Postos** — cards das principais regiões.
5. **Localizador funcional** com mapa Leaflet + filtros por bandeira + busca textual — alimentado pela **planilha CSV real** do site atual.
6. **Serviços** — grid de 8 cards com ícones.
7. **App Gasfort** — seção amarela com mockup de celular em CSS e badges App Store/Google Play (links reais).
8. **Nossa História** — timeline interativa 1995 / 2008 / 2024.
9. **Para Empresas** — formulário de cotação funcional (mockup de envio).
10. **Footer** — 4 colunas + redes sociais + LinkedIn real.
11. **Cookie banner** discreto na base.

### Interatividade
- Mapa interativo com markers amarelos.
- Filtros por bandeira (Gasfort, Ipiranga, Shell, Charrua, Santa Lúcia).
- Busca por cidade/endereço/serviço.
- Scroll reveal nas seções.
- Header com efeito de scroll.
- Menu mobile funcional.
- Formulário B2B com validação básica.

### Responsivo
- Desktop: 1440px+
- Tablet: 1024px
- Mobile: 390px

---

## 🚀 Como visualizar

Abra o arquivo `index.html` diretamente em qualquer navegador moderno:

```bash
# Via Python simples
python3 -m http.server 8080 --directory /home/nexo-operator/.openclaw/workspace/tmp/gasfort/mockup

# Depois acesse
# http://localhost:8080
```

---

## 📝 Notas sobre Dados

- **Localizador:** consome em tempo real a planilha Google Sheets publicada no linktree atual. As coordenadas dos postos são aproximadas por cidade (já que a planilha não tem lat/lng); no produto final recomenda-se geocodificar os endereços reais.
- **Contatos (e-mail/telefone/ WhatsApp):** estão como placeholders `[mockup]` pois ainda não foram fornecidos.
- **Fotos de postos:** foram substituídas por ilustrações CSS/gradientes + ícones, pois não há imagens reais disponíveis.
- **Textos institucionais:** baseados nos dados reais coletados do LinkedIn e do site atual.

---

## 🎯 Próximos Passos (se aprovado)

1. Substituir placeholders por contatos reais.
2. Inserir fotos profissionais dos postos.
3. Refinar copy com base na voz da marca.
4. Geocodificar endereços reais no localizador.
5. Adicionar página interna de detalhe do posto.
6. Implementar blog/novidades.
7. Testes de performance, acessibilidade (WCAG) e SEO.

---

*Mockup produzido por Nexo (Operator).*
