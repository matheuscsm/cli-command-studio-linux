# CLI Command Studio (Linux)

Interface gráfica nativa para Linux desenvolvida em Python (Tkinter) para centralizar e simplificar o uso das ferramentas de linha de comando mais populares de download e processamento de mídia: **yt-dlp**, **FFmpeg**, **Instaloader** e **spotDL**.

Projetado para ser distribuído como um pacote nativo `.deb` autossuficiente, com ambiente virtual (`venv`) isolado em `/opt/cli-command-studio/`, evitando conflitos com o gerenciador de pacotes do sistema operacional.

---

## ✨ Recursos

- **Ambiente Isolado:** Todas as bibliotecas e executáveis Python rodam em `/opt/cli-command-studio/venv`, sem interferir no Python global do sistema.
- **Integração com Desktop:** Atalho integrado no menu de aplicativos, ícone em alta definição e suporte a agrupamento correto na Dock/Barra de tarefas (`StartupWMClass=Clicommandstudio`).
- **Destino Inteligente:** Download direcionado automaticamente para a pasta `~/Downloads` do usuário.
- **Validação de Ferramentas:** Verificação de status em tempo real de binários essenciais (`yt-dlp`, `ffmpeg`, `instaloader`, `spotdl`).

---

## 📦 Instalação via Pacote `.deb`

A forma mais rápida de instalar em distribuições baseadas em Debian/Ubuntu (Ubuntu, Linux Mint, Pop!_OS, Debian):

1. Baixe o pacote mais recente na [página de Releases](https://github.com/matheuscsm/cli-command-studio-linux/releases).
2. Abra o terminal na pasta do arquivo baixado e instale via APT:
   ```bash
   sudo apt install ./cli-command-studio_1.0.0_amd64.deb
