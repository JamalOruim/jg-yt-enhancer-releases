# JG YouTube Enhancer

Extensão para Chrome / Edge / Brave que turbina o YouTube: EQ gráfico, downloads com fila (yt-dlp),
letras sincronizadas, loop A–B, filtros de vídeo, filtro de chat, deslikes e mais.

**Versão atual: 6.2** — [baixar o .zip](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases/download/v6.2/JG-YouTube-Enhancer-v6.2.zip) · [todas as versões](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases)

## Instalação (primeira vez)

1. Baixe o `.zip` acima e extraia numa pasta permanente (ex.: `Documentos\JG-YouTube-Enhancer`).
2. Abra `chrome://extensions`, ative o **Modo do desenvolvedor** e clique em **Carregar sem compactação**, escolhendo a pasta extraída.
3. Para os downloads: instale o [Python](https://www.python.org/) marcando *Add python.exe to PATH* e rode o `instalar_host.bat` da pasta.
   Ele instala o yt-dlp, baixa o FFmpeg e registra o host — não precisa digitar nada.

## Atualizações

A extensão verifica sozinha. Quando sair uma versão nova aparece um aviso no YouTube e um ponto verde no botão **JG**.
No painel, clique em **Atualizar agora**: ela baixa, confere a integridade e recarrega sozinha.
Sem o host instalado, use **Atualizar manualmente**: extraia o `.zip` novo por cima da pasta atual e clique em **Já extraí — recarregar**.

## Novidades da 6.2

### v6.2 — Atualizações automáticas (2026-11-20)

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

[Histórico completo](CHANGELOG.md)

---
FFmpeg: binário de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/) (licença GPL), distribuído sem modificações; código-fonte em https://ffmpeg.org.
