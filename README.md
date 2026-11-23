# TV ONLINE — V15.1 — Apenas 15 posições na lista pública

A playlist abre **diretamente** nos canais, sem pastas. A sequência termina em **15. UNIVERSAL TV**. Nenhum canal de backup é publicado ou aparece depois da posição 15.

## Ordem da grade (controle remoto)

01. SEM SINAL
02. TV CULTURA - SP
03. SEM SINAL
04. SBT HD - SP
05. GLOBO HD - SP
06. SEM SINAL
07. RECORD HD - SP
08. SEM SINAL
09. REDE TV! HD - SP
10. SEM SINAL
11. GAZETA HD - SP
12. SEM SINAL
13. BAND HD - SP
14. AXN HD - BR
15. UNIVERSAL TV

## Arquivos publicados

- `lista-pastas.m3u`: playlist direta com somente 15 posições. O nome antigo é preservado para manter o mesmo link cadastrado na LG; o conteúdo **não tem pastas**.
- `lista.m3u`: a mesma lista de 15 posições, sem backups.
- `canais-abertos.m3u`: a mesma lista de 15 posições.
- `sem-sinal.m3u8` e `sem-sinal00.ts`: vídeo que permite preencher as 6 posições SEM SINAL.
- `index.html`: site TV ONLINE, atualizado para 15 posições.

**Remova do GitHub o arquivo antigo `teste-de-links.m3u`.** Ele não é necessário nem referenciado na nova playlist. Guarde os nove links antigos somente no arquivo privado `TV_ONLINE_BACKUP_LOCAL_9_LINKS_NAO_ENVIAR_GITHUB.m3u`, baixado separadamente e **não enviado ao repositório**.

## Endereço da lista na LG (não muda)

https://trfire.github.io/TRFIRE.TV/lista-pastas.m3u

No SS IPTV, renomeie o título da playlist externa de TV SÃO PAULO para **TV ONLINE** (título local separado do arquivo M3U).

## Correções preservadas

- SBT 04: teste 06 aprovado (fonte identificada como SBT Nova Mutum - MT).
- Globo 05: teste 03 aprovado (origem identificada como SP).
- Record 07: LINK 02 nacional aprovado (pode ter diferenças de programação regional).
- RedeTV! 09: LINK 02 V7 aprovado.
- Band 13: logo em `logo-band.png`, já existente no repositório.
- Os demais canais e endereços permanecem como na V15.

## Publicação

Extraia o ZIP e carregue na raiz do repositório os **7 arquivos** da pasta `ATUALIZAR-NA-RAIZ`. Substitua os arquivos com mesmo nome e confirme o commit. Depois, **delete `teste-de-links.m3u` no GitHub** por meio do menu de arquivo (Delete file) e faça o commit da exclusão. Não carregue o arquivo de backup privado ao GitHub.

A reprodução de um link não confirma autorização de retransmissão pública; use somente fontes para as quais você tenha permissão de acesso e publicação.
