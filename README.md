# JG YouTube Enhancer

Extensão para Chrome / Edge / Brave que turbina o YouTube: EQ gráfico, downloads com fila (yt-dlp),
letras sincronizadas, loop A–B, filtros de vídeo, filtro de chat, deslikes e mais.

**Versão atual: 6.3** — [baixar o .zip](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases/download/v6.3/JG-YouTube-Enhancer-v6.3.zip) · [todas as versões](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases)

## Instalação (primeira vez)

1. Baixe o `.zip` acima e extraia numa pasta permanente (ex.: `Documentos\JG-YouTube-Enhancer`).
2. Abra `chrome://extensions`, ative o **Modo do desenvolvedor** e clique em **Carregar sem compactação**, escolhendo a pasta extraída.
3. Para os downloads: instale o [Python](https://www.python.org/) marcando *Add python.exe to PATH* e rode o `instalar_host.bat` da pasta.
   Ele instala o yt-dlp, baixa o FFmpeg e registra o host — não precisa digitar nada.

## Atualizações

A extensão verifica sozinha. Quando sair uma versão nova aparece um aviso no YouTube e um ponto verde no botão **JG**.
No painel, clique em **Atualizar agora**: ela baixa, confere a integridade e recarrega sozinha.
Sem o host instalado, use **Atualizar manualmente**: extraia o `.zip` novo por cima da pasta atual e clique em **Já extraí — recarregar**.

## Novidades da 6.3

### v6.3 — SponsorBlock e biblioteca de letras (2026-11-20)

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

[Histórico completo](CHANGELOG.md)

---
FFmpeg: binário de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/) (licença GPL), distribuído sem modificações; código-fonte em https://ffmpeg.org.
