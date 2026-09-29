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
- `m` · número da mesa (1 a 12). O convite mostra o nome da virtude bíblica: 1 Amor, 2 Fé, 3 Esperança, 4 Alegria, 5 Paz, 6 Paciência, 7 Bondade, 8 Fidelidade, 9 Mansidão, 10 Domínio Próprio, 11 Humildade, 12 Sabedoria. Os nomes estão em `MESAS` (index.html) e `NOMES` (gerar.html).
- `l` · número de lugares (opcional, por defeito 2)

## Gestão de convidados (gerar.html)

Página simples, pensada para quem não é da informática:

1. **Adicionar:** nome, telefone e mesa (1 a 12). Avisa se o convidado já existe ou se a mesa está cheia.
2. **Enviar convite:** abre uma janela com dois passos. Link curto no go.mz (opcional) e envio por WhatsApp com a mensagem pronta. O convidado fica marcado como "Convite enviado", com data e hora.
3. **Registar resposta:** quando a confirmação chega ao WhatsApp, marque "Confirmou presença" ou "Não vem".
4. **Mesas:** as 12 mesas com quem está sentado em cada uma e os lugares livres.
5. **Definições:** texto da mensagem, cópia de segurança e exportação para Excel.

A lista fica guardada no navegador do aparelho onde é usada. Faça "Guardar cópia" com regularidade; com "Recuperar cópia" passa a lista para outro aparelho.
