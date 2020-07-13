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
- [🇺🇸] Create a new keyboard shortcut to run the script;
  - Example:
  ![](https://github.com/lyangmdrs/notitrans/blob/master/shortcut_example.png)

# How to configure the target language
By default, the target language in the script is Portuguese 🇧🇷. To set another language you need to edit the script in the highlighted part below.
- notify-send -i emblem-default " Tradução:" "&#96;xsel -o | sed ':a;N;$!ba;s/\n/ /g' | trans -b -t **pt**&#96;"

In this case **pt** is the code for Potuguese Language. You can see all the supported languages and their respective codes by typing `trans -R` in a terminal.

To set the script to translate for Spanish, for example:
- notify-send -i emblem-default " Tradução:" "&#96;xsel -o | sed ':a;N;$!ba;s/\n/ /g' | trans -b -t **es**&#96;"
