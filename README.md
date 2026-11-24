# JG YouTube Enhancer

Extensão para Chrome / Edge / Brave que turbina o YouTube: EQ gráfico, downloads com fila (yt-dlp),
letras sincronizadas, loop A–B, filtros de vídeo, filtro de chat, deslikes e mais.

**Versão atual: 6.5** — [baixar o .zip](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases/download/v6.5/JG-YouTube-Enhancer-v6.5.zip) · [todas as versões](https://github.com/JamalOruim/jg-yt-enhancer-releases/releases)

## Instalação (primeira vez)

1. Baixe o `.zip` acima e extraia numa pasta permanente (ex.: `Documentos\JG-YouTube-Enhancer`).
2. Abra `chrome://extensions`, ative o **Modo do desenvolvedor** e clique em **Carregar sem compactação**, escolhendo a pasta extraída.
3. Para os downloads: instale o [Python](https://www.python.org/) marcando *Add python.exe to PATH* e rode o `instalar_host.bat` da pasta.
   Ele instala o yt-dlp, baixa o FFmpeg e registra o host — não precisa digitar nada.

## Atualizações

A extensão verifica sozinha. Quando sair uma versão nova aparece um aviso no YouTube e um ponto verde no botão **JG**.
No painel, clique em **Atualizar agora**: ela baixa, confere a integridade e recarrega sozinha.
Sem o host instalado, use **Atualizar manualmente**: extraia o `.zip` novo por cima da pasta atual e clique em **Já extraí — recarregar**.

## Novidades da 6.5

### v6.5 — Nightcore, Slowed + Reverb e estabilidade (2026-11-23)

**Novo**
- Áudio → Efeito de velocidade: Nightcore (mais rápido e agudo) e Slowed + Reverb (mais lento, grave e com ambiência)
- Ajuste de velocidade e de reverb em cada efeito, mostrando quantos semitons o tom mudou
- Atalho Shift+V alterna Normal → Nightcore → Slowed + Reverb
- Mini HUD mostra quando um efeito de velocidade está ligado

**Alterado**
- O efeito continua ligado ao ir para o próximo vídeo e depois de recarregar a página
- Trocar a velocidade pelo menu do YouTube, pelo painel ou pelo Turbo desliga o efeito, sem brigar com a sua escolha
- Ao desligar o efeito, a velocidade volta ao que estava antes

**Removido**
- Nightcore como preset de EQ (virou um efeito próprio, que não é desligado pelo EQ automático)

**Corrigido**
- Nightcore deixava de funcionar ao passar para o próximo vídeo e precisava ser reaplicado
- A extensão podia sumir do navegador: o host agora limpa da pasta arquivos com "_" no nome, que o navegador recusa

[Histórico completo](CHANGELOG.md)

---
FFmpeg: binário de [gyan.dev](https://www.gyan.dev/ffmpeg/builds/) (licença GPL), distribuído sem modificações; código-fonte em https://ffmpeg.org.
