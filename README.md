# TV ONLINE — V15 (sem pastas) — SS IPTV LG

A playlist abre diretamente nos canais, **sem nenhuma pasta**.

## Ordem da grade principal (01 a 15)

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

Depois da posição 15 estão os **9 links de backup** (posições 16 a 24), rotulados `BACKUP 01 - ...` a `BACKUP 09 - ...`. Nenhum deles aparece como pasta.

## Como funcionam os arquivos

- `lista-pastas.m3u`: **URL já usada na TV**, agora lista direta com 24 posições. Nome mantido só para evitar alterar o link configurado na TV.
- `lista.m3u`: idêntica à anterior, direta com 24 posições (15 principais + 9 backups).
- `canais-abertos.m3u`: só a grade de 15 posições.
- `teste-de-links.m3u`: 9 links de reserva preservados como arquivo técnico, sem pasta na tela.
- `sem-sinal.m3u8` e `sem-sinal00.ts`: cartela de aproximadamente 8 segundos para os espaços reservados; necessário hospedar os dois.
- `index.html`: site institucional atualizado para TV ONLINE, sem gerador de pastas.

## URL a manter no SS IPTV

https://trfire.github.io/TRFIRE.TV/lista-pastas.m3u

**Renomear o bloco da tela inicial:** no SS IPTV, vá a **Configurações → Conteúdo → Listas externas**, localize o título `TV SÃO PAULO` e renomeie para **TV ONLINE** (ou pelo editor de playlists externo, caso tenha cadastrado lá). A mudança do nome visual não é controlada pelo arquivo M3U.

## Correções já incorporadas das versões anteriores

- SBT (04): teste 06, SBT Nova Mutum (MT), pode não refletir programação regional de SP.
- Globo (05): teste 03 aprovado, Barigui Telecom, identificação de SP.
- Record (07): link 02 nacional aprovado, pode não refletir programação local de SP.
- RedeTV! (09): link 02 V7 aprovado.
- Band (13): logo hospedada em `logo-band.png` (arquivo já existente no repositório).
- Demais canais, logotipos, reservas e artes existentes mantidos.

**Sobre a publicação:** substitua os oito arquivos da pasta `ATUALIZAR-NA-RAIZ` no repositório `TRFIRE/TRFIRE.TV`, com nomes idênticos, e confirme o commit. Não é necessário apagar imagens nem outros arquivos antigos. A lista externa continuará no mesmo endereço.

A reprodução de um stream não confirma autorização para sua redistribuição pública; use somente endereços que tenha permissão para acessar e divulgar.
