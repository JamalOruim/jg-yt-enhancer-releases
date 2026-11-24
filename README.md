# JG YouTube Enhancer

Extensão para Chrome / Edge / Brave que turbina o YouTube: EQ gráfico, downloads com fila (yt-dlp),
letras sincronizadas, loop A–B, filtros de vídeo, filtro de chat, deslikes e mais.

**Versão atual: 6.6** — [baixar o .zip](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases/download/v6.6/JG-YouTube-Enhancer-v6.6.zip) · [todas as versões](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases)

## Instalação (primeira vez)

1. Baixe o `.zip` acima e extraia numa pasta permanente (ex.: `Documentos\JG-YouTube-Enhancer`).
2. Abra `chrome://extensions`, ative o **Modo do desenvolvedor** e clique em **Carregar sem compactação**, escolhendo a pasta extraída.
3. Para os downloads: instale o [Python](https://www.python.org/) marcando *Add python.exe to PATH* e rode o `instalar_host.bat` da pasta.
   Ele instala o yt-dlp, baixa o FFmpeg e registra o host — não precisa digitar nada.

## Atualizações

A extensão verifica sozinha. Quando sair uma versão nova aparece um aviso no YouTube e um ponto verde no botão **JG**.
No painel, clique em **Atualizar agora**: ela baixa, confere a integridade e recarrega sozinha.
Sem o host instalado, use **Atualizar manualmente**: extraia o `.zip` novo por cima da pasta atual e clique em **Já extraí — recarregar**.

## Novidades da 6.6

### v6.6 — Solucionador JS sem complicação (2026-11-23)

**Novo**
- O instalar_host.bat instala o deno sozinho quando o PC não tem Node.js nem deno
- Se o pip falhar, o deno é baixado direto do site oficial e a integridade é conferida

**Alterado**
- "Instalar agora" mostra o andamento e avisa quando o solucionador JS ficou pronto
- O host encontra o Node.js e o deno mesmo quando foram instalados com o navegador aberto

**Corrigido**
- "Falta o solucionador JS" continuava aparecendo depois de instalar o deno pelo botão em alguns PCs

[Histórico completo](CHANGELOG.md)

---
FFmpeg: binário de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/) (licença GPL), distribuído sem modificações; código-fonte em https://ffmpeg.org.
