# Rede Gasfort — Brief de Coleta para Mockup de Site

**Data da coleta:** 2026-06-15  
**Fonte principal:** https://redegasfort-bio.netlify.app/  
**Objetivo:** Base de dados real para criação do mockup/site institucional.

---

## 1. Identidade da Empresa

| Campo | Valor |
|-------|-------|
| Nome comercial | **Rede Gasfort** |
| Antiga marca | Rede de Postos Assunção |
| Grupo atual | Grupo Assunção |
| Slogan | "Tradição e qualidade há mais de 30 anos!" |
| Segmento | Rede de postos de combustíveis + lojas de conveniência + cuidados automotivos |
| Presença | 12+ municípios no Rio Grande do Sul |
| Unidades | 25 filiais mapeadas na planilha ativa; comunicação institucional fala "mais de 30 postos" |
| Ano de origem | 1995 (início como Posto Esso em Igrejinha/RS) |
| Marca criada | 2024 (unificação dos postos sob a marca Gasfort) |
| Followers LinkedIn | 147 |

### Linha do tempo (do LinkedIn)
- **1995** — Rede de Postos Assunção nasce em Igrejinha/RS como Posto Esso.
- **2001** — Aquisição/construção do Posto Petrobras em Sapiranga/RS.
- **2003** — Primeiro Posto Texaco.
- **2008** — Aquisição da Texaco pela Ipiranga; Rede Assunção segue crescendo.
- **2024** — Criação do Grupo Assunção; postos passam a operar sob a marca **Gasfort**.
- **2025/2026** — Comemora 30 anos de história.

---

## 2. Marca Visual

### Cores da marca Gasfort
- **Amarelo vibrante:** `#FFC400` (cor primária)
- **Amarelo hover:** `#F2BA00`
- **Texto principal:** `#1C1C1E`
- **Texto secundário/muted:** `#8E8E93`
- **Fundo app/cinza:** `#E4E4E7`
- **Cards/superfície:** `#FFFFFF`

### Logo Gasfort
- Formato: imagem JPG quadrada, fundo amarelo.
- Texto: "gasfort" em letras minúsculas, cinza escuro, sans-serif arredondada e bold.
- Ícone: chevron/seta apontando para a direita em branco, simbolizando movimento/direção.
- Estilo: minimalista, flat, moderno, alta visibilidade.
- URL do logo usado no site: `https://i.postimg.cc/fWr0L3vR/1731066267268.jpg`

### Bandeiras atuantes na rede
| Bandeira | Cor identidade | Observação |
|----------|----------------|------------|
| **Gasfort** | Amarelo/cinza | Marca própria do grupo |
| **Ipiranga** | Amarelo/azul | Franquia/branding nacional |
| **Shell** | Vermelho/amarelo | Franquia/branding internacional |
| **Charrua** | Vermelho/branco | Cavaleiro em silhueta, simbolismo gaúcho/ancestral |
| **Santa Lucia** | Laranja/preto | Iniciais "SL" em losango |

### Tipografia do site atual
- Fonte principal: Inter (Google Fonts) / fallback SF Pro Display.
- Pesos usados: 400, 500, 600, 700, 800.
- Estilo visual: inspirado em iOS/Apple — cards arredondados, squircle, sombras suaves, animações suaves.

---

## 3. Estrutura do Site Atual (Linktree / SPA)

O site atual é um **linktree mobile-first** (max-width 480px) com navegação em Single Page Application (SPA) entre duas views:

### View Home (`#view-home`)
Header com logo circular + nome + slogan.
Grid de links principais:
1. **BAIXE O NOSSO APP - iOS** → App Store (`id6498787617`)
2. **BAIXE O NOSSO APP - Android** → Google Play (`com.kodefy.gasfort`)
3. **COTAÇÃO - EMPRESAS** → Google Forms (`1FAIpQLSckzHBj9Towra7nJ5vVZXztC6w2A-iA3iUQxQ7_vkmcWrR5Xw`)
4. **NOSSAS FILIAIS** → abre view interna de lista
5. **TRABALHE CONOSCO** → Google Forms (`forms.gle/9o3a4ALs9uR8JG1w6`)
6. **LINKEDIN** → `https://www.linkedin.com/company/rede-gasfort`

### View Filiais (`#view-locations`)
- Navbar com botão voltar + título "Nossas Filiais".
- Indicador de loading: "Buscando unidades...".
- Lista de cards iOS-style com: logo da bandeira, nome da unidade, endereço, serviços, botão "Traçar Rota".
- Dados carregados em tempo real de planilha Google Sheets publicada em CSV.

### Rodapé
> "© 2026 Rede Gasfort. Todos os direitos reservados."

---

## 4. Apps da Rede

### iOS
- **Nome:** App Rede Gasfort
- **Desenvolvedor:** Kodefy - Desenvolvimento de apps
- **URL:** https://apps.apple.com/br/app/rede-gasfort/id6498787617

### Android
- **Nome:** Rede Gasfort - Combustíveis
- **Pacote:** `com.kodefy.gasfort`
- **Desenvolvedor:** Kodefy
- **Descrição:** "The Rede Gasfort App offers discounts, cashback and exchange of points for products"
- **URL:** https://play.google.com/store/apps/details?id=com.kodefy.gasfort

### Funcionalidades do app (inferidas da descrição)
- Descontos em combustível
- Cashback
- Troca de pontos por produtos
- Provavelmente: localizador de postos, histórico de abastecimento, campanhas de fidelidade.

---

## 5. Filiais — Dados Reais (25 unidades)

**Fonte:** Planilha Google Sheets publicada em CSV (link no JS do site).

### Resumo por bandeira
| Bandeira | Quantidade |
|----------|------------|
| Gasfort | 7 |
| Ipiranga | 8 |
| Shell | 3 |
| Charrua | 3 |
| Santa Lucia | 3 |
| *(SERRANO sem CNPJ)* | 1 (Santa Lucia) |

### Resumo por cidade/município
- Gramado, Rio Grande (2), Guaíba (2), Canela, Capão do Leão, Sapiranga, Porto Alegre, Capivari do Sul, Taquara (3), Parobé, Rolante (2), Santo Antônio da Patrulha (3), São Gabriel (2), Santa Margarida do Sul, Dom Feliciano, Pelotas.

### Empresas jurídicas do grupo
1. ABASTECEDORA COSTA DOCE LTDA
2. ABASTECEDORA DE COMBUSTIVEIS FELICITA
3. ABASTECEDORA DE COMBUSTIVEIS ROLANTCHÊ LTDA
4. ABASTECEDORA DE COMBUSTIVEIS ROTA DA PRAIA LTDA
5. ABASTECEDORA DE COMBUSTIVEIS ROTULA 030 LTDA
6. ABASTECEDORA DE COMBUSTIVEIS VISCONDE DE MAUA LTDA
7. ABASTECEDORA EDITH G P ASSUNCAO LTDA
8. ABASTECEDORA UNIVERSAL CASSINO LTDA
9. ABASTECEDORA UNIVERSAL DOM JOAQUIM LTDA
10. BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA
11. COMERCIAL DE COMBUSTIVEIS MARGARIDA DO SUL LTDA
12. COMERCIAL DE COMBUSTIVEIS SERRANO LTDA
13. COMERCIO DE COMBUSTIVEIS GABRIELENSE LTDA
14. SW COMERCIO DE COMBUSTIVEIS LTDA

### Lista completa de filiais

| # | Nome fantasia | Empresa | CNPJ | IE | Cidade/Filial | Endereço | Bandeira | Serviços | Link Maps |
|---|---------------|---------|------|----|---------------|----------|----------|----------|-----------|
| 1 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000559 | 056/0111010 | Gramado | AV DAS HORTENSIAS 1038, PLANALTO, 95670-000, GRAMADO-RS | Shell | SHELL SELECT | https://maps.app.goo.gl/zrZKyxs8fH5bZ4z69 |
| 2 | COMERCIAL DE COMBUSTIVEIS SERRANO | COMERCIAL DE COMBUSTIVEIS SERRANO LTDA | 33192210001150 | 100/0337500 | Rio Grande | RUA PINTO BANDEIRA 151, RIO GRANDE-RS | Gasfort | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/BgnUovRhqJHfCJcW8 |
| 3 | COMERCIAL DE COMBUSTIVEIS SERRANO | COMERCIAL DE COMBUSTIVEIS SERRANO LTDA | 33192210000773 | 058/0157709 | Guaíba - NEI BRITO | AV DR NEI BRITO, 55, SANTA RITA, 92708720, GUAÍBA-RS | Gasfort | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO; LAVANDEIRA | https://maps.app.goo.gl/MUxf2WazrtAjXxhQ6 |
| 4 | COMERCIAL DE COMBUSTIVEIS SERRANO | COMERCIAL DE COMBUSTIVEIS SERRANO LTDA | 33192210001079 | 058/0157695 | Guaíba - Castelo | AV MAL CASTELO BRANCO 1993, COLINA, 92700805, GUAÍBA-RS | Charrua | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/tcbX6fW1fRMTzEZJA |
| 5 | ABASTECEDORA VISCONDE DE MAUA | ABASTECEDORA DE COMBUSTIVEIS VISCONDE DE MAUA LTDA | 24176909000163 | 235/0017251 | Capão do Leão | AV NARCISO SILVA 1073, CENTRO, 96160000, CAPÃO DO LEÃO-RS | Ipiranga | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/49KZXH1qmzjVdokRA |
| 6 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000630 | 131/0177314 | Sapiranga | RUA SEN SALGADO FILHO 1004, SÃO LUIZ, 93806312, SAPIRANGA-RS | Shell | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/zJLTr6iaK7Av93ns6 |
| 7 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000710 | 096/4021889 | POA (Porto Alegre) | AV TRAMANDAÍ 42, IPANEMA, 91760050, PORTO ALEGRE-RS | Gasfort | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO; LAVANDEIRA; LAVAGEM | https://maps.app.goo.gl/EJAvLaWmT2yrXDxg7 |
| 8 | ABASTECEDORA ROTULA 030 | ABASTECEDORA DE COMBUSTIVEIS ROTULA 030 LTDA | 34427438000172 | 433/0007087 | Capivari do Sul | AV TELMO SESSIM 1546, CENTRO, 95552000, CAPIVARI DO SUL-RS | Ipiranga | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/FkC8ZVABt7biXBGp9 |
| 9 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000397 | 141/0112117 | Taquara - Bmzinho | RUA MAL FLORIANO 1726, CENTRO, 95600032, TAQUARA-RS | Gasfort | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO; LAVANDEIRA | https://maps.app.goo.gl/dm246E4rRL7rwGDk7 |
| 10 | ABASTECEDORA EDITH G P ASSUNCAO | ABASTECEDORA EDITH G P ASSUNCAO LTDA | 23001545000118 | 241/0074396 | Parobé - GP | ROD ERS 239 5353, CONCEICAO DO FUNIL, 95630000, PAROBÉ | Ipiranga | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/iq5keQMAqre9nGdM9 |
| 11 | COMERCIAL DE COMBUSTIVEIS SERRANO | COMERCIAL DE COMBUSTIVEIS SERRANO LTDA | 33192210000269 | 103/0035846 | Rolante - Pórtico | EST RS 239 7674, INTERIOR, 95690000, ROLANTE-RS | Ipiranga | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/CS6JTwsfbspEKQDd7 |
| 12 | ABASTECEDORA ROLANTCHÊ | ABASTECEDORA DE COMBUSTIVEIS ROLANTCHÊ LTDA | 30771575000179 | 103/0032910 | Rolante - Rolantchê | AV TENENTE PEDRO VON MUHLEN 661, CENTRO, 95690000 | Gasfort | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/9egW67wiUigtf6bq8 |
| 13 | ABASTECEDORA ROTA DA PRAIA | ABASTECEDORA DE COMBUSTIVEIS ROTA DA PRAIA LTDA | 22874782000120 | 114/0093999 | Sto Antonio da Patrulha | RUA JOAO CARLOS BEMFICA 29, MENINO DEUS, 95500000, SANTO ANTONIO DA PATRULHA-RS | Shell | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/sGTfSz7aSx9zUSZ3A |
| 14 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000125 | 141/0108160 | Taquara - Chega Aí | AV OSCAR MARTINS RANGEL 3526, JARDIM DO PRADO, 95612450, TAQUARA-RS | Gasfort | LOJA DE CONVENIÊNCIA; RESTAURANTE; TROCA DE ÓLEO; 24 HORAS | https://maps.app.goo.gl/QN1hR7nqtwyMHCBt8 |
| 15 | ABASTECEDORA EDITH G P ASSUNCAO | ABASTECEDORA EDITH G P ASSUNCAO LTDA | 23001545000207 | 120/0123724 | São Gabriel - SG | AV ANTONIO TRILHA 1222, CENTRO, 97310010, SÃO GABRIEL-RS | Ipiranga | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO | https://maps.app.goo.gl/2VsKRv4sVWHzRvtF9 |
| 16 | COMERCIO GABRIELENSE | COMERCIO DE COMBUSTIVEIS GABRIELENSE LTDA | 31147869000197 | 120/0118780 | São Gabriel - Gabrielense | RUA GEN JOAO MANOEL 579, CENTRO, 97300000, SÃO GABRIEL-RS | Charrua | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/rohPZHAr7SCB3mKk7 |
| 17 | COMERCIAL MARGARIDA DO SUL | COMERCIAL DE COMBUSTIVEIS MARGARIDA DO SUL LTDA | 31218545000100 | 495/0002324 | Sta Margarida do Sul | EST BR 290 800, CENTRO, 97335000, SANTA MARGARIDA DO SUL-RS | Ipiranga | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/quvX23pTxQeSLNBG6 |
| 18 | ABASTECEDORA FELICITA | ABASTECEDORA DE COMBUSTIVEIS FELICITA | 26898300000123 | 190/0010108 | Dom Feliciano | RUA BORGES DE MEDEIROS 266, CENTRO, 96190000, DOM FELICIANO-RS | Charrua | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/eoHEQXo2g9iUf2mg8 |
| 19 | COMERCIAL DE COMBUSTIVEIS SERRANO | COMERCIAL DE COMBUSTIVEIS SERRANO LTDA | 33192210000188 | 022/0077070 | Canela | PC DAS NACOES 15, CENTRO, 95680000, CANELA-RS | Ipiranga | AMPM; PIZZA HUT; TROCA DE ÓLEO | https://maps.app.goo.gl/LWvVW36ztPygWXZm9 |
| 20 | SW COMERCIO | SW COMERCIO DE COMBUSTIVEIS LTDA | 48054236000137 | 1140098745 | Sto Antonio 3 | AV AFONSO PORTO EMERIM 5295, SANTO ANTONIO DA PATRULHA-RS | Charrua | LOJA DE CONVENIÊNCIA; RESTAURANTE | https://maps.app.goo.gl/V3yrkgCSP6oMm9Q98 |
| 21 | BOHRER MIGUEL | BOHRER MIGUEL COMERCIO DE COMBUSTIVEIS LTDA | 28053659000982 | 141/0121230 | Taquara - Sta Lucia | R TRISTAO MONTEIRO 1781, JD DO PRADO, TAQUARA-RS | Santa Lucia | LOJA DE CONVENIÊNCIA; TROCA DE ÓLEO, LAVAGEM | https://maps.app.goo.gl/efC4dDTcrcCybjMS8 |
| 22 | ABASTECEDORA COSTA DOCE | ABASTECEDORA COSTA DOCE LTDA | 47854213000144 | 100/0333024 | Rio Grande - Costa Doce | SENADOR SALGADO FILHO 210, PARQUE SALGADO FILHO, RIO GRANDE-RS | Ipiranga | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/XJddbpwuiUdoJDmW9 |
| 23 | ABASTECEDORA UNIVERSAL CASSINO | ABASTECEDORA UNIVERSAL CASSINO LTDA | 50489010000100 | 100/0338565 | Rio Grande - Cassino | AV RIO GRANDE 802, CASSINO, RIO GRANDE-RS | Ipiranga | AMPM; TROCA DE ÓLEO | https://maps.app.goo.gl/XfwQZoJbcxEpjqobA |
| 24 | ABASTECEDORA UNIVERSAL DOM JOAQUIM | ABASTECEDORA UNIVERSAL DOM JOAQUIM LTDA | 50536623000151 | 093/0510844 | Pelotas | AV DOM JOAQUIM 510, CENTRO, PELOTAS-RS | Ipiranga | AMPM; TROCA DE ÓLEO, 24 HORAS | https://maps.app.goo.gl/nPvsdjqB3rasBqKRA |
| 25 | SERRANO | (sem CNPJ preenchido) | 33192210001230 | 1140102807 | Sto Antonio 2 | AV CORONEL VICTOR VILLA VERDE 852, PITANGUEIRAS, SANTO ANTONIO DA PATRULHA-RS | Santa Lucia | LOJA DE CONVENIÊNCIA | https://maps.app.goo.gl/pihR9hur2eLdepFBA |

### Serviços oferecidos (consolidado)
- Loja de conveniência
- Troca de óleo
- Lavanderia / lavandeira
- Lavagem de carro (car wash)
- Restaurante / lanchonete
- 24 horas
- AMPM
- Pizza Hut
- Shell Select

---

## 6. Links e Contatos Encontrados

| Tipo | URL |
|------|-----|
| Site/linktree atual | https://redegasfort-bio.netlify.app/ |
| App iOS | https://apps.apple.com/br/app/rede-gasfort/id6498787617 |
| App Android | https://play.google.com/store/apps/details?id=com.kodefy.gasfort |
| LinkedIn | https://www.linkedin.com/company/rede-gasfort |
| Cotação empresas | https://docs.google.com/forms/d/e/1FAIpQLSckzHBj9Towra7nJ5vVZXztC6w2A-iA3iUQxQ7_vkmcWrR5Xw/viewform |
| Trabalhe conosco | https://forms.gle/9o3a4ALs9uR8JG1w6 |
| Planilha de filiais (CSV) | https://docs.google.com/spreadsheets/d/e/2PACX-1vQVtKzzKxkZFD943TX73IBW5hKucyJUFeqRR0BS68krc2dPD3SibkxpGgJXTdXa8oxPs4KzsZG1Z6O-/pub?output=csv |

### NÃO foram encontrados (recomenda-se perguntar ao cliente)
- Site institucional completo (apenas linktree)
- E-mail corporativo
- Telefone comercial / SAC
- WhatsApp oficial
- Instagram / Facebook / YouTube
- Propriedades do Grupo Assunção separadas
- Slogans alternativos, manifesto ou valores escritos
- Fotos institucionais dos postos
- Equipe / diretoria

---

## 7. Recomendações para Mockup

### Seções sugeridas para um site institucional
1. **Hero** — 30 anos de tradição, energia que move o RS.
2. **Sobre / História** — timeline 1995 → 2024 → hoje.
3. **Nossos Postos** — mapa interativo ou grade de filiais com filtros (cidade, bandeira, serviço).
4. **Serviços** — combustíveis, conveniência, troca de óleo, lavagem, restaurante, fidelidade.
5. **App Gasfort** — downloads iOS/Android, funcionalidades de desconto/cashback/pontos.
6. **Cotação para Empresas** — CTA para frota/empresas.
7. **Trabalhe Conosco** — cultura + form.
8. **Blog/Notícias** — comemorações, novidades, posts do LinkedIn.
9. **Contato / Rodapé** — redes, e-mail, telefone (a confirmar).

### Tom de voz sugerido
- Confiável, familiar, regional (RS), moderna.
- Palavras-chave: tradição, qualidade, confiança, energia, movimento, 30 anos, cuidado com o carro, cuidado com a família.
- Reforçar o reposicionamento: do legado Assunção para a marca unificada Gasfort.

### Paleta recomendada (baseada na marca)
- Primária: `#FFC400` (amarelo Gasfort)
- Escura: `#1C1C1E` (quase preto)
- Neutros: `#E4E4E7`, `#8E8E93`, `#FFFFFF`
- Destaque azul (Ipiranga) / vermelho (Shell/Charrua) podem ser usados como cores de bandeira, nunca para a marca Gasfort.

### Fontes recomendadas
- **Títulos:** Inter 700/800 (ou SF Pro Display no iOS)
- **Corpo:** Inter 400/500
- Alternativa premium: "Plus Jakarta Sans" ou "Geist" para dar mais peso institucional.

### Considerações técnicas
- O cliente já tem App publicado na App Store e Play Store — site pode puxar deep links.
- A planilha de filiais já está publicada e alimenta o linktree; pode ser reaproveitada via CSV/JSON no novo site.
- O cliente já usa Netlify — facilita hospedagem.
- Não há backend aparente; site deve ser estático + eventual consumo da planilha.

---

## 8. Ativos Coletados (arquivos no workspace)

- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/gasfort-logo.jpg`
- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/logo-charrua.png`
- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/logo-ipiranga.png`
- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/logo-sta-lucia.jpg`
- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/1731066267268.jpg` (cópia do logo)
- `/home/nexo-operator/.openclaw/workspace/tmp/gasfort/REDE_GASFORT_BRIEF.md` (este arquivo)

---

*Coleta feita por Nexo (Operator). Próximo passo: validar com Marroc se faltou alguma informação essencial antes de partir para o mockup.*
