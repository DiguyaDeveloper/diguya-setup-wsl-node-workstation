# my-workspace-windows

## Install Chocolatey

### Run

Get-ExecutionPolicy

### If it returns Restricted, then run 

Set-ExecutionPolicy AllSigned 

### or 

Set-ExecutionPolicy Bypass -Scope Process

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

## Install Node

choco install nodejs

## Install Git

choco install git.install

## Install VS Code

choco install vscode

## Install Dotnet

choco install dotnetcore-sdk

## Install Dotnet 2.1.401

choco install dotnetcore-sdk --version=2.1.401

## Install Dbeaver

choco install dbeaver

## Install sourcetree

choco install sourcetree


## Install NVM

choco install nvm


## Install docker

choco install docker

## Install Chrome

choco install googlechrome

## Install firefox

choco install firefox

## Install firefox dev

choco install firefox-dev --pre 


################### 


## After restart powershell

### configure git

git config --global user.name "username"

git config --global user.email "email"

## Check config 

git config user.name
git config user.email

# Install angular CLI


npm install -g npm 

npm install -g @angular/cli

## Config version node 

nvm install 10.9.0
nvm use 10.9.0

## Instal Discord

choco install discord

## Install Slack

choco install slack

## Config aux to npm

npm config set legacy-peer-deps true
