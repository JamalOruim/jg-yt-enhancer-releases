# Histórico de versões

## v6.4 — Correções de deslikes, letras e atualização (2026-11-20)

**Alterado**
- Deslikes e busca de letras agora passam pelo processo interno da extensão, sem depender da página do YouTube
- "Atualizar agora" avisa com clareza quando o host nativo está registrado em outra pasta e diz o que fazer

**Corrigido**
- Erro "Unsafe attempt to load URL" ao buscar os deslikes
- Busca de letras podendo ser bloqueada pelo YouTube

## v6.3 — SponsorBlock e biblioteca de letras (2026-11-20)

**Novo**
- SponsorBlock: pula sozinho patrocínios, autopromoção e pedidos de like/inscrição marcados pela comunidade
- Ao pular um trecho aparece um aviso — clique nele para voltar
- Trechos do SponsorBlock aparecem coloridos na barra de progresso
- Aba Player mostra os trechos do vídeo e quanto tempo você economizou
- Ajustes → SponsorBlock: escolha o que pular (intro, encerramento, enrolação e mais)
- Busca e contador na biblioteca de letras
- Botão para limpar a biblioteca de letras (pede confirmação)

**Corrigido**
- Biblioteca de letras com muitas músicas deixava os botões minúsculos e ilegíveis
- O mesmo problema nas listas de momentos e de downloads
- Avisos que reapareciam rápido podiam sumir antes da hora

## v6.2 — Atualizações automáticas (2026-11-20)

**Novo**
- Aviso de nova versão no painel e no botão JG, com a lista do que mudou
- Botão "Atualizar agora": o host baixa a versão nova, confere a integridade e a extensão recarrega sozinha
- Histórico de versões em Ajustes → Atualizações
- Tela de novidades depois de cada atualização
- O instalar_host.bat baixa o FFmpeg automaticamente se ele não estiver na pasta

**Alterado**
- O ID da extensão agora é fixo: o host nativo continua funcionando mesmo se a pasta mudar de lugar
- O instalar_host.bat não pede mais o ID da extensão

**Removido**
- Pergunta do ID da extensão no instalador

## v6.1 — Playlists e erro 403 (2026-11-19)

**Novo**
- Pergunta "Só este vídeo" ou "Playlist inteira" ao baixar um vídeo aberto numa playlist ou Mix
- Downloads de playlist em subpasta, com arquivos numerados e progresso por item
- Ajustes → Vídeo em playlist (Perguntar / Só o vídeo / Playlist toda)
- Aviso "Falta o solucionador JS" com botão para instalar

**Alterado**
- "Atualizar yt-dlp" agora instala o yt-dlp com o solucionador do desafio JavaScript do YouTube
- Nomes de arquivo se ajustam ao limite de caminho do Windows

**Corrigido**
- Downloads falhando com "HTTP Error 403: Forbidden"
- Download de playlist em MP3 falhava ao salvar a capa da própria playlist

## v6.0 — Painel novo (2026-11-18)

**Novo**
- Painel redesenhado com 7 cores de destaque, arrastável e funcionando em tela cheia
- EQ gráfico interativo com espectro ao vivo e limiter
- Fila de downloads com cancelar, tentar de novo, resolução até 4K, bitrate e trecho A–B
- Letras sincronizadas com overlay karaokê, ajuste de sincronia e biblioteca
- Loop A–B e momentos marcados na barra de progresso
- Backup e restauração das configurações

**Alterado**
- Filtros de vídeo com presets, matiz e inverter
- Contador de deslikes com barra de aprovação

**Removido**
- Botões de texto antigos do painel (substituídos por ícones)

**Corrigido**
- Vídeo ficava mudo depois de pular anúncios
- Títulos e nomes com caracteres especiais quebravam a interface
- Formato OGG sempre falhava
- Status "Online" aparecia mesmo com o host desligado
