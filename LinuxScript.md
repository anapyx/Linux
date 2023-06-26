# LINUX SCRIPT
Linux Mint LMDE 5.

# Programas
Opera

Chrome

Vscode

IntelliJ

Spotify

Krita

Steam

Zoom

qBittorrent

OBS Studio

Shotcut

Handbrake

Anbox


## Utilitários

Git

Python

JDK

GDebi/Synaptic

Mesa digitalizadora

<details>
    <summary> Configurar </summary>

Verificar as bibliotecas e pacotes em *https://linuxwacom.github.io*.
Caso o programa não inicie, modificar o Styli do arquivo Intuos (control+comando):
```console

sudo xed /usr/share/libwacom/intuos-s-p3.tablet
Styli=@intuospt3;0xffffe;
```

</details>


# Tema & Workflow

## Ajustes iniciais
- Configurações do Sistema, em Janelas>Alt-tab>Switcher style selecionar Overflow 3D.
- Em Hot Corners, o canto superior esquerdo mostra todas as janelas.
- Em Extensões, baixar Transparent panels. Configurar para semi-transparent e usar o tema atual.

## Instalar tema
- No terminal, instalar os pacotes:
```console
sudo apt install sassc optipng inkscape libcanberra-gtk-module libglib2.0.dev libxml2-utils git
```
- Em Downloads, clonar os respositórios:
```console
git clone https://github.com/vinceliuice/WhiteSur-gtk-theme.git
git clone https://github.com/vinceliuice/WhiteSur-icon-theme.git
```
- Nas pastas criadas, executar os arquivos *./install.sh*.
- Em temas, selecionar os temas instalados para janelas, ícones, controles e desktop.

## Configurar painel e applets.
- Colocar a barra do painel na parte superior, tirar os programas e ícone do Mint. Com o botão direito no painel, abrir o Applets, instalar o Cinnamenu e substituir pelo Menu Iniciar. Configurar ícone, leiaute e definir o sessions button location em "top".
- Adicionar em Applets: Weather, Scale, Expo, User.
- Alterar o formato da data para "%e de %B, %H:%M".

## Configurar Plank Doc
- No terminal:
```console
sudo apt install plank
```
- Abrir o Plank, transferir arquivos do Whitesur GTK de temas do Plank para */home/.local/share/plank/themes*.
- Com o mouse no Plank, pressionar control+botão direito e ir em preferências, ajustar o tema para "theme-dark", ativar icon zoom, adicionar lixeira e desktop. Fixar todos os programas desejados no Plank com o botão direito.
- Ativar o Plank em startup applications.

## Google Calendar

<details>
    <summary>Configurar</summary>
  
Padrão
```console
sudo apt install gcalendar
```

Pelo Pypi:
```console
sudo apt install python3-pip python3-setuptools python3-dateutil python3-oauth2client python3-googleapi
pip3 install gcalendar
```

Pela fonte:
```console
sudo apt install python3-pip python3-setuptools python3-dateutil python3-oauth2client python3-googleapi git
git clone https://github.com/slgobinath/gcalendar.git
cd gcalendar
pip3 install -e
```

- Executar no terminal para autorizar o acesso:
```console
gcalendar
```
- Em Desklets, adicionar Google Calendar.

</details>

## Opcionais:

### Albert Launcher
Rapidez em buscas no workflow.
- Download: [Albert Launcher Package](https://software.opensuse.org/download.html?project=home%3Amanuelschneid3r&package=albert)
- Tema: [Albert Theme - BigSur](https://store.kde.org/p/1410038/)
- Em *usr/share/albert/* (abrir como root) *org.albert.frontend.widgetboxmodel/themes* colar os arquivos do tema.
- Reiniciar o Albert, com o botão direito ir em Settings e aplicar o tema BigSur_Dark.
- Setar para abrir ao iniciar, tecla de ativação sendo alt+space, ativar extensões: applications, calc, files, system, terminal e websearch.

### Nautilus
Gerenciador de arquivos padrão.

*Créditos: adaptações de [LinuxScoop YouTube Tutorial](https://youtu.be/DMs7DX3Um9E "YouTube video")*

## SHELL
Bash
- Tema: Oh My Bash - Font (default)
