# Configurando um ambiente Node.js com Windows Subsystem for Linux (WSL) e terminal ZSH

Este guia irá ajudá-lo a configurar um ambiente de desenvolvimento Node.js no Windows usando o Windows Subsystem for Linux (WSL) e o terminal ZSH.

## Instale o WSL

Primeiro, instale o WSL com as seguintes etapas:

```
wsl --install
wsl --install -d Ubuntu
wsl --set-default-version 2
```

## Configure o .wslconfig

Crie um arquivo chamado `.wslconfig` em `C:\Users\<seu-usuário>` e adicione o seguinte conteúdo para melhorar os limites de desempenho:

```
[wsl2]
memory=8GB
processors=4
swap=2GB
```

## Instale o ZSH e o Oh My Zsh

Instale o ZSH e o Oh My Zsh para melhorar sua experiência com o terminal:

```
sudo apt update
sudo apt install zsh
sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## Abra o ZSH

Abra o arquivo `~/.zshrc` no Visual Studio Code ou seu editor de escolha para configurar o tema:

```
code ~/.zshrc
```

## Configure um tema no ZSH

Dentro do arquivo `~/.zshrc`, atualize a linha a seguir para definir um tema. Por exemplo:

```
ZSH_THEME="crcandy"
```

## Instale o NVM (Node Version Manager)

Use o seguinte comando para instalar o NVM:

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

## Instale a versão estável do Node.js

Instale a versão estável mais recente do Node.js com o NVM:

```
nvm install stable
```

## Instale o NPM (Node Package Manager)

Finalmente, instale o NPM globalmente:

```
npm install -g npm
```

Agora você tem um ambiente de desenvolvimento Node.js configurado no Windows usando o WSL e o terminal ZSH. Você pode começar a desenvolver aplicativos Node.js com facilidade. Certifique-se de que todas as etapas foram concluídas com sucesso e que seu ambiente está funcionando corretamente.
