# Pedro Fernandes Filho's VSCode files

Install instructions for Windows on PowerShell:

**This will remove existing `keybindings.json` and `settings.json` files.**

**Windows**

```powershell
cd $APPDATA\Roaming\Code\User
git init -b main
git remote add origin git@github.com:pedrofernandesfilho/vscodefiles.git
rm .\keybindings.json, .\settings.json -- ErrorAction SilentlyContinue
git pull origin main
```

**Linux**

```zsh
cd ~/.config/Code/User
git init -b main
git remote add origin git@github.com:pedrofernandesfilho/vscodefiles.git
[ -f keybindings.json ] && rm keybindings.json
[ -f settings..json ] && rm settings.json
git pull -r origin main
```