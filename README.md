# Pedro Fernandes Filho's VSCode files

Install instructions for Windows on PowerShell:

**This will remove existing `keybindings.json` and `settings.json` files.**

```powershell
cd $APPDATA\Roaming\Code\User
git init
git remote add origin git@github.com:pedrofernandesfilho/vscodefiles.git
rm .\keybindings.json, .\settings.json -- ErrorAction SilentlyContinue
git pull origin main
```