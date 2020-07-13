# notitrans

[🇧🇷] Um script em shell que mostra uma notificação com uma tradução para o texto selecionado.

[🇺🇸] A shell script that shows up a notification with a translation for the selected text.

![](https://github.com/lyangmdrs/notitrans/blob/master/use_example.gif)

# Dependencies

- notify-send (this tool is usually already installed on your system): `sudo apt install libnotify-bin`
- xsel: `sudo apt install xsel`
- translate-shell: `sudo apt install translate-shell`

# How to use it
- [🇧🇷] Mova o script para um diretório cujo caminho já esteja presente na sua variável de ambiente **$PATH**;
- [🇺🇸] Move the script to a directory whose path is in your **$PATH** variable;
  - Example:
  
    `git clone https://github.com/lyangmdrs/notitrans.git`
  
    `cd notitrans`
    
    `chmod +x notitrans`
  
    `sudo mv notitrans /usr/local/bin/`
- [🇧🇷] Cire um novo atalho de teclado para executar o script;
- [🇺🇸] Create a new keyboard shortcut for run the script;
  - Example:
  ![](https://github.com/lyangmdrs/notitrans/blob/master/shortcut_example.png)
