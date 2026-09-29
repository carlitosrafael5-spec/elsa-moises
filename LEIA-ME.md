# Convite digital · Elsa & Moisés

Site estático (sem servidor, sem base de dados). Abre em qualquer telemóvel Android ou iPhone.

## Ficheiros

- `index.html` · o convite
- `gerar.html` · ferramenta para gerar o link e a mensagem de WhatsApp de cada convidado
- `img/` · fotos do casal (já reduzidas)
- `musica/musica.mp3` · **coloque aqui a música** (MP3, idealmente até 4 MB). Sem este ficheiro o botão de música simplesmente não aparece.

## Antes de publicar

No fim de `index.html`, bloco `CONFIG`:

- `whatsappNoivos`: número que recebe as confirmações, só dígitos, com 258 (ex.: `258841234567`)
- `prazoConfirmacao`: por exemplo `"15 de Novembro"` (opcional)

## Publicar no GitHub Pages

1. Criar o repositório público `elsa-moises` na conta `carlitosrafael5-spec`
2. Enviar todo o conteúdo desta pasta
3. Settings > Pages > Branch `main` / pasta raiz
4. O convite fica em `https://carlitosrafael5-spec.github.io/elsa-moises/`

Se usar outro nome de repositório, actualize o `og:image` no topo do `index.html` (imagem da pré-visualização no WhatsApp) e o endereço no `gerar.html`.

## Link personalizado de cada convidado

```
https://carlitosrafael5-spec.github.io/elsa-moises/?n=Família+Rafael&m=5
```

- `n` · nome que aparece no envelope, na saudação e já preenchido na confirmação
- `m` · mesa do convidado
- `l` · número de lugares (opcional, por defeito 2)

## Fluxo com go.mz

1. Abrir `gerar.html` (no próprio site publicado ou localmente)
2. Colar a lista: `Nome ; mesa ; telefone`, uma linha por convidado
3. Para cada convidado: copiar o link completo, criar no go.mz o link curto (o nome sugerido está na coluna "Link curto sugerido"), colar o link curto na coluna ao lado
4. Carregar em **WhatsApp**: abre a conversa com a mensagem pronta

A lista fica guardada só no navegador onde foi usada. Use "Exportar CSV" para ter cópia.
