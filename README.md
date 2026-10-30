# Rede Gasfort — versão estática de demonstração

Site estático, sem servidor de aplicação. A lista de filiais é publicada em `data/filiais.json`, convertida da aba `lista filiais` do arquivo oficial do cliente. Não há geocodificação: os links de rota da fonte são usados diretamente.

## Preview local

Na raiz do projeto:

```sh
python3 -m http.server 8080
```

Abra http://localhost:8080. Não abrir `index.html` via `file://`, pois o navegador bloqueia a leitura do JSON local.

## Vercel

Importe o repositório no Vercel, selecione **Other**/site estático e configure:

- Root Directory: `.`
- Build Command: vazio (ou `echo static site`)
- Output Directory: `.`
- Install Command: vazio

Ou, com Vercel CLI instalado/autenticado: `vercel` para preview; `vercel --prod` somente após aprovação explícita. Nenhum deploy foi feito nesta tarefa.

## Dados e pendências

`public/data/filiais.json` tem 27 registros com nome, bandeira, cidade/UF, endereço e link da planilha oficial. Os filtros são por bandeira e a busca cobre nome/cidade/endereço. O site não atribui serviços por filial porque essa planilha não os contém.

A fonte não oferece coordenadas; o painel informa isso e não desenha marcadores aproximados. O link de rota em cada card é o da planilha.

Pendências a confirmar pelo cliente:
- F24: cidade consta como Santo Antônio da Patrulha, mas endereço aponta Parobé.
- F22 Pelotas e F42 Santo Antônio da Patrulha compartilham AV AFONSO PORTO EMERIM 5295; os links de rota foram mantidos sem inferência.
- Confirmar se as divergências e endereços sem complemento são intencionais.
- Validar conteúdo institucional afirmativo (contagens, serviços gerais e histórico) antes de publicação final.

## Fontes e publicação

Fonte de filiais: `FILIAIS GASFORT + ENDEREÇO.xlsx`, aba `lista filiais`. O arquivo original não é copiado nem modificado. O CTA corporativo aponta ao formulário oficial listado no brief da coleta; não é um envio implementado pelo site. Links não confirmados de redes sociais/WhatsApp e a confirmação fictícia de formulário foram removidos.
