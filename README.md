# Austin's qutebrowser UserScripts

## Quickly Install All UserScripts
```bash
mkdir -pv ~/.local/share/qutebrowser/userscripts/
mkdir -pv ~/Downloads/qutebrowser-userscripts
git clone https://github.com/loweryaustin/qutebrowser-userscripts.git ~/Downloads/qutebrowser-userscripts
cp -v ~/Downloads/qutebrowser-userscripts/*.sh ~/.local/share/qutebrowser/userscripts/
```

## Quickly Install a Single UserScript
```bash
mkdir -pv ~/.local/share/qutebrowser/userscripts/
mkdir -pv ~/Downloads/qutebrowser-userscripts
git clone https://github.com/loweryaustin/qutebrowser-userscripts.git ~/Downloads/qutebrowser-userscripts
# Optionally list the scripts that are avaialble:
ls -lah ~/Downloads/qutebrowser-userscripts
# Move the script that you want to use into the folder that qutebrowser reads scripts from. The live-reload.sh script is used in this example:
cp -v ~/Downloads/qutebrowser-userscripts/live-reload.sh ~/.local/share/qutebrowser/userscripts/
cat ~/.local/share/qutebrowser/userscripts/live-reload.sh
```

**NOTE**: More in depth information can be found as comments within the scripts themselves

## live-reload.sh

Enables a user to live reload any webpage when a file is added,
removed, or modified within a directory on their local filesystem.
Standard application would be for a web developer who is editing a website
that is being served from his/her local computer. Atypical use might be to
reload an arbitrary webpage in Qutebrowser based on some filesystem event on
the local computer.

