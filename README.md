# Install Oh My Posh
[https://ohmyposh.dev/docs/installation/windows](https://ohmyposh.dev/docs/installation/windows)

1. winget install JanDeDobbeleer.OhMyPosh -s winget
2. New-Item -Path $PROFILE -Type File -Force
3. notepad $PROFILE
```PowerShell
. $env:USERPROFILE\.config\powershell\user_profile.ps1
```
4. Copiar carpeta **powershell** a *~/.config*
5. Instalar fuentes de NerdFonts (Hack): [https://www.nerdfonts.com/](https://www.nerdfonts.com/)
6. Instalar **PowerShell** de la Microsoft Store
7. Configurar Windows Terminal:
    - Nueva PowerShell como terminal por defecto
    - Apariencia > Tipo de fuente: Hack Nerd Font Mono
    - Apariencia > Opacidad del fondo: 50%
    - Apariencia > Habilitar material acrílico: Activado
    - Apariencia > Combinación de colores: One Half Dark v2
    - Editar JSON:
```json
        {
            "background": "#001B26",
            "black": "#282C34",
            "blue": "#61AFEF",
            "brightBlack": "#5A6374",
            "brightBlue": "#61AFEF",
            "brightCyan": "#56B6C2",
            "brightGreen": "#98C379",
            "brightPurple": "#C678DD",
            "brightRed": "#E06C75",
            "brightWhite": "#DCDFE4",
            "brightYellow": "#E5C07B",
            "cursorColor": "#FFFFFF",
            "cyan": "#56B6C2",
            "foreground": "#DCDFE4",
            "green": "#98C379",
            "name": "One Half Dark v2",
            "purple": "#C678DD",
            "red": "#E06C75",
            "selectionBackground": "#FFFFFF",
            "white": "#DCDFE4",
            "yellow": "#E5C07B"
        },
```
8. Instalar módulos:
```PowerShell
Install-Module posh-git -Scope CurrentUser -Force
Install-Module -Name Terminal-Icons -Repository PSGallery -Force
Install-Module -Name z -Force
Install-Module -name PSFzf -Scope CurrentUser -Force
```
9. Instalar **fzf**:
```PowerShell
choco install fzf
```
10. Configurar VSCode:
```json
    "terminal.integrated.fontFamily": "Hack Nerd Font Mono",
    "terminal.integrated.defaultProfile.windows": "PowerShell",
```
