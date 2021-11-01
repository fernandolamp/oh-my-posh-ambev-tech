# Oh-my-posh tema baseado no Powerlevel10k and Pwsh10k


![PWSH10k PREVIEW](https://user-images.githubusercontent.com/18193204/139718154-581fdd9a-398a-47b1-9741-630ef5cff7f7.png)<space><space>
Preview
 
## Prerequisitos

1. Windows Terminal ([Como instalar](https://docs.microsoft.com/en-us/windows/terminal/get-started "Instalar windows terminal"))

2. (Opcional, mas recomendado) Atualizar para Powershell core 7  ([Update!](https://docs.microsoft.com/en-us/powershell/scripting/install/migrating-from-windows-powershell-51-to-powershell-7?view=powershell-7.1))

3. Download da fonte MesloLGS NF (essa é a fonte usada pelo oh-my-posh):


* [MesloLGS NF Regular.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Regular.ttf)

* [MesloLGS NF Bold.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Bold.ttf)

* [MesloLGS NF Italic.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Italic.ttf)

* [MesloLGS NF Bold Italic.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Bold%20Italic.ttf)

Clique duplo em cada arquivo e escolha instalar, ou selecione todos e clique instalar.

Depois de instalado configure o seu windows terminal para usar essa fonte, é possível abrir as configurações pelo atalho `(Ctrl+,)`, procure pela configuração da fonte e selecione `Meslogs NF` para cada perfil ou como a fonte padrão de todos os perfis.


4. Execute no powershell: `Install-Module posh-git -Scope CurrentUser`, `Install-Module oh-my-posh -Scope CurrentUser`, e `Update-Module -Name oh-my-posh -AllowPrerelease -Scope CurrentUser`

5. Crie um perfil no powershell (se já não tiver): `New-Item -ItemType File -Path $PROFILE`

6. Copie o arquivo `pwsh10k-ambev-tech.omp.json` para sua pasta `Home` do windows.

    Se não souber onde fica essa pasta, abra o powershell e digite:


    ```powershell
    cd ~  
    pwd
    ```

    Será exibido o seu diretório do home


7. Abra o arquivo de profile `$profile` no seu editor de texto favorito. (VScode: `code $profile`, Notepad: `notepad $profile`)


8. Adicione essas linhas

    ```powershell
    Import-Module posh-git
    Import-Module oh-my-posh
    Set-PoshPrompt -Theme  ~/pwsh10k-ambev-tech.omp.json
    ```

Reinicie o seu terminal e veja o resultado.

## Use a fonte correta na integração com o VSCode

* Visual Studio Code: Open File → Preferences → Settings, digite terminal.integrated.fontFamily na caixa de procura de texto e configure o valor para MesloLGS NF


## Creditos (Credits )
  This project was inpired on project https://github.com/Kudostoy0u/pwsh10k