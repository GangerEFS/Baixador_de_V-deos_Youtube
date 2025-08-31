# Baixador de Vídeos YouTube 🎬🎵

## Descrição
O **Baixador de Vídeos YouTube** é uma aplicação desktop em Python que permite baixar vídeos e áudios do YouTube de forma simples, com interface gráfica moderna usando **CustomTkinter**.  
O usuário pode escolher a resolução do vídeo e acompanhar o progresso do download em tempo real.

---

## Funcionalidades
- Baixar vídeos do YouTube em diferentes resoluções.  
- Baixar apenas o áudio de vídeos.  
- Spinner indicando que o download está em andamento.  
- Mensagem de sucesso ao término do download.  
- Interface gráfica moderna e responsiva.  
- Suporte a downloads em alta resolução (DASH) com áudio separado opcional.  

---

## Tecnologias
- Python 3.13+  
- [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) – interface gráfica  
- [Pytube / Pytubefix](https://github.com/pytube/pytube) – download de vídeos  
- Threading – para downloads sem travar a interface  
- [FFmpeg](https://ffmpeg.org/) (opcional) – para unir vídeo e áudio DASH  

---

## Estrutura do Projeto

BaixadorDeVideosYouTube/

  ├── baixar_gui.py # Script principal.
 
  ├── baixar_gui_spinner.py # Versão com spinner e threads.
 
  ├── baixar_gui_resolucao.py # Versão com escolha de resolução.
 
  ├── README.md # Este arquivo.
 
  ├── venv/ # Ambiente virtual.
 
  └── downloads/ # Onde vídeos e áudios são salvos.

---

## Pré-requisitos
- Python 3.13+  
- Bibliotecas Python:
```bash
pip install customtkinter
pip install pytube       # ou pytubefix
pip install moviepy      # opcional, se for unir vídeo e áudio
pip install ffmpeg-python # opcional, manipulação de vídeo
```
FFmpeg (para unir vídeo e áudio DASH):

 Linux: sudo pacman -S ffmpeg

 Windows: baixar do site oficial


Como Usar:

1. Abra o .exe no arquivo.

2. Cole o link do vídeo no campo de entrada.

3. Para vídeos: clique Baixar Vídeo, escolha a resolução, clique Baixar.

4. Para áudios: clique Baixar Áudio.

5. Aguarde o spinner girando até aparecer “Baixado com êxito!”.

6. Arquivos salvos nas pastas videos/ e audios/.

Observações

Vídeos acima de 720p podem precisar baixar vídeo e áudio separados (DASH).

Caso queira unir vídeo + áudio automaticamente, instale ffmpeg e moviepy.

Evite links privados, restritos ou bloqueados regionalmente.

Licença

Este projeto é open-source. Sinta-se à vontade para usar, modificar e compartilhar.























 
