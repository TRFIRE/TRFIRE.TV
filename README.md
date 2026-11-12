# TV São Paulo — Playlist pessoal para SS IPTV (LG)

## O que este pacote contém

| Arquivo | Função |
| --- | --- |
| `index.html` | Página de apresentação e gerador da lista com pastas |
| `capa-principal.jpg` | Imagem principal da playlist externa |
| `logo-principal.png` | Ícone opcional para a playlist externa |
| `lista.m3u` | Lista simples, com os 7 canais e 9 reservas; funciona assim que o GitHub Pages for publicado |
| `canais-abertos.m3u` | 7 canais principais selecionados pelo proprietário |
| `teste-de-links.m3u` | 9 fontes de reserva aprovadas pelo proprietário |
| `canais-fechados.m3u` | Pasta vazia, preparada para canais legalmente acessíveis |
| `links-para-analisar.m3u` | Pasta vazia para os próximos testes |
| `EXEMPLO-lista-pastas.m3u` | Exemplo da playlist com pastas: **não use direto**, contém `SEU_USUARIO` |

As logos das emissoras são **links externos** já colocados em `tvg-logo` nas playlists. Não é preciso baixar nem hospedar imagens de terceiros no seu GitHub. Esses endereços podem mudar, e SVGs podem não renderizar em TVs antigas. O SS IPTV também pode obter logos pelo nome padronizado da emissora.

## Publicar pelo GitHub no navegador (celular ou computador)

1. Entre em https://github.com/new na sua conta.
2. Nome do repositório: **tv-sp-iptv**. Visibilidade: **Public** (para GitHub Pages gratuito). Clique em **Create repository**.
3. Extraia o ZIP no celular/computador. Na aba Code do repositório, clique em **Add file → Upload files**, selecione **todos os arquivos desta pasta** (não envie o ZIP fechado), role até o fim e clique em **Commit changes**.
4. No repositório, abra **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, depois **main / (root)** e **Save**.
5. Abra `https://SEU_USUARIO.github.io/tv-sp-iptv/` substituindo `SEU_USUARIO` por seu usuário real do GitHub. Se o Pages ainda estiver publicando, confira a própria tela Settings → Pages.
6. A página mostrará capa, canais e o botão **Gerar lista com pastas**. Clique nele. Será baixado `lista-pastas.m3u` com as URLs corretas do seu próprio domínio GitHub Pages.
7. Volte ao repositório no GitHub → **Add file → Upload files** e envie **apenas** `lista-pastas.m3u` (arquivo novo). Clique em **Commit changes**.
8. Os dois links finais serão:
   - lista simples: `https://SEU_USUARIO.github.io/tv-sp-iptv/lista.m3u`
   - lista com pastas: `https://SEU_USUARIO.github.io/tv-sp-iptv/lista-pastas.m3u`

**Atenção:** se seu usuário contém letras maiúsculas, use o endereço exato mostrado em Settings → Pages. Se alterar o nome do repositório, o gerador da página continuará funcionando porque usa o endereço atual automaticamente.

## SS IPTV da LG — criar nova capa na tela principal

1. Acesse https://ss-iptv.com/en/users/playlist no navegador e selecione sua TV já vinculada.
2. Entre em **External Playlists / Listas de reprodução externas** e clique **Add Item**.
3. Em **Displayed Name**, digite `TV SÃO PAULO`.
4. Em **Source**, cole `https://SEU_USUARIO.github.io/tv-sp-iptv/lista-pastas.m3u` (ou a lista simples, para começar).
5. Em **Tile Background**, selecione **Image** e cole `https://SEU_USUARIO.github.io/tv-sp-iptv/capa-principal.jpg`.
6. Se houver **Logo URL**, use `https://SEU_USUARIO.github.io/tv-sp-iptv/logo-principal.png`.
7. Confirme em **OK**, clique em **SAVE** no site e atualize o SS IPTV na TV.

O app oferece uma nova **tile de playlist externa**; não substitui a arte fixa da tile de playlist interna. A foto principal só aparecerá se sua versão do editor/app aceitar fundo de imagem para itens externos.

## Como atualizar no futuro

- `canais-abertos.m3u`: mantenha só os canais aprovados na TV; conserve a numeração.
- `teste-de-links.m3u`: guarde cópias alternativas aprovadas.
- `links-para-analisar.m3u`: coloque apenas candidatos temporários; ao concluir testes, limpe o arquivo.
- `canais-fechados.m3u`: use apenas URLs oficiais/autorizadas que você tenha direito de acessar.
- Atualize `lista.m3u` caso deseje manter a versão simples sincronizada; `lista-pastas.m3u` aponta para os quatro arquivos de categoria e não exige regeneração quando os canais mudarem.

## Observações sobre os links

O proprietário confirmou reprodução dos URLs em sua TV em novembro de 2026, mas isso não confirma autorização de redistribuição, permanência ou sinal regional de São Paulo. Alguns são servidores de terceiros. Um URL da Band e um da Record contêm parâmetro de token que pode expirar; não publique links particulares com senhas ou assinaturas neste repositório público. GitHub Pages hospeda arquivos, **não** transmite vídeo nem contorna restrições das emissoras.
